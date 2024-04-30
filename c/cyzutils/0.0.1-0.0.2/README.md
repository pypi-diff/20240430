# Comparing `tmp/cyzutils-0.0.1.tar.gz` & `tmp/cyzutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyzutils-0.0.1.tar", last modified: Mon Apr 15 06:18:52 2024, max compression
+gzip compressed data, was "cyzutils-0.0.2.tar", last modified: Tue Apr 30 11:38:53 2024, max compression
```

## Comparing `cyzutils-0.0.1.tar` & `cyzutils-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 06:18:52.694439 cyzutils-0.0.1/
--rw-rw-rw-   0        0        0      618 2024-04-15 06:18:52.691493 cyzutils-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      366 2024-04-15 06:18:40.000000 cyzutils-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 06:18:52.665464 cyzutils-0.0.1/cyzutils/
--rw-rw-rw-   0        0        0       19 2024-04-08 07:21:05.000000 cyzutils-0.0.1/cyzutils/__init__.py
--rw-rw-rw-   0        0        0     2101 2024-04-15 06:17:35.000000 cyzutils-0.0.1/cyzutils/mail.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:18:52.686447 cyzutils-0.0.1/cyzutils.egg-info/
--rw-rw-rw-   0        0        0      618 2024-04-15 06:18:52.000000 cyzutils-0.0.1/cyzutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2024-04-15 06:18:52.000000 cyzutils-0.0.1/cyzutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 06:18:52.000000 cyzutils-0.0.1/cyzutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 06:18:52.000000 cyzutils-0.0.1/cyzutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 06:18:52.695412 cyzutils-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1116 2024-04-15 06:05:26.000000 cyzutils-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:38:53.751339 cyzutils-0.0.2/
+-rw-rw-rw-   0        0        0      653 2024-04-30 11:38:53.742921 cyzutils-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-04-15 06:35:04.000000 cyzutils-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 11:38:53.714508 cyzutils-0.0.2/cyzutils/
+-rw-rw-rw-   0        0        0       19 2024-04-08 07:21:05.000000 cyzutils-0.0.2/cyzutils/__init__.py
+-rw-rw-rw-   0        0        0     2082 2024-04-30 11:34:25.000000 cyzutils-0.0.2/cyzutils/mail.py
+drwxrwxrwx   0        0        0        0 2024-04-30 11:38:53.740924 cyzutils-0.0.2/cyzutils.egg-info/
+-rw-rw-rw-   0        0        0      653 2024-04-30 11:38:53.000000 cyzutils-0.0.2/cyzutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2024-04-30 11:38:53.000000 cyzutils-0.0.2/cyzutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 11:38:53.000000 cyzutils-0.0.2/cyzutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-30 11:38:53.000000 cyzutils-0.0.2/cyzutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 11:38:53.752335 cyzutils-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1116 2024-04-15 06:33:21.000000 cyzutils-0.0.2/setup.py
```

### Comparing `cyzutils-0.0.1/PKG-INFO` & `cyzutils-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyzutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: my utils
 Home-page: https://github.com/cyz020403
 Author: cyz020403
 Author-email: cyz020403@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,17 +14,19 @@
 ```bash
 pip install cyzutils
 ```
 
 ### Usage
 
 ```python
-from cyzutils import send_email
+from cyzutils import mail
 
-send_email('subject', 'content', 'xxxxxxx@xxx.xx')
+mail('subject', 'content', 'xxxxxxx@xxx.xx')
+
+mail('subject', 'content') # send to myself
 ```
 
 ### 打包上传 pypi 命令
 
 ```shell
 pip install build
```

### Comparing `cyzutils-0.0.1/cyzutils/mail.py` & `cyzutils-0.0.2/cyzutils/mail.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import smtplib
 from email.mime.text import MIMEText
 from email.header import Header
 import base64
 
-def send_email(subject, content, receiver='cyzhelper@qq.com', sender='3544103431@qq.com', passward='uvbrlxzbonezdbai', \
+def mail(subject, content, receiver='cyzhelper@qq.com', sender='cyzhelper@qq.com', passward='idzeantfoqclcdgi', \
                from_nike_name='default', to_nike_name='default'):
     
     mail_host = "smtp.qq.com"
 
     if from_nike_name == 'default':
         from_nike_name = sender.split('@')[0]
     from_nike_name = base64.b64encode(from_nike_name.encode('utf-8')).decode()
@@ -34,16 +34,16 @@
         print('发送失败！！')
 
 
 if __name__ == '__main__':
     print('this is a use demo')
     subject = '嘎嘎gaga'
     content = 'gagaga gagagaga嘎嘎\n' + 'gaga! gaga!'
-    send_email(subject, content)
-    # send_email(subject, content, 'receiver@qq.com', 'sender@qq.com', 'passward')
+    mail(subject, content)
+    # mail(subject, content, 'receiver@qq.com', 'sender@qq.com', 'passward')
 
 '''
 qq邮箱官网教程
 
 POP3/SMTP 设置方法
 用户名/帐户： 你的QQ邮箱完整的地址
```

### Comparing `cyzutils-0.0.1/cyzutils.egg-info/PKG-INFO` & `cyzutils-0.0.2/cyzutils.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyzutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: my utils
 Home-page: https://github.com/cyz020403
 Author: cyz020403
 Author-email: cyz020403@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,17 +14,19 @@
 ```bash
 pip install cyzutils
 ```
 
 ### Usage
 
 ```python
-from cyzutils import send_email
+from cyzutils import mail
 
-send_email('subject', 'content', 'xxxxxxx@xxx.xx')
+mail('subject', 'content', 'xxxxxxx@xxx.xx')
+
+mail('subject', 'content') # send to myself
 ```
 
 ### 打包上传 pypi 命令
 
 ```shell
 pip install build
```

### Comparing `cyzutils-0.0.1/setup.py` & `cyzutils-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(here, 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='cyzutils',  # 必填，项目的名字，用户根据这个名字安装，pip install SpiderKeeper-new
-    version='0.0.1',  # 必填，项目的版本，建议遵循语义化版本规范
+    version='0.0.2',  # 必填，项目的版本，建议遵循语义化版本规范
     author='cyz020403',  # 项目的作者
     description='my utils',  # 项目的一个简短描述
     long_description=long_description,  # 项目的详细说明，通常读取 README.md 文件的内容
     long_description_content_type='text/markdown',  # 描述的格式，可选的值： text/plain, text/x-rst, and text/markdown
     author_email='cyz020403@gmail.com',  # 作者的有效邮箱地址
     url='https://github.com/cyz020403',  # 项目的源码地址
     license='MIT',
```

