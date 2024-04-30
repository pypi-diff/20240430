# Comparing `tmp/BsSalary_Extractor-1.3.7.tar.gz` & `tmp/bssalary_extractor-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BsSalary_Extractor-1.3.7.tar", last modified: Mon Feb 19 11:14:06 2024, max compression
+gzip compressed data, was "bssalary_extractor-1.3.8.tar", last modified: Tue Apr 30 14:09:33 2024, max compression
```

## Comparing `BsSalary_Extractor-1.3.7.tar` & `bssalary_extractor-1.3.8.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-02-19 11:14:06.418834 BsSalary_Extractor-1.3.7/
-drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-02-19 11:14:06.417296 BsSalary_Extractor-1.3.7/BsSalary_Extractor/
--rw-r--r--   0 fahadpatel   (501) staff       (20)        0 2023-11-15 17:50:27.000000 BsSalary_Extractor-1.3.7/BsSalary_Extractor/__init__.py
--rw-r--r--   0 fahadpatel   (501) staff       (20)     1522 2023-11-15 20:20:46.000000 BsSalary_Extractor-1.3.7/BsSalary_Extractor/constants.py
--rw-r--r--   0 fahadpatel   (501) staff       (20)    23476 2024-02-19 11:12:02.000000 BsSalary_Extractor-1.3.7/BsSalary_Extractor/data_extractor.py
--rw-r--r--   0 fahadpatel   (501) staff       (20)    11629 2024-02-13 07:20:51.000000 BsSalary_Extractor-1.3.7/BsSalary_Extractor/data_extractor2.py
--rw-r--r--   0 fahadpatel   (501) staff       (20)    26226 2024-02-19 11:12:21.000000 BsSalary_Extractor-1.3.7/BsSalary_Extractor/functions.py
-drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-02-19 11:14:06.418396 BsSalary_Extractor-1.3.7/BsSalary_Extractor.egg-info/
--rw-r--r--   0 fahadpatel   (501) staff       (20)     1223 2024-02-19 11:14:06.000000 BsSalary_Extractor-1.3.7/BsSalary_Extractor.egg-info/PKG-INFO
--rw-r--r--   0 fahadpatel   (501) staff       (20)      442 2024-02-19 11:14:06.000000 BsSalary_Extractor-1.3.7/BsSalary_Extractor.egg-info/SOURCES.txt
--rw-r--r--   0 fahadpatel   (501) staff       (20)        1 2024-02-19 11:14:06.000000 BsSalary_Extractor-1.3.7/BsSalary_Extractor.egg-info/dependency_links.txt
--rw-r--r--   0 fahadpatel   (501) staff       (20)      373 2024-02-19 11:14:06.000000 BsSalary_Extractor-1.3.7/BsSalary_Extractor.egg-info/requires.txt
--rw-r--r--   0 fahadpatel   (501) staff       (20)       19 2024-02-19 11:14:06.000000 BsSalary_Extractor-1.3.7/BsSalary_Extractor.egg-info/top_level.txt
--rw-r--r--   0 fahadpatel   (501) staff       (20)     1068 2023-11-15 21:11:53.000000 BsSalary_Extractor-1.3.7/LICENSE
--rw-r--r--   0 fahadpatel   (501) staff       (20)       32 2024-02-13 07:20:51.000000 BsSalary_Extractor-1.3.7/MANIFEST.in
--rw-r--r--   0 fahadpatel   (501) staff       (20)     1223 2024-02-19 11:14:06.418738 BsSalary_Extractor-1.3.7/PKG-INFO
--rw-r--r--   0 fahadpatel   (501) staff       (20)        0 2023-11-15 21:21:38.000000 BsSalary_Extractor-1.3.7/README.md
--rw-r--r--   0 fahadpatel   (501) staff       (20)      107 2023-11-15 21:11:34.000000 BsSalary_Extractor-1.3.7/pyproject.toml
--rw-r--r--   0 fahadpatel   (501) staff       (20)      588 2024-02-19 11:14:06.419181 BsSalary_Extractor-1.3.7/setup.cfg
--rw-r--r--   0 fahadpatel   (501) staff       (20)      736 2024-02-19 11:12:55.000000 BsSalary_Extractor-1.3.7/setup.py
+drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-30 14:09:33.522063 bssalary_extractor-1.3.8/
+drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-30 14:09:33.520401 bssalary_extractor-1.3.8/BsSalary_Extractor/
+-rw-r--r--   0 fahadpatel   (501) staff       (20)        0 2023-11-15 17:50:27.000000 bssalary_extractor-1.3.8/BsSalary_Extractor/__init__.py
+-rw-r--r--   0 fahadpatel   (501) staff       (20)     1522 2023-11-15 20:20:46.000000 bssalary_extractor-1.3.8/BsSalary_Extractor/constants.py
+-rw-r--r--   0 fahadpatel   (501) staff       (20)    25564 2024-04-26 11:45:08.000000 bssalary_extractor-1.3.8/BsSalary_Extractor/data_extractor.py
+-rw-r--r--   0 fahadpatel   (501) staff       (20)    11629 2024-02-13 07:20:51.000000 bssalary_extractor-1.3.8/BsSalary_Extractor/data_extractor2.py
+-rw-r--r--   0 fahadpatel   (501) staff       (20)    13508 2024-04-30 13:46:23.000000 bssalary_extractor-1.3.8/BsSalary_Extractor/data_extractor_only_sc.py
+-rw-r--r--   0 fahadpatel   (501) staff       (20)    25023 2024-04-25 12:09:42.000000 bssalary_extractor-1.3.8/BsSalary_Extractor/data_extractor_revibe.py
+-rw-r--r--   0 fahadpatel   (501) staff       (20)    28058 2024-04-30 11:39:47.000000 bssalary_extractor-1.3.8/BsSalary_Extractor/functions.py
+drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-30 14:09:33.521532 bssalary_extractor-1.3.8/BsSalary_Extractor.egg-info/
+-rw-r--r--   0 fahadpatel   (501) staff       (20)     2854 2024-04-30 14:09:33.000000 bssalary_extractor-1.3.8/BsSalary_Extractor.egg-info/PKG-INFO
+-rw-r--r--   0 fahadpatel   (501) staff       (20)      531 2024-04-30 14:09:33.000000 bssalary_extractor-1.3.8/BsSalary_Extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 fahadpatel   (501) staff       (20)        1 2024-04-30 14:09:33.000000 bssalary_extractor-1.3.8/BsSalary_Extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 fahadpatel   (501) staff       (20)     1269 2024-04-30 14:09:33.000000 bssalary_extractor-1.3.8/BsSalary_Extractor.egg-info/requires.txt
+-rw-r--r--   0 fahadpatel   (501) staff       (20)       19 2024-04-30 14:09:33.000000 bssalary_extractor-1.3.8/BsSalary_Extractor.egg-info/top_level.txt
+-rw-r--r--   0 fahadpatel   (501) staff       (20)     1068 2023-11-15 21:11:53.000000 bssalary_extractor-1.3.8/LICENSE
+-rw-r--r--   0 fahadpatel   (501) staff       (20)       32 2024-02-13 07:20:51.000000 bssalary_extractor-1.3.8/MANIFEST.in
+-rw-r--r--   0 fahadpatel   (501) staff       (20)     2854 2024-04-30 14:09:33.521979 bssalary_extractor-1.3.8/PKG-INFO
+-rw-r--r--   0 fahadpatel   (501) staff       (20)        0 2023-11-15 21:21:38.000000 bssalary_extractor-1.3.8/README.md
+-rw-r--r--   0 fahadpatel   (501) staff       (20)      107 2023-11-15 21:11:34.000000 bssalary_extractor-1.3.8/pyproject.toml
+-rw-r--r--   0 fahadpatel   (501) staff       (20)      588 2024-04-30 14:09:33.522410 bssalary_extractor-1.3.8/setup.cfg
+-rw-r--r--   0 fahadpatel   (501) staff       (20)      736 2024-04-30 14:07:16.000000 bssalary_extractor-1.3.8/setup.py
```

### Comparing `BsSalary_Extractor-1.3.7/BsSalary_Extractor/constants.py` & `bssalary_extractor-1.3.8/BsSalary_Extractor/constants.py`

 * *Files identical despite different names*

### Comparing `BsSalary_Extractor-1.3.7/BsSalary_Extractor/data_extractor.py` & `bssalary_extractor-1.3.8/BsSalary_Extractor/data_extractor_revibe.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,60 +53,97 @@
                 )
             return response.choices[0]["message"]["content"]
         
         def extract_data_for_SC(self, doc):
             extraction_input = perform_data_extraction(self.client, self.pdf_bytes)
             result_data = self.get_sal_and_name_from_SC(str(extraction_input))
             result_data = json.loads(result_data)
-            
-            if result_data['name'].lower() == 'john doe' or result_data['company_name'].lower() in ['abc company', 'xyz company']:
+            result_data['extracted_data'] = extraction_input
+
+            if result_data.get('name', '').lower() == 'john doe' or result_data.get('company_name', '').lower() in ['abc company', 'xyz company']:
                 data = get_scanned_pdf_text(doc)
                 result_data = self.get_sal_and_name_from_SC(str(data))
                 result_data = json.loads(result_data)
+                result_data['extracted_data'] = data
             
-            if result_data.get('date_of_issue') and not re.match(r'^\d{2}/\d{2}/\d{4}$', result_data['date_of_issue']):
+            if result_data.get('date_of_issue', '') and not re.match(r'^\d{2}/\d{2}/\d{4}$', result_data.get('date_of_issue', '')):
                 result_data['date_of_issue'] = clean_and_convert_date(result_data['date_of_issue'])
 
-            if re.match(r'^\d{2}/\d{2}/\d{4}$', result_data['date_of_issue']):
+            if re.match(r'^\d{2}/\d{2}/\d{4}$', result_data.get('date_of_issue', '')):
                 result_data['date_of_issue'] = hijri_to_gregorian(result_data['date_of_issue'])
 
-            result_data['salary'] = clean_salary(result_data['salary'])
-            result_data['salary'] = eastern_arabic_to_english(result_data['salary'])
+            result_data['salary'] = clean_salary(result_data.get('salary', ''))
+            result_data['salary'] = eastern_arabic_to_english(result_data.get('salary', ''))
 
             ## handle salary decimal in start
             l = [i for i in result_data['salary']]
             if len(l)>0 and l[0] == '.':
                     result_data['salary'] = ''.join(result_data['salary'][1:])
 
-            language = detect_language(result_data['name'])
+            language = detect_language(result_data.get('name', ''))
+
             if language == 'ar':
                 customer_name = self.customer_name_ar.lower()
             else:
                 customer_name = self.customer_name.lower()
             
-            Name_check = validate_name(customer_name,result_data['name'].lower())
-            if not Name_check:
-                raise Exception("Name Mismatch Error")
-            
-            is_more_than_3_months = months_difference_with_grace_period(result_data['date_of_issue'])>=3
-            if is_more_than_3_months:    
-                raise Exception("Overdated bank statement")
+            Name_check = validate_name(customer_name,result_data.get('name', '').lower())
+            # if not Name_check:
+                # raise Exception("Name Mismatch Error")
+            
+            is_more_than_3_months = months_difference_with_grace_period(result_data.get('date_of_issue', ''))>=3
+            # if is_more_than_3_months:    
+                # raise Exception("Overdated Salary Certificate")
             
             return result_data
         
+
+        def standardize_keys(self, data):
+            key_mapping = {
+                'name': 'name',
+                'Name': 'name',
+                'Customer Name': 'name',
+                'Employee Name': 'name',
+                'company_name': 'company_name',
+                'Company Name': 'company_name',
+                'designation': 'designation',
+                'Designation': 'designation',
+                'currency': 'currency',
+                'Currency': 'currency',
+                'date_of_issue': 'date_of_issue',
+                'Date of Issue': 'date_of_issue',
+                'salary': 'salary',
+                'Salary': 'salary'
+            }
+
+            standardized_data = {}
+
+            try:
+                for key, value in data.items():
+                    if key in key_mapping:
+                        standardized_data[key_mapping[key]] = value
+                    else:
+                        standardized_data[key] = value
+
+                return standardized_data
+            
+            except:
+                return data
+
+
         def extract_data(self):
     ### 1. Data Extraction (from pdf) ---------------------------------
 
             doc = fitz.open(stream=self.pdf_bytes, filetype="pdf")
             plain_text_data = []
 
-            #page_count=doc.page_count
+            page_count=doc.page_count
 
-            # if page_count>=30:
-            #     raise Exception("Unrecognized or Unsupported Document")
+            if page_count>1:
+                return {'error': 'not_salary_certificate'}
             
             for page in doc:
                 page_output = [unidecode(block[4]) for block in page.get_text("blocks") if block[6] == 0]
                 if len(page_output)>0:
                     plain_text_data.append(page_output)
                 
                 
@@ -116,14 +153,16 @@
                 plain_text_data=[ele.strip() for ele in plain_text_data if ele.strip() and ele != '\n']
                 plain_text_data=[ele.replace('\n',' ') for ele in plain_text_data]
                 
             else:
                 ### raise an error : nto a valid file
                 try:
                     result = self.extract_data_for_SC(doc)
+                    print(f"result generated here")
+                    result = self.standardize_keys(result)
                     return result
                 except:
                     raise Exception("Unrecognized or Unsupported Document 1")
      
             most_coomon_datepattern=''
             
             enbd_flag=False
@@ -150,14 +189,16 @@
 
             try:
                 plain_text_data=remove_dates_not_matching_format(plain_text_data,most_coomon_datepattern)
             except:
                 try:
                     doc = fitz.open(stream=self.pdf_bytes, filetype="pdf")
                     result_data = self.extract_data_for_SC(doc)
+                    print(f"result generated here 2")
+                    result_data = self.standardize_keys(result_data)
                     return result_data
                 except:
                     raise Exception("Unrecognized or Unsupported Document 2")
 
             plain_text_data=rearrange_dates_in_list(plain_text_data)
 
 
@@ -287,31 +328,32 @@
                 avg_salary=''
 
 
             if len(extraction_input)==0:
                 try:
                     doc = fitz.open(stream=self.pdf_bytes, filetype="pdf")
                     result_data = self.extract_data_for_SC(doc)
+                    result_data = self.standardize_keys(result_data)
                     return result_data
                 except:
-                    raise Exception("Unrecognized or Unsupported Document 2")
+                    raise Exception("Unrecognized or Unsupported Document 3")
             
             ## 6. first transaction date  ---------------------------------
 
             first_trans_date=extract_date_from_string(extraction_input[0], most_coomon_datepattern)
 
             ### 7. last transaction date  ---------------------------------
 
             last_transaction_date=extract_date_from_string(extraction_input[-1], most_coomon_datepattern)
 
             is_more_than_3_months=months_difference_with_grace_period(last_transaction_date)>=3
 
-            if is_more_than_3_months:
+            # if is_more_than_3_months:
                     
-                    raise Exception("Overdated bank statement")
+                    # raise Exception("Overdated bank statement")
 
 #             ### 8. Customer Name Extraction ---------------------------------
 
             Cust_Name=extract_name(plain_text_data)
 
             if not Cust_Name:
                 try:
```

### Comparing `BsSalary_Extractor-1.3.7/BsSalary_Extractor/data_extractor2.py` & `bssalary_extractor-1.3.8/BsSalary_Extractor/data_extractor2.py`

 * *Files identical despite different names*

### Comparing `BsSalary_Extractor-1.3.7/BsSalary_Extractor/functions.py` & `bssalary_extractor-1.3.8/BsSalary_Extractor/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,36 @@
 from hijri_converter import convert
 from datetime import datetime
 import base64
 import cv2
 import numpy as np
 from google.cloud import vision_v1
 import fitz
+from googletrans import Translator
+import PyPDF2
+
+translator = Translator()
+
 ### Define functions
 
+def translate_ar_to_en(front_id_text_desc):
+    try:
+        translated_id_text = translator.translate(front_id_text_desc, src='ar', dest='en').text
+    except:
+        translated_id_text = front_id_text_desc
+        
+    return translated_id_text
+
+def contains_salary(text, keywords):
+    if not text:
+        return False
+    
+    text = text.lower()
+    return any(keyword in text for keyword in keywords)
+
 def pdf_to_bytes(pdf_file_path):
 #     try:
         with open(pdf_file_path, "rb") as pdf_file:
             pdf_bytes = pdf_file.read()
         return pdf_bytes
 
 
@@ -42,25 +62,28 @@
         if re.match(pattern, date_str, re.IGNORECASE):
             given_date = datetime.strptime(date_str, date_format)
             break
     else:
         pass
 
     # Add a grace period of two days
-    adjusted_date = given_date + timedelta(days=2)
-
-    # Get today's date
-    today = datetime.now()
+    try:
+        adjusted_date = given_date + timedelta(days=2)
+        
+        # Get today's date
+        today = datetime.now()
 
-    # Calculate the difference in months
-    month_diff = (today.year - adjusted_date.year) * 12 + today.month - adjusted_date.month
+        # Calculate the difference in months
+        month_diff = (today.year - adjusted_date.year) * 12 + today.month - adjusted_date.month
 
-    # Adjust for day difference within the month
-    if today.day < adjusted_date.day:
-        month_diff -= 1
+        # Adjust for day difference within the month
+        if today.day < adjusted_date.day:
+            month_diff -= 1
+    except:
+        month_diff = 0
 
     return month_diff
 
 def check_dates_and_format_patterns_in_list(date_list):
     date_patterns = {
         r'\b\d{2}/\d{2}/\d{4}\b': "%d/%m/%Y",  # DD/MM/YYYY
         r'\b\d{2}-[a-zA-Z]{3}-\d{4}\b': "%d-%b-%Y",  # DD-MMM-YYYY
@@ -98,19 +121,23 @@
 
         sorted_string = ' '.join(non_digit_words + digit_words)
         sorted_strings.append(sorted_string)
 
     return sorted_strings
 
 def remove_special_characters(input_string):
-    # Using list comprehension to filter out non-letter and non-whitespace characters
-    filtered_characters = [char for char in input_string if char.isalpha() or char.isspace()]
+    try:
+        # Using list comprehension to filter out non-letter and non-whitespace characters
+        filtered_characters = [char for char in input_string if char.isalpha() or char.isspace()]
+        
+        # Joining the filtered characters back into a string
+        return ''.join(filtered_characters)
     
-    # Joining the filtered characters back into a string
-    return ''.join(filtered_characters)
+    except:
+        return ''
 
 def split_based_on_dates(text_list):
     joined_text = ' '.join(text_list)
 
     date_regex = re.compile(
    r'(?<![.\d])(\b\d{2}/\d{2}/\d{4}\b'  # DD/MM/YYYY
     r'|\b\d{2}-[a-zA-Z]{3}-\d{4}\b'  # DD-MMM-YYYY
@@ -403,35 +430,46 @@
         return None
 
 def validate_name(eid_name, extracted_name):
             threshold = 65
             similarity = fuzz.token_sort_ratio(eid_name, extracted_name)
             return similarity >= threshold
 
+def validate_name_both(eid_name, eid_name_ar, extracted_name):
+            threshold = 65
+            similarity1 = fuzz.token_sort_ratio(eid_name, extracted_name)
+            similarity2 = fuzz.token_sort_ratio(eid_name_ar, extracted_name)
+            max_score = max(similarity1, similarity2)
+
+            return max_score >= threshold
+
 def limit_string_to_tokens(data, limit):
     tokens = data.split()  # Split the string into tokens
     limited_tokens = tokens[:limit]  # Select the tokens up to the limit
     limited_data = ' '.join(limited_tokens)  # Join the limited tokens back into a string
     return limited_data
 
 
 def extract_digits_from_gpt_resp(s):
     """
     Extracts digits from a given string and returns the number.
     """
-    salary_pattern = r'Salary:\s*(.*)'
-    s=re.search(salary_pattern,s ).group(1)
-        
-    # Extract digits and decimal points
-    digits = ''.join([char for char in s if char.isdigit() or char == '.'])
+    try:
+        salary_pattern = r'Salary:\s*(.*)'
+        s=re.search(salary_pattern,s ).group(1)
+            
+        # Extract digits and decimal points
+        digits = ''.join([char for char in s if char.isdigit() or char == '.'])
 
-    # Convert the extracted string to a number
-    if digits:
-        return float(digits)
-    else:
+        # Convert the extracted string to a number
+        if digits:
+            return float(digits)
+        else:
+            return 0
+    except:
         return 0
     
 
 def extract_name_from_gpt_resp(text):
     name_pattern = r'Name:\s*(.*)'  # Regex pattern for extracting name
 
     name_match = re.search(name_pattern, text)
@@ -594,15 +632,18 @@
     image_np = np.frombuffer(image_bytes, dtype=np.uint8)
     image_content = cv2.imdecode(image_np, cv2.IMREAD_COLOR)
     _, image_bytes = cv2.imencode('.png', image_content)
 
     image = vision_v1.types.Image(content=image_bytes.tobytes())
     response = client.text_detection(image=image)
     texts = response.text_annotations
-    return texts[0].description
+    try:
+        return texts[0].description
+    except:
+        return ''
 
 def get_scanned_pdf_text(client, doc):
     text = ''
     for page_num in range(doc.page_count):
         page = doc.load_page(page_num)
         # Convert each page to an image
         pix = page.get_pixmap()
@@ -612,30 +653,43 @@
         image_base64 = base64.b64encode(image_bytes.tobytes()).decode('utf-8')
 
         page_text = extract_text_from_image(client, image_base64)
         text += page_text
     
     return text
 
-def perform_data_extraction(client, pdf_bytes):
+def perform_data_extraction(client, pdf_bytes, only_first_page=False):
     try:
-        doc = fitz.open("pdf", pdf_bytes)
+        reader = PyPDF2.PdfReader(pdf_bytes)
+        num_pages = len(reader.pages)
+        print(f"Number of pages (PyPDF2): {num_pages}")
+
         # Extract text from each page
         text = ''
-        for page_num in range(doc.page_count):
-            page = doc.load_page(page_num)
-            text += page.get_text()
+        if only_first_page:
+            # page_num = 0
+            # page = doc.load_page(page_num)
+            # text += page.get_text()
+            page = reader.pages[0]
+            text = page.extract_text()
+        else:
+            for page_num in range(num_pages):
+                text += page_num.extract_text()
+                # page = doc.load_page(page_num)
+                # text += page.get_text()
         
         ## scanned invoice
         if not text:
+            doc = fitz.open("pdf", pdf_bytes)
             text = get_scanned_pdf_text(client, doc)
 
         return text
     
     except Exception as e:
+        doc = fitz.open("pdf", pdf_bytes)
         text = get_scanned_pdf_text(client, doc)
         if text:
             return text
         else:
             return str(e)
 
 def hijri_to_gregorian(hijri_date):
@@ -678,9 +732,20 @@
         
         return english_numeral
 
     except:
         return eastern_numeral
 
 def clean_salary(salary):
+    if not isinstance(salary, str):
+        salary = str(salary)
+
     cleaned_salary = ''.join(char for char in salary if char.isdigit() or char in {',', '.'})
     return cleaned_salary
+
+def convert_sal_string_to_number(input_str):
+    try:
+        numeric_value = float(input_str.replace(',', ''))
+    except ValueError:
+        return
+
+    return numeric_value
```

### Comparing `BsSalary_Extractor-1.3.7/LICENSE` & `bssalary_extractor-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `BsSalary_Extractor-1.3.7/setup.cfg` & `bssalary_extractor-1.3.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = BsSalary_Extractor
-version = 1.3.5
+version = 1.3.8
 author = Fahad Patel
 author_email = fahadpatel1403@gmail.com
 description = This repository contains a Python program designed to execute Optical Character Recognition (OCR) and Facial Recognition on images.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `BsSalary_Extractor-1.3.7/setup.py` & `bssalary_extractor-1.3.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     required = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="BsSalary_Extractor",
-    version="1.3.7",
+    version="1.3.8",
     author="Fahad Patel",
     author_email="fahadpatel1403@gmail.com",
     long_description_content_type="text/markdown",
     url="",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

