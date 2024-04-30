# Comparing `tmp/srinadhch07-0.6.tar.gz` & `tmp/srinadhch07-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srinadhch07-0.6.tar", last modified: Sat Apr 13 18:41:31 2024, max compression
+gzip compressed data, was "srinadhch07-0.7.tar", last modified: Tue Apr 30 18:10:15 2024, max compression
```

## Comparing `srinadhch07-0.6.tar` & `srinadhch07-0.7.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 18:41:31.401874 srinadhch07-0.6/
--rw-rw-rw-   0        0        0     1085 2024-04-10 18:43:19.000000 srinadhch07-0.6/LICENSE
--rw-rw-rw-   0        0        0     4382 2024-04-13 18:41:31.401045 srinadhch07-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3339 2024-04-13 18:31:56.000000 srinadhch07-0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-13 18:41:31.401874 srinadhch07-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1430 2024-04-13 18:39:54.000000 srinadhch07-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 18:41:31.392938 srinadhch07-0.6/srinadhch07/
--rw-rw-rw-   0        0        0    15222 2024-04-10 17:53:11.000000 srinadhch07-0.6/srinadhch07/BAv2.py
--rw-rw-rw-   0        0        0    34935 2024-04-13 18:32:26.000000 srinadhch07-0.6/srinadhch07/BAv2G.py
--rw-rw-rw-   0        0        0     4733 2024-04-13 17:07:28.000000 srinadhch07-0.6/srinadhch07/QueryManager.py
--rw-rw-rw-   0        0        0      166 2024-04-13 18:38:33.000000 srinadhch07-0.6/srinadhch07/__init__.py
--rw-rw-rw-   0        0        0       63 2024-04-10 17:53:13.000000 srinadhch07-0.6/srinadhch07/hello.py
-drwxrwxrwx   0        0        0        0 2024-04-13 18:41:31.400019 srinadhch07-0.6/srinadhch07.egg-info/
--rw-rw-rw-   0        0        0     4382 2024-04-13 18:41:31.000000 srinadhch07-0.6/srinadhch07.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-04-13 18:41:31.000000 srinadhch07-0.6/srinadhch07.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 18:41:31.000000 srinadhch07-0.6/srinadhch07.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-13 18:41:31.000000 srinadhch07-0.6/srinadhch07.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-13 18:41:31.000000 srinadhch07-0.6/srinadhch07.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 18:10:15.956238 srinadhch07-0.7/
+-rw-rw-rw-   0        0        0     1085 2024-04-10 18:43:19.000000 srinadhch07-0.7/LICENSE
+-rw-rw-rw-   0        0        0     4313 2024-04-30 18:10:15.952255 srinadhch07-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3273 2024-04-30 18:08:27.000000 srinadhch07-0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-30 18:10:15.957238 srinadhch07-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2024-04-30 18:09:15.000000 srinadhch07-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 18:10:15.941241 srinadhch07-0.7/srinadhch07/
+-rw-rw-rw-   0        0        0    17929 2024-04-30 18:05:12.000000 srinadhch07-0.7/srinadhch07/BAv2.py
+-rw-rw-rw-   0        0        0       38 2024-04-30 18:06:20.000000 srinadhch07-0.7/srinadhch07/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 18:10:15.951254 srinadhch07-0.7/srinadhch07.egg-info/
+-rw-rw-rw-   0        0        0     4313 2024-04-30 18:10:15.000000 srinadhch07-0.7/srinadhch07.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-04-30 18:10:15.000000 srinadhch07-0.7/srinadhch07.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 18:10:15.000000 srinadhch07-0.7/srinadhch07.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-30 18:10:15.000000 srinadhch07-0.7/srinadhch07.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-30 18:10:15.000000 srinadhch07-0.7/srinadhch07.egg-info/top_level.txt
```

### Comparing `srinadhch07-0.6/LICENSE` & `srinadhch07-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `srinadhch07-0.6/PKG-INFO` & `srinadhch07-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srinadhch07
-Version: 0.6
+Version: 0.7
 Summary: BAv2G
 Home-page: https://github.com/Srinadhch07/BAv2.git
 Author: srinadhch07
 Author-email: <srinadhc07@gmail.com>
 License: MIT
 Keywords: python,video,chat,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
@@ -48,15 +48,15 @@
 BAv2 is available on PyPi:
 
 ```bash
 pip install srinadhch07
 ```
 
 ```bash
-pip install srinadhch07==0.3
+pip install srinadhch07==0.5
 ```
 
 BAv2 officially supports Python 3.8+.
 
 ## Cloning the Repository
 
 ```bash
@@ -64,16 +64,16 @@
 ```
 ## What's new in v2.0?
 ```
 Now this current version is integreted with google geminiai
 ```
 ## What's new in v2.1?
 ```py
-from srinadhch07.BAv2G import chatG
-chatG()
+from srinadhch07.BAv2G import chatbot
+chatbot()
 ```
 ## Requirements
 ```bash
 
 pip install -q -U google-generativeai
 
 ```
@@ -88,19 +88,16 @@
 - Still You can use previous version and present version as per users convenience
 - BAv2 and BAvG both are compitable for both online and offline environments
 
 ## Usage
 
 ```py
 from srinadhch07.BAv2 import chatbot
-from srinadhch07.BAv2G import chatG
 #To start working with BAv2 
 chatbot()
-#to start work with BAv2G
-chatG()
 ```
 
 For more Examples and Functions, have a look at the [Wiki](https://github.com/Srinadhch07/BAv2/wiki).
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `srinadhch07-0.6/README.md` & `srinadhch07-0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 BAv2 is available on PyPi:
 
 ```bash
 pip install srinadhch07
 ```
 
 ```bash
-pip install srinadhch07==0.3
+pip install srinadhch07==0.5
 ```
 
 BAv2 officially supports Python 3.8+.
 
 ## Cloning the Repository
 
 ```bash
@@ -39,16 +39,16 @@
 ```
 ## What's new in v2.0?
 ```
 Now this current version is integreted with google geminiai
 ```
 ## What's new in v2.1?
 ```py
-from srinadhch07.BAv2G import chatG
-chatG()
+from srinadhch07.BAv2G import chatbot
+chatbot()
 ```
 ## Requirements
 ```bash
 
 pip install -q -U google-generativeai
 
 ```
@@ -63,19 +63,16 @@
 - Still You can use previous version and present version as per users convenience
 - BAv2 and BAvG both are compitable for both online and offline environments
 
 ## Usage
 
 ```py
 from srinadhch07.BAv2 import chatbot
-from srinadhch07.BAv2G import chatG
 #To start working with BAv2 
 chatbot()
-#to start work with BAv2G
-chatG()
 ```
 
 For more Examples and Functions, have a look at the [Wiki](https://github.com/Srinadhch07/BAv2/wiki).
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `srinadhch07-0.6/setup.py` & `srinadhch07-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def readme() -> str:
     with open(r"README.md") as f:
         README = f.read()
     return README
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f]
 
-VERSION = '0.6'
+VERSION = '0.7'
 DESCRIPTION = 'BAv2G'
 long_description = 'Updated verision of BAv2'
 
 # Setting up
 setup(
     name="srinadhch07",
     version=VERSION,
```

### Comparing `srinadhch07-0.6/srinadhch07/BAv2.py` & `srinadhch07-0.7/srinadhch07/BAv2.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from os import name,system
 from getpass import getpass
 import webbrowser
 import time
 from  random import *
 import  os
 import ast
+import sys
 # Resurces allocation
 webbrowser.register("termux-open '%s'",None)
 news=["https://www.eenadu.net/latest-news",
 "https://timesofindia.indiatimes.com/home/headlines",
 "https://www.bbc.com/news/world"]
 listen_tech=["https://youtube.com/@TEDx",
 "https://youtube.com/@Prasadtechintelugu",
@@ -63,15 +64,15 @@
 
 
 
 
 class methods:
         
     def main(self):
-            prompt=input("\nYou\t: ")
+            prompt=input("\n\033[3;31;40mYou\t:\033[3;36;40m ")
             prompt=prompt.lower()
             #prompt=prompt.replace(" ","")
             while prompt!="bye" and prompt!="exit" and prompt!="browser" and prompt!="find" and prompt!="19189" and prompt!="history" and prompt!="news" and prompt!="listen tech" and prompt!="listen music" and prompt!="listen news" and prompt!="l music" and prompt!="l news" and prompt!="l tech":
              with open("cloud.txt","r") as f2:
               rf2=f2.read()
                 #dictioanry  read from file
               rdic=ast.literal_eval(rf2)
@@ -82,64 +83,97 @@
                 self.clear()
                 break
                 pass
               if prompt=="count" or prompt=="calculator" or prompt=="math" :
                 self.calculator()
                 break
               if prompt=="edit" or prompt=="change":
-                    edit=input("Brundha :: What would you like to change ?\nYou\t:: ")
+                    edit=input("\033[1;32;40mBrundha :\033[1;37;40m: What would you like to change ?\nYou\t:: ")
                     edit=edit.lower()
                     #edit=edit.replace(" ","")
                     if edit in rdic:
-                        ersp=input("\nBrundha ::Give me new response!\n\t[TYPE 'back' TO CANCEL THE TRAINING]\nYou\t::")
+                        ersp=input("\n\033[1;32;40mBrundha :\033[1;37;40m:Give me new response!\n\t[TYPE 'back' TO CANCEL THE TRAINING]\nYou\t::")
                         mini=ersp.lower()
                         if mini=="back" or mini=="undo":
-                            print("Brundha ::Changes Discarded !")
+                            print("\033[1;32;40mBrundha :\033[1;37;40m:Changes Discarded !")
                             break
                         else:
                             rdic[edit]=ersp
                             self.wfile(rdic)
                             break
                     else:
-                        print("Brundha :: NO such thing to change !")
+                        print("\033[1;32;40mBrundha :\033[1;37;40m: NO such thing to change !")
                         break
               if prompt=="delete" or prompt=="remove":
-                    edit=input("Brundha :: What You like to  remove ?\nYou\t::  ")
+                    edit=input("\033[1;32;40mBrundha :\033[1;37;40m: What You like to  remove ?\nYou\t::  ")
                     edit=edit.lower()
                    # edit=edit.replace(" "," ")
                     if edit in rdic and edit!="back":
-                        ersp=input("\nBrundha :: Do You want to remove ?\n\t[TYPE 'back' TO CANCEL THE TRAINING]\nYou\t:: ")
+                        ersp=input("\n\033[1;32;40mBrundha :\033[1;37;40m: Do You want to remove ?\n\t[TYPE 'back' TO CANCEL THE TRAINING]\nYou\t:: ")
                         mini=ersp.lower()
                         if mini=="back" or mini=="undo":
-                            print("Brundha :: Changes Discarded !")
+                            print("\033[1;32;40mBrundha :\033[1;37;40m: Changes Discarded !")
                             break
                         else:
                             del rdic[edit]
                             self.wfile(rdic)
-                            print("Brundha :Successfully deleted !")
+                            print("\033[1;32;40mBrundha :\033[1;37;40mSuccessfully deleted !")
                             break
                     else:
-                        print("Brundha :: NO such thing to change !")
+                        print("\033[1;32;40mBrundha :\033[1;37;40m: NO such thing to change !")
                         break
 
               if prompt in rdic and prompt!="clear":
-                      print("Brundha :",rdic[prompt])
+                      print("\033[1;32;40m\033[1;32;40mBrundha :\033[1;37;40m\033[1;37;40m",end="")
+                      for char in rdic[prompt]:
+                                if char == '\n':
+                                    sys.stdout.write(char)
+                                    sys.stdout.flush()
+                                    time.sleep(0.1)
+                                elif char == '\t':
+                                    sys.stdout.write(char)
+                                    sys.stdout.flush()
+                                    time.sleep(0.1)
+                                else:
+                                    sys.stdout.write(char)
+                                    sys.stdout.flush()
+                                    time.sleep(0.05)
+                      #print("Brundha :",rdic[prompt])
                       break
               if prompt!="edit" and prompt!="change":
                  if prompt not in rdic:
                     try:
                       convo.send_message(prompt)
                       response=str(convo.last.text)
+                      filtered_response=response.replace("Gemini","Brundha")
                       filtered_response=response.replace("**","||")
-                      print("Brundha :",filtered_response)
+                      #filtered_response=response.replace("gemini","Brundha")
+                      #print("Brundha :",filtered_response)
+                      print("\033[1;32;40mBrundha :\033[1;37;40m ",end="")
+                      for char in filtered_response:
+                                if char == '\n':
+                                    sys.stdout.write(char)
+                                    sys.stdout.flush()
+                                    time.sleep(0.1)
+                                elif char == '\t':
+                                    sys.stdout.write(char)
+                                    sys.stdout.flush()
+                                    time.sleep(0.1)
+                                else:
+                                    sys.stdout.write(char)
+                                    sys.stdout.flush()
+                                    time.sleep(0.05)
                     except:
-                      print("Brundha : I'm sorry the prmopt you have entered is violating safety measures.")
-                    rdic[prompt]=response
-                    self.wfile(rdic)
-                    break
+                      print("\033[1;32;40mBrundha :\033[1;37;40mSorry for the interruption.Your prompt has been unsuccessful. Following statements may reasons for unssuccesful Prompt. \n1.Please check your internet Connection and try again.\n2.I'm sorry the prmopt you have entered is violating safety measures.")
+                    try:
+                        rdic[prompt]=filtered_response
+                        self.wfile(rdic)
+                        break
+                    except:
+                        break
             if prompt=="bye" or prompt=="exit":
                   bye=[
             "Goodbye and take care!",
             "Farewell, my friend!",
             "Until we meet again!",
             "Safe travels!",
             "Wishing You all the best!",
@@ -174,39 +208,39 @@
             "Farewell, and remember You're always in our thoughts!",
             "Safe journey, and goodbye with a smile!",
             "Wishing You a bright and beautiful future!",
             "Take care, and may Your days be filled with sunshine!",
             "Goodbye, and may the memories linger on!",
             "Until next time, stay awesome!",
         ]
-                  print("Brundha :",choice(bye))
+                  print("\033[1;32;40mBrundha :\033[1;37;40m",choice(bye))
                   exit(0)
             if prompt=="find" or prompt=="browser":
                     self.browser()
             if prompt=="19189":
                     with open("cloud.txt",'r') as f:
                         rf=f.read()
                         rdic=ast.literal_eval(rf)
                         rdic=rdic.values()
                         rdic=list(rdic)
                         count=1
-                        print("Brundha :")
+                        print("\033[1;32;40mBrundha :\033[1;37;40m")
                         for i in rdic:
                             print(count," - ",i,"\n")
                             count+=1
 
             if prompt=="history":
                     with open("cloud.txt",'r') as f:
                         rf=f.read()
                         rdic=ast.literal_eval(rf)
                         rdic=rdic.keys()
                         rdic=list(rdic)
                         rdic.reverse()
                         count=1
-                        print("Brundha :")
+                        print("\033[1;32;40mBrundha :\033[1;37;40m")
                         for i in rdic:
                             print(count," - ",i,"\n")
                             count+=1            
             if prompt=="news":
                 new=webbrowser.open_new_tab(choice(news))
             if prompt=="listen news" or prompt=="l news":
                 new=webbrowser.open_new_tab(choice(listen_news))
@@ -217,30 +251,30 @@
     def clear(self):
         if name=="nt":
             _=system('cls')
         if name=='posix':
             _=system('clear')
     def calculator(self):
         try:
-            value=eval(input("Brundha : Enter Expression\nYOU\t: "))
-            print("Brundha : SOLUTION :",value,"\n")
+            value=eval(input("\033[1;32;40mBrundha :\033[1;37;40m Enter Expression\nYOU\t: "))
+            print("\033[1;32;40mBrundha :\033[1;37;40m SOLUTION :",value,"\n")
         except:
-            print("Brundha : Invalid Expression.")
+            print("\033[1;32;40mBrundha :\033[1;37;40m Invalid Expression.")
     def help(self):
             print("""
-Brundha :
+\033[1;32;40mBrundha :\033[1;37;40m
             Additional keys                 Functionality
 
 
             clear/cls           - clears the coversation
             count/calculator        - Opens Calculator
             cancel/undo/back        - used to stop the changes or cancel the actions
             delete/remove           - used to delete the response of the Brundha(Your Assistant)
             edit/change             - Used to edit the response of Brunda
-            search/find             - Opens search Bar for Internet
+            browser/find             - Opens search Bar for Internet
             news                - Redirects to latest News Pages
             listen music/lmusic      - Suggests latest music
             listen news /lnews       - Used to watch latest news
             listen tech /ltech       - Used to watch latest Tech updates
     """)
     def browser(self):
         webbrowser.register("termux-open '%s'",None)
@@ -305,63 +339,63 @@
                 a=os.stat("cloud.txt").st_size
                 if a==0:
                     response_cache={}
                     self.wfile(response_cache)
                     pass
                 else:
                     pass
-            print("Brundha :", choice(greet))
+            print("\033[1;32;40mBrundha :\033[1;37;40m", choice(greet))
 
 
     def security(self):
             f=open("login.txt","a+")
             a=os.stat("login.txt").st_size
             if a==0:
                 print("\t\tBefore using the assistant bot please read the upcoming link....")
                 time.sleep(1)
                 #new=webbrowser.open_new_tab("https://docs.google.com/document/d/13-pLv3yYj3wjVLorW_M2TaddwH7do2tSmkV1dhcSH-k/edit?usp=drivesdk")
                 time.sleep(3)
                 print("\t\tNote : Please be careful while creating pin it cannot be changed due to privacy reaasons\n\n")
                 try:
                     r=int(input("\t\tSIGN-IN\nPIN : "))
                 except:
-                    print("Brundha : Please enter digits only !")
+                    print("\033[1;32;40mBrundha :\033[1;37;40m Please enter digits only !")
                 try:
                     rr=int(input("Confirm Pin : "))
                 except:
-                    print("Brundha : Please enter digits only !")
+                    print("\033[1;32;40mBrundha :\033[1;37;40m Please enter digits only !")
                 if r==rr:
                     f.write('{}'.format(r))
-                    print("Brundha : your assistant setup is  succesful.....")
+                    print("\033[1;32;40mBrundha :\033[1;37;40m your assistant setup is  succesful.....")
                     time.sleep(2)
-                    print("Brundha :About myself ! \nThe BAv2 employs state-of-the-art machine learning techniques.\nSuch as deep learning and reinforcement learning, to continuously enhance its performance. \nIt analyzes vast amounts of data, including user queries, previous interactions, and external sources, to extract meaningful insights and optimize its responses. \nBy leveraging this wealth of information, the app becomes more intelligent, context-aware, and capable of providing personalized assistance tailored to each user's requirements.")
+                    print("\033[1;32;40mBrundha :\033[1;37;40mAbout myself ! \nThe BAv2 employs state-of-the-art machine learning techniques.\nSuch as deep learning and reinforcement learning, to continuously enhance its performance. \nIt analyzes vast amounts of data, including user queries, previous interactions, and external sources, to extract meaningful insights and optimize its responses. \nBy leveraging this wealth of information, the app becomes more intelligent, context-aware, and capable of providing personalized assistance tailored to each user's requirements.")
                     time.sleep(10)
                 else:
-                    print("Brundha :Invalid PIN!")
+                    print("\033[1;32;40mBrundha :\033[1;37;40mInvalid PIN!")
                     self.security()
             f.close()
             with open('login.txt','r') as f:
                 rf=f.read()
                 rf=int(rf)
                 #print(rf)
                 pin=getpass("\n\n\t\tLOG-IN\nPIN  : ")
                 try :
                     pin=int(pin)
                 except:
                     self.clear()
-                    print("Brundha : Please enter digits only !")
+                    print("\033[1;32;40mBrundha :\033[1;37;40m Please enter digits only !")
                 if rf==pin or pin==1821:
                     self.clear()
                     pass
                 else:
                     self.clear()
-                    print("Brundha : Invalid PIN\n")
+                    print("\033[1;32;40mBrundha :\033[1;37;40m Invalid PIN\n")
                     self.security()
 
 def chatbot():
     bot=methods()
     bot.security()
     bot.intro()
     while True:
-        bot.main()     
-                         
+        bot.main()  
 
+
```

### Comparing `srinadhch07-0.6/srinadhch07.egg-info/PKG-INFO` & `srinadhch07-0.7/srinadhch07.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srinadhch07
-Version: 0.6
+Version: 0.7
 Summary: BAv2G
 Home-page: https://github.com/Srinadhch07/BAv2.git
 Author: srinadhch07
 Author-email: <srinadhc07@gmail.com>
 License: MIT
 Keywords: python,video,chat,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
@@ -48,15 +48,15 @@
 BAv2 is available on PyPi:
 
 ```bash
 pip install srinadhch07
 ```
 
 ```bash
-pip install srinadhch07==0.3
+pip install srinadhch07==0.5
 ```
 
 BAv2 officially supports Python 3.8+.
 
 ## Cloning the Repository
 
 ```bash
@@ -64,16 +64,16 @@
 ```
 ## What's new in v2.0?
 ```
 Now this current version is integreted with google geminiai
 ```
 ## What's new in v2.1?
 ```py
-from srinadhch07.BAv2G import chatG
-chatG()
+from srinadhch07.BAv2G import chatbot
+chatbot()
 ```
 ## Requirements
 ```bash
 
 pip install -q -U google-generativeai
 
 ```
@@ -88,19 +88,16 @@
 - Still You can use previous version and present version as per users convenience
 - BAv2 and BAvG both are compitable for both online and offline environments
 
 ## Usage
 
 ```py
 from srinadhch07.BAv2 import chatbot
-from srinadhch07.BAv2G import chatG
 #To start working with BAv2 
 chatbot()
-#to start work with BAv2G
-chatG()
 ```
 
 For more Examples and Functions, have a look at the [Wiki](https://github.com/Srinadhch07/BAv2/wiki).
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

