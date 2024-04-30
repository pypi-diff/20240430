# Comparing `tmp/jax-tools-1.0.89.tar.gz` & `tmp/jax-tools-1.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-tools-1.0.89.tar", last modified: Wed Nov  8 07:52:55 2023, max compression
+gzip compressed data, was "jax-tools-1.0.97.tar", last modified: Thu Mar 21 02:58:45 2024, max compression
```

## Comparing `jax-tools-1.0.89.tar` & `jax-tools-1.0.97.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-11-08 07:52:55.988923 jax-tools-1.0.89/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-11-08 07:52:55.988319 jax-tools-1.0.89/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      580 2023-06-02 08:47:19.000000 jax-tools-1.0.89/README.md
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-11-08 07:52:55.936226 jax-tools-1.0.89/jax_tools/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 12:57:36.000000 jax-tools-1.0.89/jax_tools/__init__.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-11-08 07:52:55.961766 jax-tools-1.0.89/jax_tools/cmd/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-02 10:01:41.000000 jax-tools-1.0.89/jax_tools/cmd/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      245 2023-06-02 10:08:59.000000 jax-tools-1.0.89/jax_tools/cmd/jax.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     1609 2023-06-06 02:34:28.000000 jax-tools-1.0.89/jax_tools/cmd/jax_encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      643 2023-06-06 03:32:23.000000 jax-tools-1.0.89/jax_tools/cmd/jax_fix.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     3088 2023-11-08 07:52:54.000000 jax-tools-1.0.89/jax_tools/cmd/jax_gpt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.89/jax_tools/cmd/jax_nd.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     4239 2023-10-26 03:40:34.000000 jax-tools-1.0.89/jax_tools/cmd/jax_pam.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      362 2023-06-02 10:03:36.000000 jax-tools-1.0.89/jax_tools/cmd/nd.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-11-08 07:52:55.965946 jax-tools-1.0.89/jax_tools/cmd_tools/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-06-06 02:29:37.000000 jax-tools-1.0.89/jax_tools/cmd_tools/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     9060 2023-10-18 04:43:52.000000 jax-tools-1.0.89/jax_tools/cmd_tools/pam.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     6271 2023-06-27 02:06:15.000000 jax-tools-1.0.89/jax_tools/colorful_font.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     4444 2023-06-06 02:37:59.000000 jax-tools-1.0.89/jax_tools/encrypt.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     2567 2023-08-16 03:29:45.000000 jax-tools-1.0.89/jax_tools/logger.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     3301 2023-06-02 11:00:20.000000 jax-tools-1.0.89/jax_tools/network_test.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      668 2023-07-10 07:14:56.000000 jax-tools-1.0.89/jax_tools/proxies.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      881 2023-07-11 06:13:02.000000 jax-tools-1.0.89/jax_tools/ps.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     4062 2023-07-03 01:31:32.000000 jax-tools-1.0.89/jax_tools/ssh.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-11-08 07:52:55.986783 jax-tools-1.0.89/jax_tools/utils/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        0 2023-05-31 13:11:26.000000 jax-tools-1.0.89/jax_tools/utils/__init__.py
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      254 2023-06-01 08:29:19.000000 jax-tools-1.0.89/jax_tools/utils/settings.py
-drwxr-xr-x   0 cyber.anonym   (501) staff       (20)        0 2023-11-08 07:52:55.944084 jax-tools-1.0.89/jax_tools.egg-info/
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      963 2023-11-08 07:52:55.000000 jax-tools-1.0.89/jax_tools.egg-info/PKG-INFO
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      698 2023-11-08 07:52:55.000000 jax-tools-1.0.89/jax_tools.egg-info/SOURCES.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)        1 2023-11-08 07:52:55.000000 jax-tools-1.0.89/jax_tools.egg-info/dependency_links.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      261 2023-11-08 07:52:55.000000 jax-tools-1.0.89/jax_tools.egg-info/entry_points.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)      112 2023-11-08 07:52:55.000000 jax-tools-1.0.89/jax_tools.egg-info/requires.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       10 2023-11-08 07:52:55.000000 jax-tools-1.0.89/jax_tools.egg-info/top_level.txt
--rw-r--r--   0 cyber.anonym   (501) staff       (20)       38 2023-11-08 07:52:55.989159 jax-tools-1.0.89/setup.cfg
--rw-r--r--   0 cyber.anonym   (501) staff       (20)     2068 2023-11-08 07:52:54.000000 jax-tools-1.0.89/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-21 02:58:45.103751 jax-tools-1.0.97/
+-rw-rw-rw-   0        0        0     1244 2024-03-21 02:58:45.100750 jax-tools-1.0.97/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-06-02 08:47:19.000000 jax-tools-1.0.97/README.md
+drwxrwxrwx   0        0        0        0 2024-03-21 02:58:45.062420 jax-tools-1.0.97/jax_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:57:36.000000 jax-tools-1.0.97/jax_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-21 02:58:45.088580 jax-tools-1.0.97/jax_tools/cmd/
+-rw-rw-rw-   0        0        0        0 2023-06-02 10:01:41.000000 jax-tools-1.0.97/jax_tools/cmd/__init__.py
+-rw-rw-rw-   0        0        0      253 2024-03-08 08:29:42.000000 jax-tools-1.0.97/jax_tools/cmd/jax.py
+-rw-rw-rw-   0        0        0     1617 2024-03-08 08:29:42.000000 jax-tools-1.0.97/jax_tools/cmd/jax_encrypt.py
+-rw-rw-rw-   0        0        0      651 2024-03-08 08:29:42.000000 jax-tools-1.0.97/jax_tools/cmd/jax_fix.py
+-rw-rw-rw-   0        0        0     3195 2023-11-09 07:03:17.000000 jax-tools-1.0.97/jax_tools/cmd/jax_gpt.py
+-rw-rw-rw-   0        0        0      370 2024-03-08 08:34:12.000000 jax-tools-1.0.97/jax_tools/cmd/jax_nd.py
+-rw-rw-rw-   0        0        0     5292 2024-03-11 03:19:34.000000 jax-tools-1.0.97/jax_tools/cmd/jax_pam.py
+-rw-rw-rw-   0        0        0      370 2024-03-11 01:42:12.000000 jax-tools-1.0.97/jax_tools/cmd/nd.py
+drwxrwxrwx   0        0        0        0 2024-03-21 02:58:45.092581 jax-tools-1.0.97/jax_tools/cmd_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-06 02:29:37.000000 jax-tools-1.0.97/jax_tools/cmd_tools/__init__.py
+-rw-rw-rw-   0        0        0     9288 2024-03-11 02:28:42.000000 jax-tools-1.0.97/jax_tools/cmd_tools/pam.py
+-rw-rw-rw-   0        0        0     6496 2024-03-08 08:20:51.000000 jax-tools-1.0.97/jax_tools/colorful_font.py
+-rw-rw-rw-   0        0        0     4761 2024-03-08 08:29:42.000000 jax-tools-1.0.97/jax_tools/encrypt.py
+-rw-rw-rw-   0        0        0     2567 2023-08-16 03:29:45.000000 jax-tools-1.0.97/jax_tools/logger.py
+-rw-rw-rw-   0        0        0     3514 2023-12-21 01:43:32.000000 jax-tools-1.0.97/jax_tools/network_test.py
+-rw-rw-rw-   0        0        0      967 2023-12-21 03:11:45.000000 jax-tools-1.0.97/jax_tools/proxies.py
+-rw-rw-rw-   0        0        0     1253 2024-03-11 01:45:57.000000 jax-tools-1.0.97/jax_tools/ps.py
+-rw-rw-rw-   0        0        0     5829 2024-03-21 02:58:43.000000 jax-tools-1.0.97/jax_tools/ssh.py
+drwxrwxrwx   0        0        0        0 2024-03-21 02:58:45.099750 jax-tools-1.0.97/jax_tools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-31 13:11:26.000000 jax-tools-1.0.97/jax_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      527 2023-12-21 02:57:16.000000 jax-tools-1.0.97/jax_tools/utils/base.py
+-rw-rw-rw-   0        0        0      254 2023-06-01 08:29:19.000000 jax-tools-1.0.97/jax_tools/utils/settings.py
+drwxrwxrwx   0        0        0        0 2024-03-21 02:58:45.073421 jax-tools-1.0.97/jax_tools.egg-info/
+-rw-rw-rw-   0        0        0     1244 2024-03-21 02:58:44.000000 jax-tools-1.0.97/jax_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      722 2024-03-21 02:58:45.000000 jax-tools-1.0.97/jax_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-21 02:58:44.000000 jax-tools-1.0.97/jax_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      261 2024-03-21 02:58:44.000000 jax-tools-1.0.97/jax_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      112 2024-03-21 02:58:44.000000 jax-tools-1.0.97/jax_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-03-21 02:58:44.000000 jax-tools-1.0.97/jax_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-21 02:58:45.103751 jax-tools-1.0.97/setup.cfg
+-rw-rw-rw-   0        0        0     2138 2024-03-21 02:58:43.000000 jax-tools-1.0.97/setup.py
```

### Comparing `jax-tools-1.0.89/README.md` & `jax-tools-1.0.97/README.md`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.89/jax_tools/cmd/jax_encrypt.py` & `jax-tools-1.0.97/jax_tools/cmd/jax_encrypt.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 # Ensure the existence of the encryption key file
 JAX_ENCRYPT = AESCipher().encrypt
 JAX_DECRYPT = AESCipher().decrypt
 
 
-def main():
+def main() -> None:
     """
     main
     Returns:
 
     """
     parser = argparse.ArgumentParser(
         description="Jax-encrypt is used to encrypt and decrypt your sensitive information", prog='JAX-ENCRYPT')
```

### Comparing `jax-tools-1.0.89/jax_tools/cmd/jax_fix.py` & `jax-tools-1.0.97/jax_tools/cmd/jax_fix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 jax_fix use for provide information to help fix problem
 """
 import sys
 
 
-def main():
+def main() -> None:
     """
     Main function
     Returns:
 
     """
     info_dict = {
         "pip": "Upgrade pip: python -m pip install --upgrade pip",
```

### Comparing `jax-tools-1.0.89/jax_tools/cmd/jax_gpt.py` & `jax-tools-1.0.97/jax_tools/cmd/jax_gpt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding:utf-8 -*-
 """
 ask gpt
 """
+import logging
 import os
-import time
+from jax_tools.logger import logger
 
 import openai
 from jax_tools.encrypt import AESCipher
 from typing import TypeVar
 import sys
 
 _KT = TypeVar('_KT')
@@ -31,15 +32,17 @@
         while True:
             question = input('请输入问题：')
             if question in ['exit', 'quit', 'q', '']:
                 print("本次会话结束，再见！")
                 exit(0)
             question_queue.append({"role": "user", "content": question})
             question_queue = handle_question_length(question_queue)
+            logger.info('开始')
             answer = ask_gpt(question_queue)
+            logger.info('结束')
             question_queue += [{"role": "assistant", "content": answer}]
             print()
     except KeyboardInterrupt:
         print("本次会话结束，再见！")
         exit(0)
 
 
@@ -79,15 +82,15 @@
     if not os.path.exists(openai_key_file):
         print('OpenAI key file not found, please create it first, the key file path is: {}'.format(openai_key_file))
     openai_key = AESCipher().decrypt(open(openai_key_file).read())
     # 设置API密钥
     openai.api_key = openai_key
     # 调用OpenAI API并使用流式处理接收响应
     response = openai.ChatCompletion.create(
-        model="gpt-4-1106-preview",
+        model="gpt-3.5-turbo-1106",
         messages=question_queue,
         stream=True
     )
     # Define a variable to store the response
     message = str()
     for chunk in response:
         for char in chunk['choices'][0]['delta'].get('content', ''):
```

### Comparing `jax-tools-1.0.89/jax_tools/cmd/jax_pam.py` & `jax-tools-1.0.97/jax_tools/cmd/jax_pam.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!env python3
 # -*- coding:utf-8 -*-
 """
 Poppy Entrypoint
 """
 from jax_tools.cmd_tools.pam import PasswordManager as pm
+from win10toast import ToastNotifier
 import sys
 import getpass
 import subprocess
 import threading
 
 
 def print_help() -> None:
@@ -46,25 +47,26 @@
     Update account
     Returns:
 
     """
     account_count = pm.print_account_list()
     num = int(input(u'请输入您想要更新的账号NUM(1~{} 从上方首列获取)：'.format(account_count)))
     account_info = pm.get_user_info(num)
-    name = account_info.get(pm.NAME)
-    username = account_info.get(pm.USERNAME)
+    name = account_info.get(pm.NAME_KEY)
+    username = account_info.get(pm.USERNAME_KEY)
     new_name = input(u'请输入新的账号名称(默认名称:{})：'.format(name))
+    new_url = input(u'请输入新的url(默认url:{}): '.format(account_info.get(pm.URL_KEY)))
     new_username = input(u'请输入新的用户名(默认用户名{}): '.format(username))
     if not new_name:
         new_name = name
     if not new_username:
         new_username = username
     password = getpass.getpass(u'请输入登录密码或验证token: ')
     if pm.delete_account(name, print_msg=False):
-        pm.add_account(new_name, new_username, password, num, print_msg=False)
+        pm.add_account(new_name, new_url, new_username, password, num, print_msg=False)
         print(u'NUM:{}, name:{}更新成功'.format(num, name))
 
 
 def delete_account() -> None:
     """
     Delete account
     Returns:
@@ -78,26 +80,33 @@
         pm.delete_account(name)
 
 
 def notify(title: str, message: str) -> None:
     """
     Notify
     Args:
-        title:
-        message:
+        title (str): title of notify
+        message (str): message to notify
 
     Returns:
-
     """
     applescript = f'display notification "{message}" with title "{title}"'
     # If you want to use this function, you need to install terminal-notifier
     try:
+        # try to use terminal-notifier
         subprocess.call(['osascript', '-e', applescript])
+    except (FileNotFoundError, TypeError):
+        pass  # 忽略异常
+
+    try:
+        toaster = ToastNotifier()
+        # 发送通知
+        toaster.show_toast(title, message, duration=1)
     except FileNotFoundError:
-        pass
+        pass  # 忽略异常
 
 
 def main() -> None:
     """
     Main Function
     Returns:
 
@@ -106,35 +115,43 @@
     add_sign_list = ['add', '--add', '-a']
     help_sign_list = ['--help', '-h']
     delete_sign_list = ['--delete', 'delete', '-d']
     update_sign_list = ['--update', 'update', '-u']
     get_sign_list = ['--get', 'get', '-g']
 
     try:
+        # If the first argument is in the list, then execute the corresponding function
         arg_1 = sys.argv[1]
+        # If the first argument is in the list of list_sign_list, then print the account list
         if arg_1 in list_sign_list:
             pm.print_account_list()
+        # If the first argument is in the list of help_sign_list, then print the help message
         elif arg_1 in help_sign_list:
             print_help()
+        # If the first argument is in the list of add_sign_list, then add account
         elif arg_1 in add_sign_list:
             name = input(u'请输入您的要新建的账号名称(如:jenkins web root account)：')
+            url = input(u'请输入您的要新建的账号的url(如:https://www.jenkins.com):')
             username = input(u'请输入你的登录用户名: ')
             password = getpass.getpass(u'请输入你的登录密码或验证token: ')
-            pm.add_account(name, username, password, None)
+            pm.add_account(name, url, username, password, None)
         elif arg_1 in delete_sign_list:
             delete_account()
         elif arg_1 in update_sign_list:
             update_account()
         elif arg_1 in get_sign_list:
             threading.Thread(target=pm().get_password, args=(sys.argv[2],)).start()
             notify('Jax Password Manager',
                    'The content you need has been copied to the clipboard, key:{}'.format(sys.argv[2]))
+
         else:
             threading.Thread(target=minimize_window).start()
             threading.Thread(target=pm().get_password, args=(sys.argv[1],)).start()
+            notify('Jax Password Manager',
+                   'The content you need has been copied to the clipboard, key:{}'.format(sys.argv[1]))
     except IndexError:
         print_help()
     except ValueError:
         print(u'输入的NUM不合法，请重新输入')
     except KeyboardInterrupt:
         print(u'退出程序')
```

### Comparing `jax-tools-1.0.89/jax_tools/cmd_tools/pam.py` & `jax-tools-1.0.97/jax_tools/cmd_tools/pam.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,26 +24,27 @@
     data_file = os.path.join(JAX_DATA_DIR, '.pam.json')
     if os.path.exists(data_file):
         data_list = json.loads(open(data_file, 'r').read())
     else:
         data_list = list()
 
     # Define string
-    NAME = 'name'
-    USERNAME = 'username'
-    PASSWORD = 'password'
+    NAME_KEY = 'name'
+    URL_KEY = 'url'
+    USERNAME_KEY = 'username'
+    PASSWORD_KEY = 'password'
     DUPLICATE_ACCOUNT = u'您输入的账号名在系统中已存在，请修改账号名进行区分'
     ACCOUNT_CREATED = u'账号{}已创建成功'
     ACCOUNT_DELETED = u'账号{}已删除成功'
     NUM_OF_ACCOUNT = u'第{0}个账号信息: {1}'
     ACCOUNT_NOT_FOUND = u'账号{}没有找到，如果您输入的账号信息含空格，请将完整的账号引号"包裹起来'
 
     def get_password(self, search_str: '') -> None:
         """
-        Get Password
+        Get password by search string and copy to clipboard
         Args:
             search_str: Search string
 
         Returns: password
 
         """
         # If search string is integer, get password by num
@@ -69,18 +70,18 @@
 
         """
         # Reverse data list
         for encrypted_pw_info in self.data_list:
             # Decrypt password info
             pw_info = json.loads(AESCipher().decrypt(encrypted_pw_info))
             # Get account name
-            name = pw_info.get(self.NAME)
+            name = pw_info.get(self.NAME_KEY)
             # If name equals search string, copy password to clipboard
             if name.startswith(search_str):
-                return pw_info.get(self.PASSWORD)
+                return pw_info.get(self.PASSWORD_KEY)
         return str()
 
     def __search_by_contains(self, search_str: str) -> str:
         """
         Search by contains
         Args:
             search_str (str): Search string
@@ -89,18 +90,18 @@
 
         """
         # Reverse data list
         for encrypted_pw_info in self.data_list:
             # Decrypt password info
             pw_info = json.loads(AESCipher().decrypt(encrypted_pw_info))
             # Get account name
-            name = pw_info.get(self.NAME)
+            name = pw_info.get(self.NAME_KEY)
             # If name equals search string, copy password to clipboard
             if name.__contains__(search_str):
-                return pw_info.get(self.PASSWORD)
+                return pw_info.get(self.PASSWORD_KEY)
         return str()
 
     def __get_pw_by_num(self, num: int) -> str:
         """
         Get password by num
         Args:
             num (int): Num
@@ -110,15 +111,15 @@
         """
         try:
             encrypted_pw_info = self.data_list[num - 1]
         except IndexError:
             print('Jax Remind: The account number you entered does not exist')
             sys.exit(1)
         pw_info = json.loads(AESCipher().decrypt(encrypted_pw_info))
-        return pw_info.get(self.PASSWORD)
+        return pw_info.get(self.PASSWORD_KEY)
 
     def __search_by_equal(self, search_str: str) -> str:
         """
         Search by equal
         Args:
             search_str (str): Search string
 
@@ -126,18 +127,18 @@
 
         """
         # Reverse data list
         for encrypted_pw_info in self.data_list:
             # Decrypt password info
             pw_info = json.loads(AESCipher().decrypt(encrypted_pw_info))
             # Get account name
-            name = pw_info.get(self.NAME)
+            name = pw_info.get(self.NAME_KEY)
             # If name equals search string, copy password to clipboard
             if name == search_str:
-                return pw_info.get(self.PASSWORD)
+                return pw_info.get(self.PASSWORD_KEY)
         return str()
 
     @classmethod
     def print_account_list(cls) -> int:
         """
         Print account list
         Returns:
@@ -149,16 +150,16 @@
         min_serial_len = 3
         max_serial_len = len(str(len(cls.data_list)))
         space_len = 2
         if max_serial_len < min_serial_len:
             max_serial_len = min_serial_len
         for encrypted_pw_info in cls.data_list:
             pw_info = json.loads(AESCipher().decrypt(encrypted_pw_info))
-            name = pw_info.get(cls.NAME)
-            username = pw_info.get(cls.USERNAME)
+            name = pw_info.get(cls.NAME_KEY)
+            username = pw_info.get(cls.USERNAME_KEY)
             if len(name) > max_name_len:
                 max_name_len = len(name)
             if len(username) > max_username_len:
                 max_username_len = len(username)
         head_and_tail_str = '+' + '-' * (max_serial_len + space_len) + '+' + '-' * (
                 max_name_len + space_len) + '+' + '-' * (max_username_len + space_len) + '+'
         print('Jax Remind: You have {} accounts'.format(len(cls.data_list)))
@@ -166,16 +167,16 @@
               ' then you can paste the password to the specified location')
         print(head_and_tail_str)
         print(f'| {"NUM".ljust(max_serial_len)} | {"NAME".ljust(max_name_len)} | {"USERNAME".ljust(max_username_len)} |'
               )
         print(head_and_tail_str)
         for encrypted_pw_info in cls.data_list:
             pw_info = json.loads(AESCipher().decrypt(encrypted_pw_info))
-            name = pw_info.get(cls.NAME)
-            username = pw_info.get(cls.USERNAME)
+            name = pw_info.get(cls.NAME_KEY)
+            username = pw_info.get(cls.USERNAME_KEY)
             serial_num = cls.data_list.index(encrypted_pw_info) + 1
             print(
                 f'| {str(serial_num).ljust(max_serial_len)} | {name.ljust(max_name_len)} |'
                 f' {username.ljust(max_username_len)} |')
         print(head_and_tail_str)
         return len(cls.data_list)
 
@@ -202,68 +203,69 @@
             print_msg: Print message
 
         Returns:
 
         """
         for encrypted_pw_info in cls.data_list:
             pw_info = json.loads(AESCipher().decrypt(encrypted_pw_info))
-            account_name = pw_info.get(cls.NAME)
+            account_name = pw_info.get(cls.NAME_KEY)
             if name == account_name:
                 cls.data_list.remove(encrypted_pw_info)
                 # dump account list to json
                 data_json = json.dumps(cls.data_list)
                 # write to data file
                 open(cls.data_file, 'w').write(data_json)
                 # Print finally message
                 if print_msg:
                     print(cls.ACCOUNT_DELETED.format(name))
                 return True
         print(cls.ACCOUNT_NOT_FOUND.format(name))
         return False
 
     @classmethod
-    def add_account(cls, name: str, username: str, password: str, num: Optional[int], print_msg: bool = True) -> None:
+    def add_account(cls, name: str, url: str, username: str, password: str, num: Optional[int],
+                    print_msg: bool = True) -> None:
         """
         Add Account to data file
         Args:
             name: Account name
+            url: Account url
             username: Username
             password: Password
-            num: Num
+            num: Num of account
             print_msg: Print message
 
         Returns:
 
         """
         # Traverse encrypted account list
         for encrypted_pw_info in cls.data_list:
             # Get account information
             pw_info = json.loads(AESCipher().decrypt(encrypted_pw_info))
-            account_name = pw_info.get(cls.NAME)
+            account_name = pw_info.get(cls.NAME_KEY)
             # If new name is duplicate with exist name, return and print a message
             if name == account_name:
                 print(cls.DUPLICATE_ACCOUNT)
                 return
         # Define account information use a dict
-        account_info = {cls.NAME: name, cls.USERNAME: username, cls.PASSWORD: password}
+        account_info = {cls.NAME_KEY: name, cls.URL_KEY: url, cls.USERNAME_KEY: username, cls.PASSWORD_KEY: password}
         # Define encrypted account information
         encrypted_account_info = AESCipher().encrypt(json.dumps(account_info))
         # Add new account to account list
         if num:
             cls.data_list.insert(num - 1, encrypted_account_info)
         else:
             cls.data_list.append(encrypted_account_info)
         # dump account list to json
         data_json = json.dumps(cls.data_list)
         # write to data file
-        open(cls.data_file, 'w').write(data_json)
+        open(cls.data_file, 'w', encoding='utf-8').write(data_json)
         # Print finally message
         if print_msg:
             print(cls.ACCOUNT_CREATED.format(name))
 
 
 if __name__ == '__main__':
     try:
         PasswordManager().get_password(sys.argv[1])
     except IndexError:
         print(PasswordManager().get_user_info(2))
-        pass
```

### Comparing `jax-tools-1.0.89/jax_tools/colorful_font.py` & `jax-tools-1.0.97/jax_tools/colorful_font.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Colorful Log Process
 """
 import time
+from typing import Union
 
 
 class ColorfulFont(object):
     """
     Colored Font
     """
     STYLE_NORMAL = 0
@@ -19,88 +20,88 @@
     COLOR_GREEN = 32
     COLOR_YELLOW = 33
     COLOR_FUCHSIA = 35
     COLOR_NORMAL = 39
 
     color_num = COLOR_NORMAL
 
-    def __new__(cls, msg, color_num=None) -> str:
+    def __new__(cls, msg: str, color_num: Union[int] = None) -> str:
         """
         New instance
         Args:
             msg (str): Message text.
             color_num (int): color number
         Returns
             str: Colored text.
         """
         color_num = color_num or cls.color_num
         return cls.text(msg, color_num)
 
     @classmethod
-    def text(cls, msg, color_num=None):
+    def text(cls, msg: str, color_num: Union[int] = None) -> str:
         """
         Get colored text with the given message and color number.
 
         Args:
             msg (str): Message text.
             color_num (int, optional): Color number. If not provided, the default color number of the class will be used
 
         Returns:
             str: Colored text.
         """
         color_num = color_num or cls.color_num
         return cls.colorful_text(cls.STYLE_NORMAL, color_num, msg)
 
     @classmethod
-    def bold(cls, msg, color_num=None):
+    def bold(cls, msg: str, color_num: Union[int] = None) -> str:
         """
         Get bold colored text with the given message and color number.
 
         Args:
             msg (str): Message text.
             color_num (int, optional): Color number. If not provided, the default color number of the class will be used
 
         Returns:
             str: Bold colored text.
         """
         color_num = color_num or cls.color_num
         return cls.colorful_text(cls.STYLE_BOLD, color_num, msg)
 
     @classmethod
-    def underline(cls, msg, color_num=None):
+    def underline(cls, msg: str, color_num: Union[int] = None) -> str:
         """
         Get underlined colored text with the given message and color number.
 
         Args:
             msg (str): Message text.
             color_num (int, optional): Color number. If not provided, the default color number of the class will be used
 
         Returns:
             str: Underlined colored text.
         """
         color_num = color_num or cls.color_num
         return cls.colorful_text(cls.STYLE_UNDERLINE, color_num, msg)
 
     @classmethod
-    def inverse(cls, msg, color_num=None):
+    def inverse(cls, msg: str, color_num: Union[int] = None) -> str:
         """
         Get inversely colored text with the given message and color number.
 
         Args:
             msg (str): Message text.
             color_num (int, optional): Color number. If not provided, the default color number of the class will be used
 
         Returns:
             str: Inversely colored text.
         """
         color_num = color_num or cls.color_num
         return cls.colorful_text(cls.STYLE_INVERSE, color_num, msg)
 
     @classmethod
-    def colorful_text(cls, style, color, msg):
+    def colorful_text(cls, style: int, color: int, msg: str) -> str:
         """
         Colorful text
 
         Args:
             style (int): Text style. Possible values: cls.STYLE_NORMAL, cls.STYLE_BOLD, cls.STYLE_UNDERLINE,
                           cls.STYLE_INVERSE.
             color (int): Color number. Possible values: cls.COLOR_CYANIC, cls.COLOR_RED, cls.COLOR_GREEN,
@@ -151,15 +152,15 @@
 class Normal(ColorfulFont):
     """
     Normal Colored Font
     """
     color_num = ColorfulFont.COLOR_NORMAL
 
 
-def bold_msg(color, msg):
+def bold_msg(color: int, msg: str) -> str:
     """
     Return a bold colorful message.
 
     Args:
         color (int): The color code or name.
         msg (str): The message to be formatted.
 
@@ -172,15 +173,15 @@
 
 class GetColor(ColorfulFont):
     """
     Get Font Color
     """
 
     @classmethod
-    def score(cls, s):
+    def score(cls, s: Union[float, str]) -> int:
         """
         Get color based on the score value.
 
         Args:
             s (float or str): Score value.
 
         Returns:
@@ -199,15 +200,15 @@
             elif s > 0:
                 response = cls.COLOR_GREEN
             else:
                 response = cls.COLOR_NORMAL
         return response
 
     @classmethod
-    def date(cls, d):
+    def date(cls, d: str) -> int:
         """
         Get color based on the date.
 
         Args:
             d (str): Date string.
 
         Returns:
```

### Comparing `jax-tools-1.0.89/jax_tools/encrypt.py` & `jax-tools-1.0.97/jax_tools/encrypt.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from Crypto.Cipher import AES
 from base64 import b64encode
 from base64 import b64decode
 from Crypto.Util.Padding import pad, unpad
 from jax_tools.utils import settings as st
 
 
-def get_local_key():
+def get_local_key() -> str:
     """
     Ensure that the encryption key exists locally, if not, generate a new one
     Returns:
 
     """
     if os.path.exists(st.JAX_KEY_FILE):
         encryption_key = open(st.JAX_KEY_FILE, 'r').read().strip()
@@ -42,15 +42,15 @@
     """
     AES Encryption Class, can use CBC or GCM mode, default is GCM mode
     You can use encrypt_body and decrypt_body to encrypt and decrypt request body
     You can use encrypt_content and decrypt_content to encrypt and decrypt content
     """
 
     # key for encrypting sensitive data
-    def __init__(self, key=get_local_key(), cbc_mode=False):
+    def __init__(self, key: str = get_local_key(), cbc_mode: bool = False) -> None:
         """
         Init method
         Args:
             key: give a token  as a key use for encrypting request body
         """
         if len(key) > 32:
             # Get the key from key 8:24
@@ -62,56 +62,57 @@
         self.cbc_mode = cbc_mode
         if self.cbc_mode:
             self.encryption_mode = AES.MODE_CBC
         else:
             self.encryption_mode = AES.MODE_GCM
 
     @staticmethod
-    def get_random_str(length):
+    def get_random_str(length: int) -> str:
         """
         Get a string from random length.
         Args:
-            length:
+            length (int): Length of random string
 
         Returns:
+            str: Random string
 
         """
         # get secret random
         random_str = ''.join(secrets.choice(string.ascii_letters + string.digits) for _ in range(length))
         return random_str
 
-    def encrypt(self, data, key=str()):
+    def encrypt(self, data: str, key: str = str()) -> str:
         """
         Encryption base  method
         Args:
-            data:
-            key:
+            data (str): Data to encrypt
+            key (str): Encryption key
 
         Returns:
-
+            str: Encrypted string
         """
         if key == str():
             key = self.key
         key = key.encode('utf-8')
         iv = self.get_random_str(AES.block_size)
         cipher = AES.new(key, self.encryption_mode, iv.encode('utf-8'))
         cipher_text = b64encode(cipher.encrypt(pad(data.encode('utf-8'), AES.block_size))).decode()
         result = "{0}{1}{2}{3}".format(iv[:self.length], cipher_text[:self.length], iv[self.length:],
                                        cipher_text[self.length:])
         return result
 
-    def decrypt(self, data, key=str()):
+    def decrypt(self, data: str, key: str = str()) -> str:
         """
         Decryption base method
         Args:
-            data: Data
-            key: Encryption key
+            data (str): Data to decrypt
+            key (str): Encryption key
 
         Returns:
-
+            str: Decrypted string
         """
         if key == str():
             key = self.key
         key = key.encode('utf-8')
         iv = "{0}{1}".format(data[0:self.length], data[self.length
                                                        * 2:self.length * 2 + (AES.block_size - self.length)])
         cipher_text = "{0}{1}".format(
@@ -120,28 +121,26 @@
         try:
             plaintext = unpad(cipher.decrypt(b64decode(cipher_text)), AES.block_size).decode()
         except ValueError:
             plaintext = 'Failed decrypt, please give a correct encrypted string'
         return plaintext
 
 
-def encrypt_hmac_sha256(plaintext, secret_key):
+def encrypt_hmac_sha256(plaintext: str, secret_key: str) -> str:
     """
     Use HMAC-SHA256 to do irreversible encryption, such as encrypting user passwords
 
     Args:
         plaintext: plaintext
         secret_key: secret key
 
     Returns:
-
+        str: Encrypted string
     """
     secret_key = secret_key.encode('utf-8')
     plaintext = plaintext.encode('utf-8')
     cipher_data = base64.b64encode(
         hmac.new(
             secret_key,
             plaintext,
             digestmod=hashlib.sha256).digest())
     return cipher_data.decode()
-
-
```

### Comparing `jax-tools-1.0.89/jax_tools/logger.py` & `jax-tools-1.0.97/jax_tools/logger.py`

 * *Files identical despite different names*

### Comparing `jax-tools-1.0.89/jax_tools/network_test.py` & `jax-tools-1.0.97/jax_tools/network_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 # -*- coding: utf-8 -*-
 """
 Check if the target IP and port is open
 """
 import socket
 import sys
 from ping3 import ping
-from jax_tools.colorful_font import Green as green
-from jax_tools.colorful_font import Red as red
-from jax_tools.colorful_font import Yellow as yellow
+from jax_tools.colorful_font import Green
+from jax_tools.colorful_font import Red
+from jax_tools.colorful_font import Yellow
+from jax_tools.colorful_font import ColorfulFont
+from typing import Optional, Union
 
 
-def check_icmp_connectivity(ip):
+def check_icmp_connectivity(ip: str) -> bool:
     """
     Check if the target IP is reachable
     Args:
         ip(str): IP address or hostname
 
     Returns:
-
+        bool: True if the target IP is reachable, False otherwise
     """
     try:
         # Use ping3 to check if the target IP is reachable
         if ping(ip):
             return True
         else:
             return False
     except Exception as e:
         print(e)
         return False
 
 
-def check_connectivity(ip, port, need_print_msg=False):
+def check_connectivity(ip: str, port: int, need_print_msg: Optional[bool] = False) -> bool:
     """
     检查目标IP和端口是否可以连接
     Args:
         ip (str): Destination IP address or hostname
         port (int): Destination port
         need_print_msg (bool): Whether to print the result
 
     Returns:
-        True if the port is open
-        False if the port is closed or the connection is refused
+        bool: True if the port is open, False if the port is closed or the connection is refused
     """
     print_msg = PrintMSG
     print_msg.need_print = need_print_msg
     s = None
     network_unreachable = 'Network is unreachable'
     result_dict = {
         35: 'The port is closed',
@@ -66,49 +67,49 @@
         # 创建一个socket对象
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.settimeout(5)  # 设置超时时间（单位：秒）
         if isinstance(port, str):
             try:
                 port = int(port)
                 if port < 0 or port > 65535:
-                    print_msg(yellow("The port must be between 0 and 65535"))
+                    print_msg(Yellow("The port must be between 0 and 65535"))
                     sys.exit(1)
             except ValueError:
-                print_msg(yellow("The port must be a number"))
+                print_msg(Yellow("The port must be a number"))
                 sys.exit(1)
         # 尝试连接到目标IP和端口
         result = s.connect_ex((ip, port))
         if result == 0:
-            print_msg(green.bold("Connection success"))
+            print_msg(Green.bold("Connection success"))
             result = True
         elif result in result_dict.keys():
             if check_icmp_connectivity(ip):
-                print_msg(red("Connection error: " + result_dict[result]))
+                print_msg(Red("Connection error: " + result_dict[result]))
             else:
-                print_msg(red("Connection error: " + result_dict[result] + "and ping not work"))
+                print_msg(Red("Connection error: " + result_dict[result] + "and ping not work"))
             result = False
         else:
-            print_msg(red("Connection error：" + str(result)))
+            print_msg(Red("Connection error：" + str(result)))
             result = False
     except socket.error as e:
-        print_msg(red("Connection error：" + e))
+        print_msg(Red("Connection error：" + e))
         result = False
     finally:
         if s:
             s.close()
     return result
 
 
 class PrintMSG(object):
     """
     Print message
     """
     need_print = True
 
-    def __init__(self, msg):
+    def __init__(self, msg: Union[str, ColorfulFont] = str()) -> None:
         """
         Init
         Args:
             msg : Message to print
         """
         if self.need_print:
             print(msg)
```

### Comparing `jax-tools-1.0.89/jax_tools/ps.py` & `jax-tools-1.0.97/jax_tools/ps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,51 @@
+"""
+This module provides a function to get the CPU and memory usage of all processes running on the system.
+"""
 import platform
 import psutil
+from typing import TypeVar
+KT = TypeVar('KT')
+VT = TypeVar('VT')
 
-def get_process_info():
+
+def get_process_info() -> list[dict[str, VT]]:
+    """
+    Get process info
+    Returns:
+
+    """
     processes = []
     for process in psutil.process_iter(['pid', 'name', 'cpu_percent', 'memory_percent']):
         processes.append(process.info)
     return processes
 
-def print_process_info():
+
+def print_process_info() -> None:
+    """
+    Print process info
+    Returns:
+
+    """
     processes = get_process_info()
     filtered_processes = [process for process in processes if process['cpu_percent'] is not None]
     sorted_processes = sorted(filtered_processes, key=lambda x: x['cpu_percent'], reverse=True)
     print("PID\tCPU%\tMemory%\tName")
     for process in sorted_processes:
         print(f"{process['pid']}\t{process['cpu_percent']}\t{process['memory_percent']}\t{process['name']}")
 
-def main():
+
+def main() -> None:
+    """
+    Main function
+    Returns:
+
+    """
     system = platform.system()
     if system == 'Linux' or system == 'Darwin':
         print_process_info()
     else:
         print("Unsupported operating system.")
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `jax-tools-1.0.89/jax_tools/ssh.py` & `jax-tools-1.0.97/jax_tools/ssh.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # -*- coding: utf-8 -*-
 """
 ssh operations
 """
+import os.path
+
 import paramiko
 from jax_tools.logger import logger
+from typing import Optional
+import base64
 
 
 class SSHClient(object):
     """
     SSH Connector
     """
     SSH_CONNECTION_FAILED = 'SSH connection failed'
 
-    def __init__(self, host, port, username, password) -> None:
+    def __init__(self, host: str, port: int, username: str, password: str) -> None:
         """
         SSH Connector
         Args:
             host (str): host for ssh connection
             port (int): port for ssh connection
             username (str): username for ssh connection
             password (str): password for ssh connection
         """
         self.host = host
         self.username = username
         self.password = password
         self.port = port
         self.ssh_client = self.__get_ssh_client()
 
-    def __get_ssh_client(self):
+    def __get_ssh_client(self) -> Optional[paramiko.SSHClient]:
         """
         Get ssh client
         Args:
 
         Returns:
             ssh client or None
 
@@ -56,15 +60,15 @@
             logger.error(e)
             response = None
         if response:
             return client
         else:
             return response
 
-    def run_cmd(self, cmd, read_line=False, time_out=300):
+    def run_cmd(self, cmd: str, read_line: bool = False, time_out: int = 300) -> Optional[str]:
         """
         Run command on remote host
         Args:
             cmd (str): command to run
             read_line (bool): True if read line by line, False if read all
             time_out (int): timeout in seconds
 
@@ -83,37 +87,82 @@
             else:
                 result = std_out.read().decode('utf-8').rstrip()
         except Exception as e:
             logger.error('Connection exception, User login info may be wrong, or connection has been closed, '
                          ' msg: %s' % e)
         return result
 
-    def put_file(self, local_file, remote_file):
+    def put_file(self, local_file: str, remote_file: str) -> None:
         """
         Put file to remote host
         Args:
             local_file (str): local file path
             remote_file (str): remote file path
 
         Returns:
 
         """
         if self.ssh_client is None:
             logger.warning(self.SSH_CONNECTION_FAILED)
             return
+        if not os.path.exists(local_file):
+            logger.warning('Local file not exists')
+            return
+        try:
+            with open(local_file, 'rb') as f:
+                file_content = f.read()
+                encoded_content = base64.b64encode(file_content).decode('utf-8')
+                self.run_cmd('echo "{}" | base64 --decode > {}'.format(encoded_content, remote_file))
+        except Exception as e:
+            logger.error('Got exception in put file to remote server: %s' % e)
+
+    def get_file(self, remote_file: str, local_file: str) -> None:
+        """
+        Get file from remote host
+        Args:
+            remote_file (str): remote file path
+            local_file (str): local file path
+
+        Returns:
+
+        """
+        if self.ssh_client is None:
+            logger.warning(self.SSH_CONNECTION_FAILED)
+            return
+        try:
+            file_content = self.run_cmd('cat {}'.format(remote_file))
+            if file_content:
+                with open(local_file, 'w') as f:
+                    f.write(file_content)
+        except Exception as e:
+            logger.error('Got exception in get file from remote server: %s' % e)
+
+    def sftp_put_file(self, local_file: str, remote_file: str) -> None:
+        """
+        Put file to remote host using sftp
+        Args:
+            local_file (str): local file path
+            remote_file (str): remote file path
+
+        Returns:
+
+        """
+        if self.ssh_client is None:
+            logger.warning(self.SSH_CONNECTION_FAILED)
+            return
         try:
             sftp_client = self.ssh_client.open_sftp()
             sftp_client.put(local_file, remote_file)
         except Exception as e:
             logger.error('Connection exception, User login info may be wrong, or connection has been closed, '
                          ' msg: %s' % e)
 
-    def get_file(self, remote_file, local_file):
+    def sftp_get_file(self, remote_file: str, local_file: str) -> None:
         """
-        Get file from remote host
+        Get file from remote host using sftp
         Args:
             remote_file (str): remote file path
             local_file (str): local file path
 
         Returns:
 
         """
@@ -130,11 +179,10 @@
         """
         Close ssh connection
         Returns:
 
         """
         self.ssh_client.close()
 
-    def __del__(self):
+    def __del__(self) -> None:
         if self.ssh_client:
             self.close()
-
```

### Comparing `jax-tools-1.0.89/jax_tools.egg-info/SOURCES.txt` & `jax-tools-1.0.97/jax_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 jax_tools/cmd/jax_gpt.py
 jax_tools/cmd/jax_nd.py
 jax_tools/cmd/jax_pam.py
 jax_tools/cmd/nd.py
 jax_tools/cmd_tools/__init__.py
 jax_tools/cmd_tools/pam.py
 jax_tools/utils/__init__.py
+jax_tools/utils/base.py
 jax_tools/utils/settings.py
```

### Comparing `jax-tools-1.0.89/setup.py` & `jax-tools-1.0.97/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# -*- coding:utf-8 -*-
-"""
-pypi定义打包信息的文件
-"""
-import setuptools
-
-
-def read_file(file_path):
-    """
-    Read file
-    Args:
-        file_path (str): file path
-
-    Returns:
-
-    """
-    with open(file_path, 'r') as f:
-        return f.read()
-
-
-setuptools.setup(
-    name="jax-tools",
-    version="1.0.89",
-    author=u"Jax",
-    author_email='alvin.wan.cn@hotmail.com',
-    description=u"Jax common tools library",
-    platforms=['CentOS', 'Redhat', 'MacOS', 'Windows'],
-    long_description=read_file('README.md'),
-    long_description_content_type="text/markdown",
-    url="https://jax-arsenals.com",
-    license="MIT Licence",
-    python_requires=">=3.0.0",
-    # 定义要构建到包中的文件列表，这些文件会放到/usr/local下
-    data_files=[],
-    packages=['jax_tools', 'jax_tools.utils', 'jax_tools.cmd', 'jax_tools.cmd_tools'],
-    exclude=['build.py'],
-    package_dir={},
-    package_data={
-        # 'jax_tools': ['*.md'],
-        '': ['CHANGELOG.md']
-    },
-    include_package_data=True,
-    keywords=['jax'],
-    # 安装时需要执行的脚本列表，如可用于管理配置文件
-    scripts=[],
-    download_url="https://jax-arsenals.com",
-    # 定义可以为哪些模块提供依赖
-    provides=[],
-    install_requires=[
-        "ping3 >= 4.0.4",
-        "paramiko >= 3.2.0",
-        "colorlog >= 6.7.0",
-        "pycryptodome >= 3.18.0",
-        "pyperclip >= 1.8.2",
-        "psutil >= 5.9.5",
-        "openai == 0.27.8"
-    ],
-    # 定义entry points, 前面的sta指的是命令，第二个sta表示模块名，也是目录名，第三个sta表示脚本名，最好那个main，表示sta.py中的main函数
-    entry_points={
-        'console_scripts': [
-            'jax=jax_tools.cmd.jax:main',
-            'nd=jax_tools.cmd.nd:main',
-            'jax-nd=jax_tools.cmd.nd:main',
-            'jax-encrypt=jax_tools.cmd.jax_encrypt:main',
-            'jax-fix=jax_tools.cmd.jax_fix:main',
-            'jax-pam=jax_tools.cmd.jax_pam:main',
-            'jax-gpt=jax_tools.cmd.jax_gpt:main',
-        ]
-    }
-)
+# -*- coding:utf-8 -*-
+"""
+pypi定义打包信息的文件
+"""
+import setuptools
+
+
+def read_file(file_path):
+    """
+    Read file
+    Args:
+        file_path (str): file path
+
+    Returns:
+
+    """
+    with open(file_path, 'r') as f:
+        return f.read()
+
+
+setuptools.setup(
+    name="jax-tools",
+    version="1.0.97",
+    author=u"Jax",
+    author_email='alvin.wan.cn@hotmail.com',
+    description=u"Jax common tools library",
+    platforms=['CentOS', 'Redhat', 'MacOS', 'Windows'],
+    long_description=read_file('README.md'),
+    long_description_content_type="text/markdown",
+    url="https://jax-arsenals.com",
+    license="MIT Licence",
+    python_requires=">=3.0.0",
+    # 定义要构建到包中的文件列表，这些文件会放到/usr/local下
+    data_files=[],
+    packages=['jax_tools', 'jax_tools.utils', 'jax_tools.cmd', 'jax_tools.cmd_tools'],
+    exclude=['build.py'],
+    package_dir={},
+    package_data={
+        # 'jax_tools': ['*.md'],
+        '': ['CHANGELOG.md']
+    },
+    include_package_data=True,
+    keywords=['jax'],
+    # 安装时需要执行的脚本列表，如可用于管理配置文件
+    scripts=[],
+    download_url="https://jax-arsenals.com",
+    # 定义可以为哪些模块提供依赖
+    provides=[],
+    install_requires=[
+        "ping3 >= 4.0.4",
+        "paramiko >= 3.2.0",
+        "colorlog >= 6.7.0",
+        "pycryptodome >= 3.18.0",
+        "pyperclip >= 1.8.2",
+        "psutil >= 5.9.5",
+        "openai == 0.27.8"
+    ],
+    # 定义entry points, 前面的sta指的是命令，第二个sta表示模块名，也是目录名，第三个sta表示脚本名，最好那个main，表示sta.py中的main函数
+    entry_points={
+        'console_scripts': [
+            'jax=jax_tools.cmd.jax:main',
+            'nd=jax_tools.cmd.nd:main',
+            'jax-nd=jax_tools.cmd.nd:main',
+            'jax-encrypt=jax_tools.cmd.jax_encrypt:main',
+            'jax-fix=jax_tools.cmd.jax_fix:main',
+            'jax-pam=jax_tools.cmd.jax_pam:main',
+            'jax-gpt=jax_tools.cmd.jax_gpt:main',
+        ]
+    }
+)
```

