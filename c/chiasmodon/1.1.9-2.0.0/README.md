# Comparing `tmp/chiasmodon-1.1.9.tar.gz` & `tmp/chiasmodon-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-1.1.9.tar", last modified: Thu Apr 18 23:54:08 2024, max compression
+gzip compressed data, was "chiasmodon-2.0.0.tar", last modified: Tue Apr 30 19:18:25 2024, max compression
```

## Comparing `chiasmodon-1.1.9.tar` & `chiasmodon-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 23:54:08.209658 chiasmodon-1.1.9/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.9/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    14419 2024-04-18 23:54:08.209658 chiasmodon-1.1.9/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13873 2024-04-18 03:14:25.000000 chiasmodon-1.1.9/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 23:54:08.209658 chiasmodon-1.1.9/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    14419 2024-04-18 23:54:08.000000 chiasmodon-1.1.9/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-18 23:54:08.000000 chiasmodon-1.1.9/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 23:54:08.000000 chiasmodon-1.1.9/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-18 23:54:08.000000 chiasmodon-1.1.9/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 23:54:08.000000 chiasmodon-1.1.9/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 23:54:08.209658 chiasmodon-1.1.9/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21181 2024-04-18 23:43:55.000000 chiasmodon-1.1.9/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    18945 2024-04-18 23:53:55.000000 chiasmodon-1.1.9/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-18 23:54:08.209658 chiasmodon-1.1.9/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-18 23:53:53.000000 chiasmodon-1.1.9/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-30 19:18:25.213553 chiasmodon-2.0.0/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-2.0.0/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-04-30 19:18:25.213553 chiasmodon-2.0.0/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11584 2024-04-30 19:12:19.000000 chiasmodon-2.0.0/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-30 19:18:25.213553 chiasmodon-2.0.0/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    12235 2024-04-30 19:18:25.000000 chiasmodon-2.0.0/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-30 19:18:25.000000 chiasmodon-2.0.0/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-30 19:18:25.000000 chiasmodon-2.0.0/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       39 2024-04-30 19:18:25.000000 chiasmodon-2.0.0/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-30 19:18:25.000000 chiasmodon-2.0.0/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-30 19:18:25.213553 chiasmodon-2.0.0/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21965 2024-04-30 19:16:31.000000 chiasmodon-2.0.0/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    28120 2024-04-30 19:15:47.000000 chiasmodon-2.0.0/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-30 19:18:25.213553 chiasmodon-2.0.0/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1262 2024-04-30 19:17:08.000000 chiasmodon-2.0.0/setup.py
```

### Comparing `chiasmodon-1.1.9/LICENSE.txt` & `chiasmodon-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.9/cli/chiasmodon_cli.py` & `chiasmodon-2.0.0/cli/chiasmodon_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/python3
+# PYTHON_ARGCOMPLETE_OK
 
 import os
 import sys
+import argcomplete
 import json
 import argparse
 import tldextract
 from yaspin import yaspin
 from pathlib import Path 
-from pychiasmodon import Chiasmodon,Result,VERSION,VIEW_TYPE_LIST,T
+from pychiasmodon import Chiasmodon,Result,VERSION,VIEW_TYPE_LIST,T,_METHODS
 
 ROOT_DIR = os.path.dirname(os.path.abspath(__file__))
 
 class ULIT:
     @staticmethod
     def rFile(file:Path) -> str:
         if not file.is_file():
@@ -47,15 +49,15 @@
         return '{}.{}'.format(x.domain, x.suffix)
 
 class Scan(Chiasmodon):
     def __init__(self, options:argparse.Namespace) -> None:        
         self.options :argparse.Namespace=options
         self.result :list = []
         conf_file :Path = Path(ROOT_DIR, 'conf.json')
-        token:str = '' 
+        token:str = ''
         
         if not conf_file.is_file():ULIT.wJsonToFile(conf_file, {})
 
         if self.options.init:
             token = self.options.init
             ULIT.wJsonToFile(conf_file, {'token':self.options.init})
 
@@ -64,118 +66,177 @@
             token = ''
 
         else:
             token = ULIT.rFileToJson(conf_file).get('token') or ''
 
         super().__init__(
             token=token,
-            color=True,
-            #debug=self.options.debug, 
+            conf_file=conf_file,
+            color=True if not self.options.no_color else False,
             debug=True, 
             check_token=self.options.init,
         )
 
         if self.options.init:
             sys.exit()
         
         self.scan_mode = True
 
     def scan_callback(self,beta,ys):
         self.print(beta.print(), ys)
 
     def proc(self):
-        if not self.options.domain:
+        if not self.options.query:
             self.print(f"{T.RED}You can't run scan without company domain\nPlease use (-d or --domain) to scan the domain{T.RESET}")
             sys.exit(0)
         
-        domain = ULIT.get_root_domain(self.options.domain)
+        domain = ULIT.get_root_domain(self.options.query)
         if not domain:
             self.print(f"{T.RED}Wrong domain{T.RESET}",)
             sys.exit(0)
 
         self.output_folder = Path(domain)
         self.output_folder.mkdir(exist_ok=True, parents=True)
 
         self.__scan(
             domain=domain,
         )
 
 
     def __scan(self, domain):
         print_output = f'{T.MAGENTA}>{T.RESET}{T.YELLOW} Saved output{T.RESET}: \n'
-
         output = {
             'related':[],
+            'apps':[], 
             'client-creds':[],
             'client-usernames':[],
             'client-passwords':[],
             'client-emails':[],
             'employe-creds':[],
             'employe-usernames':[],
             'employe-passwords':[],
             'employe-emails':[],
             'subdomains':[],
             'urls':[],
             'endpoints':[],
             'ports':[],
-            # 'company-apps':[], # "soon"
-            # 'company-asns':[], # "soon"
 
         }
         
-        self.print(f"\nFind related companies for {T.GREEN+domain+T.RESET}",ys=False)
-        related = self.search(
-            method='domain',
-            query=domain,
-            country=self.options.country,
-            view_type='subdomain',
-            sort=True ,
-            timeout=self.options.timeout,
-            only_domain_emails=False,
-            all=False,
-            limit=1000000,
-            callback_view_result=self.scan_callback,
-            yaspin=yaspin,
-            related=True,
-        )
+        if self.options.scan_related.lower() == 'yes':
+            related = self.search(
+                method='domain',
+                query=domain,
+                view_type='related',
+                sort=True ,
+                timeout=self.options.timeout,
+                limit=1000000,
+                callback_view_result=self.scan_callback,
+                yaspin=yaspin,
+                search_text=f'Find {T.GREEN+domain+T.RESET} related companies...',
+                err_text=f'Not found related !'
+            )
 
-        output['related'] = [i.save_format() for i in related]
 
-        if related:
-            ULIT.wFile((self.output_folder / 'related.txt'), '\n'.join(output['related'])) 
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'related.txt')}{T.RESET}\n"
+            if related:
+                output['related'] = [i.save_format() for i in related]
+                ULIT.wFile((self.output_folder / 'related.txt'), '\n'.join(output['related'])) 
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'related.txt')}{T.RESET}\n"
+            else:
+                self.print(f'{T.RED}💥 Not found related !{T.RESET}')
+            self.print(f'{T.MAGENTA}{"-"*30}{T.RESET}')
+        if self.options.scan_subdomains.lower() == 'yes':
+            subdomains = self.search(
+                method='domain',
+                query=domain,
+                view_type='subdomain',
+                sort=True ,
+                timeout=self.options.timeout,
+                limit=1000000,
+                callback_view_result=self.scan_callback,
+                yaspin=yaspin,
+                search_text=f'Find {T.GREEN+domain+T.RESET} subdomains...',
+                err_text=f'Not found subdomains !'
+            )
 
+
+            if subdomains:
+                output['subdomains'] = [i.save_format() for i in subdomains]
+                ULIT.wFile((self.output_folder / 'subdomains.txt'), '\n'.join(output['subdomains'])) 
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'subdomains.txt')}{T.RESET}\n"
+            self.print(f'{T.MAGENTA}{"-"*30}{T.RESET}')
+            
+        if self.options.scan_apps.lower() == 'yes':
+            apps = self.search(
+                method='app.domain',
+                query=domain,
+                view_type='app',
+                sort=True ,
+                timeout=self.options.timeout,
+                limit=1000000,
+                callback_view_result=self.scan_callback,
+                yaspin=yaspin,
+                search_text=f'Find {T.GREEN+domain+T.RESET} Apps...',
+                err_text=f'Not found apps !'
+            )
+
+
+            if apps:
+                output['apps'] = [i.save_format() for i in apps]
+                ULIT.wFile((self.output_folder / 'apps.txt'), '\n'.join(output['apps'])) 
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'apps.txt')}{T.RESET}\n"
+            self.print(f'{T.MAGENTA}{"-"*30}{T.RESET}')
+        if self.options.scan_ips.lower() == 'yes':
+            ips = self.search(
+                method='domain.all',
+                query=domain,
+                view_type='ip',
+                sort=True ,
+                timeout=self.options.timeout,
+                limit=1000000,
+                callback_view_result=self.scan_callback,
+                yaspin=yaspin,
+                search_text=f'Find {T.GREEN+domain+T.RESET} IPs...',
+                err_text=f'Not found ips !'
+            )
+
+
+            if ips:
+                output['ips'] = [i.save_format() for i in ips]
+                ULIT.wFile((self.output_folder / 'ips.txt'), '\n'.join(output['ips'])) 
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'ips.txt')}{T.RESET}\n"
+                
+            self.print(f'{T.MAGENTA}{"-"*30}{T.RESET}')
         if self.options.scan_clients.lower() == 'yes':
-            self.print(f"\nFind client creds in {T.GREEN+'*.'+domain+T.RESET}")
             client_creds:list[Result] = self.search(
-                method='domain',
                 query=domain,
-                country=self.options.country,
+                method='domain.all',
                 view_type='cred',
                 sort=True ,
                 timeout=self.options.timeout,
-                only_domain_emails=False,
-                all=True,
                 limit=1000000,
                 callback_view_result=self.scan_callback,
-                yaspin=yaspin
+                yaspin=yaspin,
+                search_text=f'Find {T.GREEN+domain+T.RESET} client creds...',
+                err_text=f'Not found clients !'
+                
             )
-            output['client-creds'] =[i.save_format() for i in client_creds]
         
             if client_creds:
+                output['client-creds'] =[i.save_format() for i in client_creds]
                 ULIT.wFile((self.output_folder / 'client-creds.txt'), '\n'.join([':'.join(i) for i in output['client-creds']]))
                 print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'client-creds.txt')}{T.RESET}\n"
                 
                 for i in client_creds:
-                    output['client-usernames'].append(i.username) if i.username and not i.email  and '/' not in i.username and  i.username not in output['client-usernames']  else None
-                    output['client-passwords'].append(i.password) if i.password and i.password not in output['client-passwords'] else None
-                    output['client-emails'].append(i.email) if i.email  and i.email not in output['client-emails'] else None
+                    output['client-usernames'].append(i.credUsername) if i.credUsername and not i.credEmail  and '/' not in i.credUsername and  i.credUsername not in output['client-usernames']  else None
+                    output['client-passwords'].append(i.credPassword) if i.credPassword and i.credPassword not in output['client-passwords'] else None
+                    output['client-emails'].append(i.credEmail) if i.credEmail  and i.credEmail not in output['client-emails'] else None
                     output['subdomains'].append(i.domain) if i.domain and i.domain not in output['subdomains'] and i.domain != domain else None
                     output['urls'].append(i.url) if i.url and i.url not in output['urls'] else None
-                    output['endpoints'].append(i.urlEndpoint) if i.urlEndpoint and i.urlEndpoint not in output['endpoints'] else None
+                    output['endpoints'].append(i.urlPath) if i.urlPath and i.urlPath not in output['endpoints'] else None
                     output['ports'].append(i.urlPort) if i.urlPort and i.urlPort not in output['ports'] else None
                     
                 ULIT.wFile((self.output_folder / 'client-usernames.txt'), '\n'.join(output['client-usernames']))
                 print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'client-usernames.txt')}{T.RESET}\n"
                 ULIT.wFile((self.output_folder / 'client-emails.txt'), '\n'.join(output['client-emails']))
                 print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'client-emails.txt')}{T.RESET}\n"
                 ULIT.wFile((self.output_folder / 'client-passwords.txt'), '\n'.join(output['client-passwords']))
@@ -186,38 +247,36 @@
                 print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'ports.txt')}{T.RESET}\n"
                 ULIT.wFile((self.output_folder / 'subdomains.txt'), '\n'.join(output['subdomains']))
                 print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'subdomains.txt')}{T.RESET}\n"
                 ULIT.wFile((self.output_folder / 'urls.txt'), '\n'.join([f"{i}" for i in output['urls']]))
                 print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'urls.txt')}{T.RESET}\n"
 
 
+            self.print(f'{T.MAGENTA}{"-"*30}{T.RESET}')
         if self.options.scan_employees.lower() == 'yes':
-            self.print(f"\nFind employees creds for {T.GREEN+domain+T.RESET}")
             employe_creds = self.search(
-                method='domain',
                 query=domain,
-                country=self.options.country,
+                method='cred.email.domain',
                 view_type='cred',
-                sort=True ,
+                sort=True,
                 timeout=self.options.timeout,
-                only_domain_emails=True,
-                all=False,
                 limit=1000000,
-                callback_view_result=self.scan_callback,
-                yaspin=yaspin
+                yaspin=yaspin,
+                search_text=f'Find {T.GREEN+domain+T.RESET} employees creds...',
+                err_text=f'Not found Employees!'
             )
-            output['employe-creds'] =[i.save_format() for i in employe_creds]
 
             if employe_creds:
+                output['employe-creds'] =[i.save_format() for i in employe_creds]
                 ULIT.wFile((self.output_folder / 'employe-creds.txt'), '\n'.join([':'.join(i) for i in output['employe-creds']]))
                 print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-creds.txt')}{T.RESET}\n"
                 for i in employe_creds:
-                    output['employe-usernames'].append(i.username) if i.username and not i.email and '/' not in i.username and i.username not in output['employe-usernames']  else None
-                    output['employe-passwords'].append(i.password) if i.password and i.password not in output['employe-passwords'] else None
-                    output['employe-emails'].append(i.email) if i.email  and i.email not in output['employe-emails'] else None
+                    output['employe-usernames'].append(i.credUsername) if i.credUsername and not i.credEmail and '/' not in i.credUsername and i.credUsername not in output['employe-usernames']  else None
+                    output['employe-passwords'].append(i.credPassword) if i.credPassword and i.credPassword not in output['employe-passwords'] else None
+                    output['employe-emails'].append(i.credEmail) if i.credEmail  and i.credEmail not in output['employe-emails'] else None
                     
                 ULIT.wFile((self.output_folder / 'employe-usernames.txt'), '\n'.join(output['employe-usernames']))
                 print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-usernames.txt')}{T.RESET}\n"
                 ULIT.wFile((self.output_folder / 'employe-emails.txt'), '\n'.join(output['employe-emails']))
                 print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-emails.txt')}{T.RESET}\n"
                 ULIT.wFile((self.output_folder / 'employe-passwords.txt'), '\n'.join(output['employe-passwords']))
                 print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-passwords.txt')}{T.RESET}\n"
@@ -247,31 +306,33 @@
             token = ''
 
         else:
             token = ULIT.rFileToJson(conf_file).get('token') or ''
 
         super().__init__(
             token=token,
-            color=True,
+            conf_file=conf_file,
+            color=True if not self.options.no_color else False,
             #debug=self.options.debug, 
             debug=True, 
             check_token=self.options.init,
         )
 
         if self.options.init:
             sys.exit()
 
     def review_results(self,
                        beta:Result, 
                        ys=True,
                     ) -> None:
 
-        self.print(beta.print(), ys=ys)
-        self.result.append(beta.save_format())
-    
+        if beta.save_format() not in self.result:
+            self.print(beta.print(), ys=ys)
+            self.result.append(beta.save_format())
+        
     def save_result(self, view_type) -> None:
 
         if self.options.output:
 
             if self.options.output_type == "text":
                 if self.result and view_type != 'cred':
                     self.result = list(set(self.result))
@@ -298,70 +359,38 @@
                     self.result
                 )
 
 
 
     def proc(self):
 
-        if self.options.email:
-            query = ULIT.rFile(f).splitlines() if (f:=Path(self.options.email)).is_file() else [self.options.email.strip().lower()]
-            method = 'email'
-
-        if self.options.domain:
-            query = ULIT.rFile(f).splitlines() if (f:=Path(self.options.domain)).is_file() else [self.options.domain.strip().lower()]
-            method = 'domain'
-
-        if self.options.asn:
-            query = ULIT.rFile(f).splitlines() if (f:=Path(self.options.asn)).is_file() else [self.options.asn.strip().lower()]
-            method = 'asn'
-
-        if self.options.cidr:
-            query = ULIT.rFile(f).splitlines() if (f:=Path(self.options.cidr)).is_file() else [self.options.cidr.strip()]
-            method = 'cidr'
-      
-        if self.options.app:
-            query = ULIT.rFile(f).splitlines() if (f:=Path(self.options.app)).is_file() else [self.options.app.strip().lower()]
-            method='app'
-
-        if self.options.username:
-            query = ULIT.rFile(f).splitlines() if (f:=Path(self.options.username)).is_file() else [self.options.username.strip()]
-            method ='username'
-
-        if self.options.password:
-            query = ULIT.rFile(f).splitlines() if (f:=Path(self.options.password)).is_file() else [self.options.password.strip()]
-            method = 'password'
-
-        if self.options.endpoint:
-            query = ULIT.rFile(f).splitlines() if (f:=Path(self.options.endpoint)).is_file() else [self.options.endpoint.strip()]
-            method = 'endpoint'
-        
+        query = ULIT.rFile(f).splitlines() if (f:=Path(self.options.query)).is_file() else [self.options.query.strip()] 
+
+
         for i in query:
             self.search(
                 query=i,
-                method=method,
-                country=self.options.country,
+                method=self.options.method,
                 view_type=self.options.view_type,
                 limit=self.options.limit,
-                all=self.options.all,
-                only_domain_emails=self.options.domain_emails,
                 timeout=self.options.timeout,
                 sort=True,
-                callback_view_result=self.review_results,
-                related=self.options.related,
                 yaspin=yaspin,
+                callback_view_result=self.review_results,
             )
 
         if self.options.output and self.result:
             self.save_result(self.options.view_type)
             self.print(f'{T.MAGENTA}>{T.RESET}{T.YELLOW} Saved output to {T.RESET}: {T.GREEN}{self.options.output}{T.RESET}')
 
       
 if __name__ == "__main__":
 
-    print(f"""
+    if len(sys.argv) == 1 or '--help' in sys.argv or '-h' in sys.argv:
+        print(f"""
    🙂           🙂                 
   /|\\           /|\\               
   /\\            /\\                                                                                   
  \\___/        \\___/                 🔑
 {T.BLUE}~^~^~^~^~^~^~^~^~^~^~^~^~{T.BLUE}~^~^~^~{T.GREEN}    {T.RESET}/|\\{T.GREEN}
 |\\   {T.YELLOW}\\\\\\\\{T.GREEN}__     {T.MAGENTA}Chiasmodon{T.RESET} {T.RED}{VERSION}{T.GREEN}    {T.RESET}/\\{T.GREEN}
 | \\_/    {T.RED}o{T.GREEN} \\    {T.CYAN}o{T.GREEN}                  {T.RESET}\\___/{T.GREEN}
@@ -369,99 +398,109 @@
 | / \\__+___/        
 |/     |/           
 
 {T.MAGENTA}>{T.RESET} {T.YELLOW}Admin{T.RESET}: {T.GREEN}https://t.me/Chiasmod0n
 {T.RESET}""")
     parser = argparse.ArgumentParser(description='Chiasmodon CLI',  formatter_class=argparse.RawTextHelpFormatter,)
 
-    parser.add_argument('-d','--domain',        help='Search by domain.',type=str)
-    parser.add_argument('-a','--app',           help='Search by google play applciton id.',type=str)
-    parser.add_argument('-c','--cidr',          help='Search by CIDR.',type=str)
-    parser.add_argument('-n','--asn',          help='Search by ASN.',type=str)
-    parser.add_argument('-e','--email',         help='Search by email, only pro, only pro account.',type=str)
-    parser.add_argument('-u','--username',      help='Search by username, only pro account.',type=str)
-    parser.add_argument('-p','--password',      help='Search by password, only pro account.',type=str)
-    parser.add_argument('-ep','--endpoint',     help='Search by url endpoint.',type=str)    
-    parser.add_argument('-s','--scan',          help='scan the company domain (Related company, Clients, Employees, Company ASNs, Company Apps).',action='store_true', default=False)
+    if '-lm' not in sys.argv and '--list-methods' not in sys.argv and '-lv' not in sys.argv and '--list-view-type' not in sys.argv and '-v' not in sys.argv and '--version' not in sys.argv and '--init' not in sys.argv:
+        parser.add_argument('query', type=str,      help='query argument')
+
+    parser.add_argument('-m','--method',        help='method to search by it,default is "domain".', choices=_METHODS, type=str, default='domain')
+    parser.add_argument('-vt','--view-type',    help='type view the result default is "full".', choices=VIEW_TYPE_LIST, type=str, default='full')
+    parser.add_argument('-s','--scan',          help='scan the company domain (Related company, Clients, Employees, Company ASNs, Company Apps).',action='store_true')
+    parser.add_argument('-sr','--scan-related', help='Run related scan, default is yes, Ex: -sr no',type=str, default='yes')
+    parser.add_argument('-ss','--scan-subdomains', help='Run subdomains scan, default is yes, Ex: -ss no',type=str, default='yes')
+    parser.add_argument('-sa','--scan-apps',    help='Run App scan, default is yes, Ex: -sa no',type=str, default='yes')
+    parser.add_argument('-si','--scan-ips',     help='Run IPs scan, default is yes, Ex: -si no',type=str, default='yes')
     parser.add_argument('-sc','--scan-clients', help='Run clients scan, default is yes, Ex: -sc no',type=str, default='yes')
     parser.add_argument('-se','--scan-employees',help='Run employees scan, default is yes, Ex: -se no',type=str, default='yes')
-    #parser.add_argument('-fs','--full-scan',    help='',action='store_true', default=False) # "soon" 
-    parser.add_argument('-C','--country',       help='sort result by country code default is all', type=str, default='all')
-    parser.add_argument('-A','--all',           help='view all result using "like",this option work only with (-d or --domain),default is False', action='store_true', default=False)
-    parser.add_argument('-de','--domain-emails',help='only result for company "root" domain, this option work only with (-d or --domain), default is False',action='store_true', default=False)
-    parser.add_argument('-r','--related',       help='Get related company domains,this option work only with (-d or --domain), default False',action='store_true', default=False)
     parser.add_argument('-o','--output',        help='filename to save the result', type=str,)
-    parser.add_argument('-vt','--view-type',    help='type view the result default is "cred".', choices=VIEW_TYPE_LIST, type=str, default='cred')
     parser.add_argument('-ot','--output-type',  help='output format default is "text".', choices=['text', 'json', 'csv'], type=str, default='text')
+    parser.add_argument('-t','--timeout',       help='request timeout default is 360 sec.',type=int, default=360)
+    parser.add_argument('-l','--limit',         help='limit results default is 10000.',type=int, default=10000)
+    parser.add_argument('-nc','--no-color',     help='show result without color.',action='store_true')
+    parser.add_argument('-lv','--list-view-type',help='list view type.',action='store_true')
+    parser.add_argument('-lm','--list-methods',   help='list methods.',  action='store_true')
     parser.add_argument('--init',               help='set the api token.',type=str)
-    parser.add_argument('-T','--timeout',       help='request timeout default is 360 sec.',type=int, default=360)
-    parser.add_argument('-L','--limit',         help='limit results default is 10000.',type=int, default=10000)
 
-    parser.add_argument('-v','--version',         help='version.',action='store_true')
-    #parser.add_argument('-D','--debug',         help='debug mode default is false.',action='store_true', default=False)
-    
+    parser.add_argument('-v','--version',         help='version.',action='store_true') 
+
     parser.epilog  = f'''
 Examples:
 
     # Scan company by domain
-    {Path(sys.argv[0]).name} --domain example.com --scan
+    {Path(sys.argv[0]).name} example.com --scan
 
     # Search for target domain, you will see the result for only this "example.com" 
-    {Path(sys.argv[0]).name} --domain example.com 
+    {Path(sys.argv[0]).name} example.com 
     
+    # Search in target and target subdomains
+    {Path(sys.argv[0]).name} example.com --method domain.all
+
     # Search for target subdomains
-    {Path(sys.argv[0]).name} --domain example.com --all 
-    
-    # Search for target domain, you will see the result for only this "example.com" on United States 
-    {Path(sys.argv[0]).name} --domain example.com --country US 
+    {Path(sys.argv[0]).name} example.com --view-type subdomain
+        
+    # Search for all creds in United States 
+    {Path(sys.argv[0]).name} US --method cred.country
 
     # Search for related companies by domain
-    {Path(sys.argv[0]).name} --domain example.com --related
+    {Path(sys.argv[0]).name} example.com --view-type related
 
     # search for target app id 
-    {Path(sys.argv[0]).name} --app com.example 
+    {Path(sys.argv[0]).name} com.discord --method app.id 
+    
+    # search for target app domain 
+    {Path(sys.argv[0]).name} discord.com --method app.domain
+    
+    # search for target app name 
+    {Path(sys.argv[0]).name} Discord --method app.name
     
-    # Search for target asn
-    {Path(sys.argv[0]).name} --asn AS123 --type-view cred
+    # Search for ip asn
+    {Path(sys.argv[0]).name} AS123 --method ip.asn
 
-    # Search for target username
-    {Path(sys.argv[0]).name} --username someone --country CA
+    # Search for cred username
+    {Path(sys.argv[0]).name} someone --method cred.username
 
-    # Search for target password
-    {Path(sys.argv[0]).name} --password example@123
+    # Search for cred password
+    {Path(sys.argv[0]).name} example@123 --method cred.password
 
-    # Search for target endpoint
-    {Path(sys.argv[0]).name} --endpoint /wp-login.php
+    # Search for url endpoint
+    {Path(sys.argv[0]).name} /wp-login.php --method url.path
 
-    # Search for target cidr
-    {Path(sys.argv[0]).name} --cidr x.x.x.x/24
+    # Search for ip
+    {Path(sys.argv[0]).name} 1.1.1.1 --method ip
+
+    # Search for cidr
+    {Path(sys.argv[0]).name} xx.xx.xx.0/24 --method ip
 
     # Search for target creds by domain emsils
-    {Path(sys.argv[0]).name} --domain example.com --domain-emails 
-    {Path(sys.argv[0]).name} --domain example.com --domain-emails --output example-creds.json --output-type json
-    {Path(sys.argv[0]).name} --domain example.com --domain-emails --view-type email --output example-emails.txt --output-type text
-    
-    # Search for target subdomain
-    {Path(sys.argv[0]).name} --domain company.com --view-type subdomain
-    
+    {Path(sys.argv[0]).name} example.com --method cred.email.domain
+
     # Search for target email
-    {Path(sys.argv[0]).name} --email someone@example.com  
-    {Path(sys.argv[0]).name} --email someone@example.com --view-type url 
+    {Path(sys.argv[0]).name} someone@example.com --method cred.email  
 
     # search for multiple targets: 
-    {Path(sys.argv[0]).name} --domain targets.txt --output example-creds.txt 
-    {Path(sys.argv[0]).name} --domain targets.txt --view-type url --output example-urls.txt 
+    {Path(sys.argv[0]).name} targets.txt --method domain  --output example-creds.txt 
     '''
+
+    argcomplete.autocomplete(parser)
     args = parser.parse_args()
-    if args.version:
-        print(VERSION)
+    if args.list_view_type:
+        for i in VIEW_TYPE_LIST:
+            print(i)
         sys.exit(0)
 
-    if not args.scan and not args.domain and not args.email and not args.app  and not args.cidr and not args.asn and not args.init and not args.username and not args.password and not args.endpoint:
-        parser.print_help()
+    if args.list_methods:
+        for i in _METHODS:
+            print(i)
+        sys.exit(0)
+
+    if args.version:
+        print(VERSION)
         sys.exit(0)
 
     if args.scan:
         root=Scan(options=args)
         root.proc()
 
     else:
```

### Comparing `chiasmodon-1.1.9/setup.py` & `chiasmodon-2.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='1.1.9',
-      description='Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..',
+      version='2.0.0',
+      description='Chiasmodon is an OSINT tool that allows users to gather information from various sources and conduct targeted searches based on domains, Google Play applications, email addresses, IP addresses, organizations, URLs, and more. It provides comprehensive scanning capabilities, customizable output formats, and additional options for enhanced data analysis and customization.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
       scripts=['cli/chiasmodon_cli.py'],
-      install_requires=['requests', 'yaspin', 'tldextract']
-     ) 
+      install_requires=['requests', 'yaspin', 'tldextract','argcomplete']
+    )
```

