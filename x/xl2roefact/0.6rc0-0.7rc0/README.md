# Comparing `tmp/xl2roefact-0.6rc0.tar.gz` & `tmp/xl2roefact-0.7rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xl2roefact-0.6rc0.tar", last modified: Sat Apr 20 01:23:45 2024, max compression
+gzip compressed data, was "xl2roefact-0.7rc0.tar", last modified: Tue Apr 30 04:54:45 2024, max compression
```

## Comparing `xl2roefact-0.6rc0.tar` & `xl2roefact-0.7rc0.tar`

### file list

```diff
@@ -1,27 +1,14 @@
--rw-r--r--   0        0        0    35149 2024-04-20 01:23:19.951218 xl2roefact-0.6rc0/LICENSE
--rw-r--r--   0        0        0    18602 2024-04-20 01:23:19.951218 xl2roefact-0.6rc0/README.md
--rw-r--r--   0        0        0     3364 2024-04-20 01:23:45.699419 xl2roefact-0.6rc0/pyproject.toml
--rw-r--r--   0        0        0        1 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/.gitkeep
--rw-r--r--   0        0        0    21622 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.json
--rw-r--r--   0        0        0   268862 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xlsx
--rw-r--r--   0        0        0    15740 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xml
--rw-r--r--   0        0        0      986 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/_test_results.txt
--rw-r--r--   0        0        0    24084 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/fact_RENF1004.json
--rw-r--r--   0        0        0    16332 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/fact_RENF1004.xlsx
--rw-r--r--   0        0        0     1531 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/tests/todosXML.md
--rw-r--r--   0        0        0      567 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/__init__.py
--rw-r--r--   0        0        0      626 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/__main__.py
--rw-r--r--   0        0        0     1500 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/__version__.py
--rw-r--r--   0        0        0     7913 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/app_cli.py
--rw-r--r--   0        0        0      727 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/chkisld.py
--rw-r--r--   0        0        0      584 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/chkxml.py
--rw-r--r--   0        0        0     8915 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/config_settings.py
--rw-r--r--   0        0        0     1808 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/data/README_app_config_rules.md
--rw-r--r--   0        0        0        1 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/data/__init__.py
--rw-r--r--   0        0        0     7134 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/data/app_settings.yml
--rw-r--r--   0        0        0      600 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/ldxml.py
--rw-r--r--   0        0        0    10480 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/libutils.py
--rw-r--r--   0        0        0    71476 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/rdinv.py
--rw-r--r--   0        0        0     1319 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/sys_settings.py
--rw-r--r--   0        0        0      612 2024-04-20 01:23:20.363222 xl2roefact-0.6rc0/xl2roefact/wrxml.py
--rw-r--r--   0        0        0    61200 1970-01-01 00:00:00.000000 xl2roefact-0.6rc0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 04:54:21.768450 xl2roefact-0.7rc0/LICENSE
+-rw-r--r--   0        0        0    18839 2024-04-30 04:54:21.768450 xl2roefact-0.7rc0/README.md
+-rw-r--r--   0        0        0     3336 2024-04-30 04:54:45.852591 xl2roefact-0.7rc0/pyproject.toml
+-rw-r--r--   0        0        0     1808 2024-04-30 04:54:22.220453 xl2roefact-0.7rc0/src/data/README_app_config_rules.md
+-rw-r--r--   0        0        0        1 2024-04-30 04:54:22.220453 xl2roefact-0.7rc0/src/data/__init__.py
+-rw-r--r--   0        0        0     7134 2024-04-30 04:54:22.220453 xl2roefact-0.7rc0/src/data/app_settings.yml
+-rw-r--r--   0        0        0        1 2024-04-30 04:54:22.220453 xl2roefact-0.7rc0/tests/.gitkeep
+-rw-r--r--   0        0        0    21688 2024-04-30 04:54:22.220453 xl2roefact-0.7rc0/tests/Fact_Petrom_11017969.json
+-rw-r--r--   0        0        0   268862 2024-04-30 04:54:22.224453 xl2roefact-0.7rc0/tests/Fact_Petrom_11017969.xlsx
+-rw-r--r--   0        0        0    15740 2024-04-30 04:54:22.224453 xl2roefact-0.7rc0/tests/Fact_Petrom_11017969.xml
+-rw-r--r--   0        0        0      986 2024-04-30 04:54:22.224453 xl2roefact-0.7rc0/tests/_test_results.txt
+-rw-r--r--   0        0        0    24150 2024-04-30 04:54:22.224453 xl2roefact-0.7rc0/tests/fact_RENF1004.json
+-rw-r--r--   0        0        0    16332 2024-04-30 04:54:22.224453 xl2roefact-0.7rc0/tests/fact_RENF1004.xlsx
+-rw-r--r--   0        0        0    61437 1970-01-01 00:00:00.000000 xl2roefact-0.7rc0/PKG-INFO
```

### Comparing `xl2roefact-0.6rc0/LICENSE` & `xl2roefact-0.7rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6rc0/README.md` & `xl2roefact-0.7rc0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![Static Badge](https://img.shields.io/badge/version-{{ xl2roefact_version }}-blue)
 
 Legaturi externe utile:
 
 * [**Web Site**](https://invoicetoroefact.renware.eu/). (*Pentru acces corect la toate referintele din acest document vizitati site-ul dedicat acestui sistem.*)
 * [Pachet *PyPi*](https://pypi.org/project/xl2roefact/)
 * [Surse *GitHub*](https://github.com/petre-renware/api_to_roefact/)
-* [Vedere de ansamblu pachet biblioteca Python](./doc/README_xl2roefact_library.md)
+* [Referinta *dezvoltare software - biblioteca Python*](https://invoicetoroefact.renware.eu/xl2roefact/doc/README_xl2roefact_library.html)
 * [Referinta *API*](https://invoicetoroefact.renware.eu/xl2roefact/doc/wrapper_810.05a-xl2roefact_DLD_specs.html)
 <!--Refrence to source doc. If used like that, then must be resolved with an external tool before generating a complete README.html doc. The `mkdoxs` is able to do that but in `PyPi` published version will be unusable
 (./doc/810.05a-xl2roefact_DLD_specs.md)
 -->
 
 
 ## Facilitati
@@ -199,15 +199,15 @@
 
 **Comenzile detaliate:**
 
 <a id="comenzile-aplicatiei"></a>  <!-- #NOTE ATTN do not drop this anchor tag because is referred in `mkdocs.yml` navigation section -->
 
 <!--#NOTE: next section generate application commands in same style as obtained using `--help` CLI options -->
 ::: mkdocs-typer
-    :module: xl2roefact.app_cli
+    :module: xl2roefact.src.app_cli
     :command: app_cli
     :prog_name: xl2roefact
     :depth: 2
 
 
 
 
@@ -223,15 +223,15 @@
 >
 >* una este valoarea introdusa intr-o celula (de ex cu 3 zecimale) si
 >* alta este valoarea afisata (cu 2 zecimale) - aceasta din urma trebuie obtinuta prin formatarea celulei respective de a afisa 2 zecimale prin rotunjire insa valoarea efectiva trebuie sa fie cea originala cu 3 zecimale, lucru (diferenta) care se poate vedea la editarea continutului celulei.
 
 
 ### Reguli recomamdate in configurarea aplicatiei pe specificul Excel al facturilor dumneavoastra
 
-{% include './xl2roefact/data/README_app_config_rules.md' %}
+{% include './src/data/README_app_config_rules.md' %}
 
 
 
 
 ## Tutorial utilizare aplicatie
 
 
@@ -307,36 +307,41 @@
 * **`Invoice`** - datele efective ale facturii
 * **`meta_info`**
     * informatii referitoare la procesarea facturii si mapa de conversie a cheii `Invoice` din formatul `JSON` in formatul `XML` cerut de sistemul *RO E-Fact*
     * harta de ajutor in conversia formatului JSON in formatul XML acceptat de sistemul RO E-Fact (cheie `meta_info.map_JSONkeys_XMLtags`) si definititiile XML aferente (cheie `meta_info.invoice_XML_schemes`)
     * alte informatii despre fisierul Excel prelucrat (numele, worksheet cu factura, data si ora procesarii, CRC pentru verificare, etc)
 * **`excel_original_data`** - informatiile originale din fisierul Excel, asa cum au fost ele identificate si gasite precum si locatia (adresele celulelor). Aceste informatii sunt utile in cazul in care exista neclaritati in urma procesuluicde conversie pentru "a intelege" de unde si cum arata informatiile originale din fisierul Excel
 
-<small markdown="1">Pentru detalii suplimentare despre formatul JSON trebyie consultata componenta referitoare la ***[biblioteca `xl2roefact` destinata dezvoltarii software](./doc/README_xl2roefact_library.md)***.</small>
+Detalii suplimentare despre formatul JSON se gasesc in documentaţia *[Referinta dezvoltare software](./doc/README_xl2roefact_library.md)*.
 
 
 
 
 ## Descarcare (download) aplicatie xl2roefact CLI
 
 * [Pachet instalare aplicatie Windows](../doc_src/downloads.md#format-executabil-windows-x64)
 * [Pachet instalare script Python](../doc_src/downloads.md#format-biblioteca-python)
 * [Model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact)
 * [Sablon fisier-date informatii furnizor](../doc_src/downloads.md#sablon-fisier-cu-date-furnizor)
 
 
 
 
+## Referinta dezvoltare software
+
+Documentatia **["Referinta dezvoltare software"](./doc/README_xl2roefact_library.md)** ofera detail necesare pentru utilizarea bibliotecii sursa in dezvoltari specifice, extindere si integrare cu alte sisteme.
+
+
 
 
 ## Date identificare
 
 * part number (p/n): `0000-0095-xl2roefact`
-* producator si copyright: RENWare Software Systems
-* author: Petre Iordanescu (petre.iordanescu@gmail.com)
+* producator si copyright: RENWare Software Systems (referinte detalii tehnice: Petre Iordanescu, *petre.iordanescu@gmail.com*)
+
 
 
 
 ## [License](./LICENSE "download")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xl2roefact-0.6rc0/pyproject.toml` & `xl2roefact-0.7rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -51,40 +51,40 @@
     "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Operating System :: OS Independent",
     "Topic :: Office/Business :: Financial",
 ]
-version = "0.6rc0"
+version = "0.7rc0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://invoicetoroefact.renware.eu"
 PDF-Documentation = "https://invoicetoroefact.renware.eu/pdfs/print_page.html/print_page.pdf"
 PyPi-Package = "https://pypi.org/project/xl2roefact/"
 GitHub = "https://github.com/petre-renware/api_to_roefact"
 
 [project.scripts]
-xl2roefact = "xl2roefact.app_cli:main"
+xl2roefact = "src.app_cli:main"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
 
 [tool.pdm.version]
 source = "file"
-path = "xl2roefact/__version__.py"
+path = "src/__version__.py"
 
 [tool.pdm.build.wheel-data]
 data = [
     { path = "data/*", relative-to = "data/" },
 ]
 
 [tool.pdm.scripts.build_wheel]
@@ -104,18 +104,18 @@
     "--log-level=WARN",
     "--onefile",
     "--noconfirm",
     "xl2roefact_copy_for_sexe.py",
 ]
 
 [tool.pdm.scripts.post_build_sexe]
-call = "xl2roefact.libutils:complete_sexe_file"
+call = "src.libutils:complete_sexe_file"
 
 [tool.pdm.scripts.build_doc]
-shell = "pydoc-markdown -I xl2roefact >doc/810.05a-xl2roefact_DLD_specs.md"
+shell = "pydoc-markdown -I src >doc/810.05a-xl2roefact_DLD_specs.md"
 
 [tool.pdm.scripts.build_all]
 composite = [
     "build_wheel",
     "build_msi",
     "build_sexe",
     "build_doc",
```

### Comparing `xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.json` & `xl2roefact-0.7rc0/tests/Fact_Petrom_11017969.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9735119047619047%*

 * *Differences: {"'Invoice'": "{'cbc_Note': 'generated @2024-04-30T04:18:15.916550+00:00 with xl2roefact by "*

 * *              "RENware Software Systems', 'cbc_InvoiceTypeCode': '380'}",*

 * * "'meta_info'": "{'last_processing_time': '2024-04-30T04:18:15.916180+00:00', "*

 * *                "'map_JSONkeys_XMLtags': {insert: [(54, ['cbc_InvoiceTypeCode', "*

 * *                "'cbc:InvoiceTypeCode'])], delete: [47]}}"}*

```diff
@@ -169,16 +169,17 @@
                 }
             ],
             "cbc_TaxAmount": 8123.66
         },
         "cbc_DocumentCurrencyCode": "RON",
         "cbc_DueDate": "2023-11-16",
         "cbc_ID": "11017969",
+        "cbc_InvoiceTypeCode": "380",
         "cbc_IssueDate": "2023-10-17",
-        "cbc_Note": "proccesed @2024-04-18T04:10:02.798583+00:00 with xl2roefact",
+        "cbc_Note": "generated @2024-04-30T04:18:15.916550+00:00 with xl2roefact by RENware Software Systems",
         "cbc_TaxPointDate": "2023-11-25"
     },
     "excel_original_data": {
         "invoice_footer_area": {
             "end_cell": [
                 49,
                 8
@@ -484,15 +485,15 @@
         "invoice_max_rows": 49,
         "invoice_worksheet": "Factura(Invoice)",
         "items_table_start_cell": [
             29,
             1
         ],
         "items_table_start_marker": "No. crt.",
-        "last_processing_time": "2024-04-18T04:10:02.798215+00:00",
+        "last_processing_time": "2024-04-30T04:18:15.916180+00:00",
         "map_JSONkeys_XMLtags": [
             [
                 "cac_InvoiceLine",
                 "cac:InvoiceLine"
             ],
             [
                 "cac_Item",
@@ -675,18 +676,14 @@
                 "cac:PartyTaxScheme"
             ],
             [
                 "cbc_DueDate",
                 "cbc:DueDate"
             ],
             [
-                "cbc_InvoiceTypeCode",
-                "cbc:InvoiceTypeCode"
-            ],
-            [
                 "cbc_Note",
                 "cbc:Note"
             ],
             [
                 "cbc_TaxPointDate",
                 "cbc:TaxPointDate"
             ],
@@ -705,11 +702,15 @@
             [
                 "cbc_PaymentMeansCode",
                 "cbc:PaymentMeansCode"
             ],
             [
                 "cbc_TaxPointDate",
                 "cbc:TaxPointDate"
+            ],
+            [
+                "cbc_InvoiceTypeCode",
+                "cbc:InvoiceTypeCode"
             ]
         ]
     }
 }
```

### Comparing `xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xlsx` & `xl2roefact-0.7rc0/tests/Fact_Petrom_11017969.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6rc0/tests/Fact_Petrom_11017969.xml` & `xl2roefact-0.7rc0/tests/Fact_Petrom_11017969.xml`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6rc0/tests/_test_results.txt` & `xl2roefact-0.7rc0/tests/_test_results.txt`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6rc0/tests/fact_RENF1004.json` & `xl2roefact-0.7rc0/tests/fact_RENF1004.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9735119047619047%*

 * *Differences: {"'Invoice'": "{'cbc_Note': 'generated @2024-04-30T04:18:15.993391+00:00 with xl2roefact by "*

 * *              "RENware Software Systems', 'cbc_InvoiceTypeCode': '380'}",*

 * * "'meta_info'": "{'last_processing_time': '2024-04-30T04:18:15.992957+00:00', "*

 * *                "'map_JSONkeys_XMLtags': {insert: [(54, ['cbc_InvoiceTypeCode', "*

 * *                "'cbc:InvoiceTypeCode'])], delete: [47]}}"}*

```diff
@@ -196,16 +196,17 @@
                 }
             ],
             "cbc_TaxAmount": 7389.15
         },
         "cbc_DocumentCurrencyCode": "RON",
         "cbc_DueDate": "2023-09-27",
         "cbc_ID": "RENF-1004",
+        "cbc_InvoiceTypeCode": "380",
         "cbc_IssueDate": "2023-08-28",
-        "cbc_Note": "proccesed @2024-04-18T04:10:02.876896+00:00 with xl2roefact",
+        "cbc_Note": "generated @2024-04-30T04:18:15.993391+00:00 with xl2roefact by RENware Software Systems",
         "cbc_TaxPointDate": "2023-09-25"
     },
     "excel_original_data": {
         "invoice_footer_area": {
             "end_cell": [
                 31,
                 9
@@ -559,15 +560,15 @@
         "invoice_max_rows": 31,
         "invoice_worksheet": "FACTURA FINALA",
         "items_table_start_cell": [
             20,
             1
         ],
         "items_table_start_marker": "#",
-        "last_processing_time": "2024-04-18T04:10:02.876450+00:00",
+        "last_processing_time": "2024-04-30T04:18:15.992957+00:00",
         "map_JSONkeys_XMLtags": [
             [
                 "cac_InvoiceLine",
                 "cac:InvoiceLine"
             ],
             [
                 "cac_Item",
@@ -750,18 +751,14 @@
                 "cac:PartyTaxScheme"
             ],
             [
                 "cbc_DueDate",
                 "cbc:DueDate"
             ],
             [
-                "cbc_InvoiceTypeCode",
-                "cbc:InvoiceTypeCode"
-            ],
-            [
                 "cbc_Note",
                 "cbc:Note"
             ],
             [
                 "cbc_TaxPointDate",
                 "cbc:TaxPointDate"
             ],
@@ -780,11 +777,15 @@
             [
                 "cbc_PaymentMeansCode",
                 "cbc:PaymentMeansCode"
             ],
             [
                 "cbc_TaxPointDate",
                 "cbc:TaxPointDate"
+            ],
+            [
+                "cbc_InvoiceTypeCode",
+                "cbc:InvoiceTypeCode"
             ]
         ]
     }
 }
```

### Comparing `xl2roefact-0.6rc0/tests/fact_RENF1004.xlsx` & `xl2roefact-0.7rc0/tests/fact_RENF1004.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6rc0/xl2roefact/config_settings.py` & `xl2roefact-0.7rc0/src/data/app_settings.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,216 +1,182 @@
-"""Configuration and setting parameters.
-
-Regulile recomandate se gasessc in documentul (recommended rules are in document `xl2roefact/data/README_app_config_rules.md`)
-
-Public objects:
-
-* `rules_content`: contains the rules text (rendered)
-
-Info:
-
-* copyright: (c) 2023 RENWare Software Systems
-* author: Petre Iordanescu (petre.iordanescu@gmail.com)
-"""
-
-from pathlib import Path
-import os
-import sys
-from rich.markdown import Markdown
-import yaml
-from pprint import pprint
-from .libutils import hier_get_data_file
-
-"""---------------------------------------------------------------------------------------------------------------------------
-# NOTE: urmatorii parametri sunt utilizati pentru a obtine valori implicite (default) atunci cind nu sunt gasite anumite date / informatii.
-#   Uzual ei sunt folositi de comanda `xl2json` reprezentind functionalitatea de extragere a datelor din Excel si exportul lor in formatul JSON (modulul `rdinv)
----------------------------------------------------------------------------------------------------------------------------"""
-
-# --- coeficientul TVA implicit
-# este utilizat de catre aplicatie in toate conditiile in care nu este gasit unul in fiserul de intrare
-DEFAULT_VAT_PERCENT: float = 0.19
-
-# --- denumirea unui produs ce nu poate fi identificat
-# este utilizat de catre aplicatie in toate conditiile in care denumirea unui produs sau serviciu (liniile facturii) nu este specifcata
-# denumirea este considerta necunoscuta atunci cind este lasata 'blank' sau pur si simplu celula respectiva este goala
-DEFAULT_UNKNOWN_ITEM_NAME: str = "--- n/a ---"
-
-# --- unitatea de masura implicita
-# este utilizat de catre aplicatie in toate conditiile in care unitatea de masura unui produs sau serviciu (liniile facturii) nu este cunoscuta
-# unitatea de masura este considerta necunoscuta atunci cind este lasata 'blank' sau pur si simplu celula respectiva este goala
-DEFAULT_UNKNOWN_UOM: str|None = None
-
-# --- moneda implicita
-# este utilizat de catre aplicatie in toate conditiile in care pe factura nu este specifcata in clar o moneda
-# specifcarea monedei ca sau in titlurile coloanelor nu este luata in considerare (nu este garantat ca este moneda reala a facturii !)
-DEFAULT_CURRENCY: str = "RON"
-
-# --- tara implicita
-# aceste constante sunt utilizate ca si tara implicita pentru "parterii" facturilor in condtiile in care tarile "parterilor" nu sunt gasite
-# in mod explicit pe factura (in zona de adresa). Prin sintagma "partener" pe factura sa intelege oricare din cele doua parti implicate in
-# procesul de facturare, si anume: FURNIZORUL si CLIENTUL
-DEFAULT_CUSTOMER_COUNTRY: str = "RO"
-# ...and the corresponding one for supplier
-DEFAULT_SUPPLIER_COUNTRY: str = "RO"
-
-#--- scadenta implicita
-# scadenta implicita a facturii (in zile calendaristice) daca nu estrecuta in clar pe factura
-DEFAULT_DUE_DATE_DAYS: int = 30
-
-
-"""---------------------------------------------------------------------------------------------------------------------------
-# NOTE: "pattern-uri" (sabloane) de identificare si regasire a datelor folositi de
-#   comanda `xl2json` reprezentind functionalitatea de extragere a datelor din Excel si exportul lor in formatul JSON (modulul `rdinv)
----------------------------------------------------------------------------------------------------------------------------"""
-
-# --- contine secventele de caractere care permit inceputul zonei (sub-tabelului) ce contine liniile facturii
-PATTERN_FOR_INVOICE_ITEMS_SUBTABLE_MARKER: list[str] = [
-    " crt", " crt.",
-    "no. crt.", "no crt", "no. crt", "no crt.",
-    "nr. crt.", "nr crt", "nr. crt", "nr crt.",
-    "#",
-]
-
-# --- numarul facturii
-# acest parametru permit identificarea numarului facturii, astfel sistemul va cauta dupa secventele din parametrul
-# `PATTERN_FOR_INVOICE_NUMBER_LABEL`,... (cautarea fiind indiferenta de marimea caracterelor).
-# Aceasta reprezentind "eticheta" unde se presupune a fi numarul facturii.  Pentru a gasi numarul efectiv al facturii,
-# sistemul va cauta in directiile DREAPTA (UP) si apoi daca nu gaseste JOS (DOWN)
-PATTERN_FOR_INVOICE_NUMBER_LABEL: list[str] = [
-    "nr. fact", "nr fact", "numar fact", "fact nr", "factura num",
-    "invoice number", "invoice no", "invoice:",
-]
-
-# --- moneda facturii
-# pattern utilizat pentru a gasi moneda facturii (daca a fost specificata iar daca nu gaseste se va utiliza DEFAULT_CURRENCY)
-PATTERN_FOR_INVOICE_CURRENCY_LABEL: list[str] = [
-    "mone",
-    "curr", "ccy"
-]
-
-# --- data facturii
-# pattern utilizat pentru a gasi data facturii
-# NOTE-1 in XML formatul utilizat este YYYY-MM-DD
-# NOTE-2 in celula Excel aferenta datei se asteapta ca formatul sa fie cel stadard de data calendaristica (ATENTIE: NU string)
-PATTERN_FOR_INVOICE_ISSUE_DATE_LABEL: list[str] = [
-    "data", "data fact", "data emit",
-    "date", "invoice date", "issue date",
-]
-
-# --- client (customer)
-# pattern utilizat pentru a gasi aria (zona) cu datele furnizorului
-PATTERN_FOR_INVOICE_CUSTOMER_SUBTABLE_MARKER: list[str] = [
-    "clien",
-    "custo",
-    "sc", "s.c", "diviz", "depart",
-    "sa", "s.a",
-    "srl", "s.r.l",
-    "pfa", "p.f.a",
-    "ra", "r.a",
-]
-
-# --- numele legal al companiei
-# pattern utilizat pentru regasirea numelui legal al clientului
-# NOTE se presupune a fi la inceputul zonei cu datele clientului, deci se ca cauta dupa acelasi pattern
-PATTERN_FOR_CUSTOMER_LEGAL_NAME = PATTERN_FOR_INVOICE_CUSTOMER_SUBTABLE_MARKER
-
-# --- pattern pentru regasirea codului unic de inregistrare (sau Company ID in engleza) (pattern comun pentru client si furnizor)
-PATTERN_FOR_PARTNER_ID = [
-    "cui", "c.u.i",
-    "cif", "c.i.f",
-    "id",
-]
-
-# --- pattern pentru regasirea nr de inreg la Registrul Comertului
-PATTERN_FOR_PARTNER_REGCOM = [
-    "reg com", "reg. com", "comert",
-]
-
-# --- pattern-uri pentru regasirea bancii si a contului bancar
-PATTERN_FOR_PARTNER_BANK = [
-    "banc", "bank",
-]
-PATTERN_FOR_PARTNER_IBAN = [
-    "iban", "cont", "bank acc",
-]
-
-# --- pattern pentru regasirea datelor de contact (tel, email)
-PATTERN_FOR_PARTNER_TEL = [
-    "tel", "phon",
-]
-PATTERN_FOR_PARTNER_EMAIL = [
-    "mail", "email", "e-mail",
-]
-
-# --- pattern pentru regasirea adresei (pattern comun pentru client si furnizor)
-# este important ca ordinea de cautare sa permita ca sansele sa fie maximizate pentru cautarea adresei complete sau macar a tarii
-PATTERN_FOR_PARTNER_ADDRESS = [
-    "adr", "addr",
-    "tara", "count",
-    "locali", "oras",
-    "city", "town",
-    "str",
-]
-PATTERN_FOR_PARTNER_ADDRESS_COUNTRY = [
-    "tara", "countr",
-]
-PATTERN_FOR_PARTNER_ADDRESS_CITY = [
-    "judet", "county",
-    "locali",
-    "oras", "city", "town", "land"
-]
-PATTERN_FOR_PARTNER_ADDRESS_STREET = [
-    "str", "sos", "bd", "calea",
-    "ave", "highwa",
-]
-PATTERN_FOR_PARTNER_ADDRESS_ZIPCODE = [
-    "cod pos", "zip cod", "postal",
-]
-
-# --- furnizor (supplier)
-# pattern utilizat pentru a gasi aria (zona) cu datele furnizorului
-PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER: list[str] = [
-    "furniz", "proprie",
-    "suppl", "owne",
-    "sc", "s.c", "diviz", "depart",
-    "sa", "s.a",
-    "srl", "s.r.l",
-    "pfa", "p.f.a",
-    "ra", "r.a",
-]
-
-# --- numele legal al companiei furnizoare
-# pattern utilizat pentru regasirea numelui legal al furnizorului
-# NOTE se presupune a fi la inceputul zonei cu datele furnizorului, deci se ca cauta dupa acelasi pattern
-PATTERN_FOR_SUPPLIER_LEGAL_NAME = PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER
-
-# --- data scadentei
-# pattern utilizat pentru regasirea datei scadentei facturii
-PATTERN_FOR_DUE_DATE = [
-    "scad", "termen plat", "termen de plat"
-    "due da", "date due"
-]
-
-
-
-
-# ------- NOTE: the following code runs unconditionally at module import
-
-# section to read settings from external data file
-file_to_use = hier_get_data_file("app_settings.yml")
-python_object = None  # suppose no settings loaded
-if file_to_use:
-    yaml_in = file_to_use.read_text()
-    python_object = yaml.safe_load(yaml_in)
-    print("***INFO: Application settings loaded from file.")
-# assign `python_object` to locals() environment...
-if python_object is not None:  # ...only if previous method has read something
-    locals().update(python_object)
-else:  # if nothing or wrong read from previous method, settings applied will remain to values hard-coded in this module
-    print("***INFO: Application settings loaded from application code (default settings).")
-
-# prepare `rules_content` public variable to be use as "mini help" by `settings -r` command of application
-rules_content = ""  # initialize with empty string to show nothing in case is a problem with file reading
-rules_file = hier_get_data_file("README_app_config_rules.md")
-rules_content = Markdown(rules_file.read_text())
-
-
+#
+# Fisier de configurare a aplicatiei xl2roefact.
+# 
+# Copyright (c) 2024 RENware Software Systems
+# Author: Petre Iordanescu, petre.iordanescu@gmail.com
+#
+
+
+
+README_rules: "README_app_config_rules.md"
+
+#--------------------------------------------------------------------------------------------------------------------------
+# NOTE: urmatorii parametri sunt utilizati pentru a obtine valori implicite (default) atunci cind nu sunt gasite anumite date / informatii.
+#   Uzual ei sunt folositi de comanda `xl2json` reprezentind functionalitatea de extragere a datelor din Excel si exportul lor in formatul JSON (modulul `rdinv)
+#---------------------------------------------------------------------------------------------------------------------------
+
+# --- coeficientul TVA implicit
+# este utilizat de catre aplicatie in toate conditiile in care nu este gasit unul in fiserul de intrare
+# TIP RECOMANDAT AL INFORMATIEI; numar zecimal
+DEFAULT_VAT_PERCENT: 0.19
+
+# --- denumirea unui produs ce nu poate fi identificat
+# este utilizat de catre aplicatie in toate conditiile in care denumirea unui produs sau serviciu (liniile facturii) nu este specifcata
+# denumirea este considerta necunoscuta atunci cind este lasata 'blank' sau pur si simplu celula respectiva este goala
+DEFAULT_UNKNOWN_ITEM_NAME: "--- n/a ---"
+
+# --- unitatea de masura implicita
+# este utilizat de catre aplicatie in toate conditiile in care unitatea de masura unui produs sau serviciu (liniile facturii) nu este cunoscuta
+# unitatea de masura este considerta necunoscuta atunci cind este lasata 'blank' sau pur si simplu celula respectiva este goala
+DEFAULT_UNKNOWN_UOM: null
+
+# --- moneda implicita
+# este utilizat de catre aplicatie in toate conditiile in care pe factura nu este specifcata in clar o moneda
+# specifcarea monedei ca sau in titlurile coloanelor nu este luata in considerare (nu este garantat ca este moneda reala a facturii !)
+DEFAULT_CURRENCY: "RON"
+
+# --- tara implicita
+# aceste constante sunt utilizate ca si tara implicita pentru "parterii" facturilor in condtiile in care tarile "parterilor" nu sunt gasite
+# in mod explicit pe factura (in zona de adresa). Prin sintagma "partener" pe factura sa intelege oricare din cele doua parti implicate in
+# procesul de facturare, si anume: FURNIZORUL si CLIENTUL
+DEFAULT_CUSTOMER_COUNTRY: "RO"
+DEFAULT_SUPPLIER_COUNTRY: "RO"
+
+#--- scadenta implicita
+# scadenta implicita a facturii (in zile calendaristice) daca nu estrecuta in clar pe factura
+DEFAULT_DUE_DATE_DAYS: 30
+
+
+#---------------------------------------------------------------------------------------------------------------------------
+# NOTE: "pattern-uri" (sabloane) de identificare si regasire a datelor folositi de
+#   comanda `xl2json` reprezentind functionalitatea de extragere a datelor din Excel si exportul lor in formatul JSON (modulul `rdinv)
+#---------------------------------------------------------------------------------------------------------------------------
+
+# --- contine secventele de caractere care permit inceputul zonei (sub-tabelului) ce contine liniile facturii
+PATTERN_FOR_INVOICE_ITEMS_SUBTABLE_MARKER: [
+    " crt", " crt.",
+    "no. crt.", "no crt", "no. crt", "no crt.",
+    "nr. crt.", "nr crt", "nr. crt", "nr crt.",
+    "#",
+]
+
+# --- numarul facturii
+# acest parametru permit identificarea numarului facturii, astfel sistemul va cauta dupa secventele din parametrul
+# `PATTERN_FOR_INVOICE_NUMBER_LABEL`,... (cautarea fiind indiferenta de marimea caracterelor).
+# Aceasta reprezentind "eticheta" unde se presupune a fi numarul facturii.  Pentru a gasi numarul efectiv al facturii,
+# sistemul va cauta in directiile DREAPTA (UP) si apoi daca nu gaseste JOS (DOWN)
+PATTERN_FOR_INVOICE_NUMBER_LABEL: [
+    "nr. fact", "nr fact", "numar fact", "fact nr", "factura num",
+    "invoice number", "invoice no", "invoice:",
+]
+
+# --- moneda facturii
+# pattern utilizat pentru a gasi moneda facturii (daca a fost specificata iar daca nu gaseste se va utiliza DEFAULT_CURRENCY)
+PATTERN_FOR_INVOICE_CURRENCY_LABEL: [
+    "mone",
+    "curr", "ccy"
+]
+
+# --- data facturii
+# pattern utilizat pentru a gasi data facturii
+# NOTE-1 in XML formatul utilizat este YYYY-MM-DD
+# NOTE-2 in celula Excel aferenta datei se asteapta ca formatul sa fie cel stadard de data calendaristica (ATENTIE: NU string)
+PATTERN_FOR_INVOICE_ISSUE_DATE_LABEL: [
+    "data", "data fact", "data emit",
+    "date", "invoice date", "issue date",
+]
+
+# --- client (customer)
+# pattern utilizat pentru a gasi aria (zona) cu datele clientului
+PATTERN_FOR_INVOICE_CUSTOMER_SUBTABLE_MARKER: &patt_cust_marker [
+    "clien",
+    "custo",
+    "sc", "s.c", "diviz", "depart",
+    "sa", "s.a",
+    "srl", "s.r.l",
+    "pfa", "p.f.a",
+    "ra", "r.a",
+]
+
+# --- numele legal al companiei
+# pattern utilizat pentru regasirea numelui legal al clientului
+# NOTE se presupune a fi la inceputul zonei cu datele furnizorului, deci se ca cauta dupa acelasi pattern
+PATTERN_FOR_CUSTOMER_LEGAL_NAME: *patt_cust_marker
+
+# --- pattern pentru regasirea codului unic de inregistrare (sau Company ID in engleza) (pattern comun pentru client si furnizor)
+PATTERN_FOR_PARTNER_ID: [
+    "cui", "c.u.i",
+    "cif", "c.i.f",
+    "id",
+]
+
+# --- pattern pentru regasirea nr de inreg la Registrul Comertului
+PATTERN_FOR_PARTNER_REGCOM: [
+    "reg com", "reg. com", "comert",
+]
+
+# --- pattern-uri pentru regasirea bancii si a contului bancar
+PATTERN_FOR_PARTNER_BANK: [
+    "banc", "bank",
+]
+PATTERN_FOR_PARTNER_IBAN: [
+    "iban", "cont", "bank acc",
+]
+
+# --- pattern pentru regasirea datelor de contact (tel, email)
+PATTERN_FOR_PARTNER_TEL: [
+    "tel", "phon",
+]
+PATTERN_FOR_PARTNER_EMAIL: [
+    "mail", "email", "e-mail",
+]
+
+# --- pattern pentru regasirea adresei (pattern comun pentru client si furnizor)
+# este important ca ordinea de cautare sa permita ca sansele sa fie maximizate pentru cautarea adresei complete sau macar a tarii
+PATTERN_FOR_PARTNER_ADDRESS: [
+    "adr", "addr",
+    "tara", "count",
+    "locali", "oras",
+    "city", "town",
+    "str",
+]
+PATTERN_FOR_PARTNER_ADDRESS_COUNTRY: [
+    "tara", "countr",
+]
+PATTERN_FOR_PARTNER_ADDRESS_CITY: [
+    "judet", "county",
+    "locali",
+    "oras", "city", "town", "land"
+]
+PATTERN_FOR_PARTNER_ADDRESS_STREET: [
+    "str", "sos", "bd", "calea",
+    "ave", "highwa",
+]
+PATTERN_FOR_PARTNER_ADDRESS_ZIPCODE: [
+    "cod pos", "zip cod", "postal",
+]
+
+# --- furnizor (supplier)
+# pattern utilizat pentru a gasi aria (zona) cu datele furnizorului
+PATTERN_FOR_INVOICE_SUPPLIER_SUBTABLE_MARKER: &patt_suppl_marker [
+    "furniz", "proprie",
+    "suppl", "owne",
+    "sc", "s.c", "diviz", "depart",
+    "sa", "s.a",
+    "srl", "s.r.l",
+    "pfa", "p.f.a",
+    "ra", "r.a",
+]
+
+# --- numele legal al companiei furnizoare
+# pattern utilizat pentru regasirea numelui legal al furnizorului
+# NOTE se presupune a fi la inceputul zonei cu datele furnizorului, deci se ca cauta dupa acelasi pattern
+PATTERN_FOR_SUPPLIER_LEGAL_NAME: *patt_suppl_marker
+
+# --- data scadentei
+# pattern utilizat pentru regasirea datei scadentei facturii
+PATTERN_FOR_DUE_DATE: [
+    "scad", "termen plat", "termen de plat",
+    "due da", "date due",
+]
+
+
```

### Comparing `xl2roefact-0.6rc0/xl2roefact/data/README_app_config_rules.md` & `xl2roefact-0.7rc0/src/data/README_app_config_rules.md`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.6rc0/PKG-INFO` & `xl2roefact-0.7rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl2roefact
-Version: 0.6rc0
+Version: 0.7rc0
 Summary: Excel invoices data retrieve, export & upload to RO E-Fact system
 Author-Email: Petre Iordanescu <petre.iordanescu@gmail.com>, RENware Software Systems <renware.systems@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -734,15 +734,15 @@
 ![Static Badge](https://img.shields.io/badge/version-{{ xl2roefact_version }}-blue)
 
 Legaturi externe utile:
 
 * [**Web Site**](https://invoicetoroefact.renware.eu/). (*Pentru acces corect la toate referintele din acest document vizitati site-ul dedicat acestui sistem.*)
 * [Pachet *PyPi*](https://pypi.org/project/xl2roefact/)
 * [Surse *GitHub*](https://github.com/petre-renware/api_to_roefact/)
-* [Vedere de ansamblu pachet biblioteca Python](./doc/README_xl2roefact_library.md)
+* [Referinta *dezvoltare software - biblioteca Python*](https://invoicetoroefact.renware.eu/xl2roefact/doc/README_xl2roefact_library.html)
 * [Referinta *API*](https://invoicetoroefact.renware.eu/xl2roefact/doc/wrapper_810.05a-xl2roefact_DLD_specs.html)
 <!--Refrence to source doc. If used like that, then must be resolved with an external tool before generating a complete README.html doc. The `mkdoxs` is able to do that but in `PyPi` published version will be unusable
 (./doc/810.05a-xl2roefact_DLD_specs.md)
 -->
 
 
 ## Facilitati
@@ -928,15 +928,15 @@
 
 **Comenzile detaliate:**
 
 <a id="comenzile-aplicatiei"></a>  <!-- #NOTE ATTN do not drop this anchor tag because is referred in `mkdocs.yml` navigation section -->
 
 <!--#NOTE: next section generate application commands in same style as obtained using `--help` CLI options -->
 ::: mkdocs-typer
-    :module: xl2roefact.app_cli
+    :module: xl2roefact.src.app_cli
     :command: app_cli
     :prog_name: xl2roefact
     :depth: 2
 
 
 
 
@@ -952,15 +952,15 @@
 >
 >* una este valoarea introdusa intr-o celula (de ex cu 3 zecimale) si
 >* alta este valoarea afisata (cu 2 zecimale) - aceasta din urma trebuie obtinuta prin formatarea celulei respective de a afisa 2 zecimale prin rotunjire insa valoarea efectiva trebuie sa fie cea originala cu 3 zecimale, lucru (diferenta) care se poate vedea la editarea continutului celulei.
 
 
 ### Reguli recomamdate in configurarea aplicatiei pe specificul Excel al facturilor dumneavoastra
 
-{% include './xl2roefact/data/README_app_config_rules.md' %}
+{% include './src/data/README_app_config_rules.md' %}
 
 
 
 
 ## Tutorial utilizare aplicatie
 
 
@@ -1036,36 +1036,41 @@
 * **`Invoice`** - datele efective ale facturii
 * **`meta_info`**
     * informatii referitoare la procesarea facturii si mapa de conversie a cheii `Invoice` din formatul `JSON` in formatul `XML` cerut de sistemul *RO E-Fact*
     * harta de ajutor in conversia formatului JSON in formatul XML acceptat de sistemul RO E-Fact (cheie `meta_info.map_JSONkeys_XMLtags`) si definititiile XML aferente (cheie `meta_info.invoice_XML_schemes`)
     * alte informatii despre fisierul Excel prelucrat (numele, worksheet cu factura, data si ora procesarii, CRC pentru verificare, etc)
 * **`excel_original_data`** - informatiile originale din fisierul Excel, asa cum au fost ele identificate si gasite precum si locatia (adresele celulelor). Aceste informatii sunt utile in cazul in care exista neclaritati in urma procesuluicde conversie pentru "a intelege" de unde si cum arata informatiile originale din fisierul Excel
 
-<small markdown="1">Pentru detalii suplimentare despre formatul JSON trebyie consultata componenta referitoare la ***[biblioteca `xl2roefact` destinata dezvoltarii software](./doc/README_xl2roefact_library.md)***.</small>
+Detalii suplimentare despre formatul JSON se gasesc in documentaţia *[Referinta dezvoltare software](./doc/README_xl2roefact_library.md)*.
 
 
 
 
 ## Descarcare (download) aplicatie xl2roefact CLI
 
 * [Pachet instalare aplicatie Windows](../doc_src/downloads.md#format-executabil-windows-x64)
 * [Pachet instalare script Python](../doc_src/downloads.md#format-biblioteca-python)
 * [Model de sablon de configuare](../doc_src/downloads.md#sablon-fisier-configurare-a-aplicatiei-xl2roefact)
 * [Sablon fisier-date informatii furnizor](../doc_src/downloads.md#sablon-fisier-cu-date-furnizor)
 
 
 
 
+## Referinta dezvoltare software
+
+Documentatia **["Referinta dezvoltare software"](./doc/README_xl2roefact_library.md)** ofera detail necesare pentru utilizarea bibliotecii sursa in dezvoltari specifice, extindere si integrare cu alte sisteme.
+
+
 
 
 ## Date identificare
 
 * part number (p/n): `0000-0095-xl2roefact`
-* producator si copyright: RENWare Software Systems
-* author: Petre Iordanescu (petre.iordanescu@gmail.com)
+* producator si copyright: RENWare Software Systems (referinte detalii tehnice: Petre Iordanescu, *petre.iordanescu@gmail.com*)
+
 
 
 
 ## [License](./LICENSE "download")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

