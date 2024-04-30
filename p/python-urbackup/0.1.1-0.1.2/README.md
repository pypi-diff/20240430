# Comparing `tmp/python-urbackup-0.1.1.tar.gz` & `tmp/python-urbackup-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-urbackup-0.1.1.tar", last modified: Sun Apr 28 20:09:11 2024, max compression
+gzip compressed data, was "python-urbackup-0.1.2.tar", last modified: Tue Apr 30 21:42:14 2024, max compression
```

## Comparing `python-urbackup-0.1.1.tar` & `python-urbackup-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:09:11.885025 python-urbackup-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 20:09:06.000000 python-urbackup-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-28 20:09:06.000000 python-urbackup-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-28 20:09:11.885025 python-urbackup-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-28 20:09:06.000000 python-urbackup-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:09:11.885025 python-urbackup-0.1.1/python_urbackup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-28 20:09:11.000000 python-urbackup-0.1.1/python_urbackup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-28 20:09:11.000000 python-urbackup-0.1.1/python_urbackup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 20:09:11.000000 python-urbackup-0.1.1/python_urbackup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-28 20:09:11.000000 python-urbackup-0.1.1/python_urbackup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 20:09:11.000000 python-urbackup-0.1.1/python_urbackup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-28 20:09:11.889025 python-urbackup-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-28 20:09:10.000000 python-urbackup-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 20:09:11.885025 python-urbackup-0.1.1/urbackup/
--rw-r--r--   0 runner    (1001) docker     (127)    12673 2024-04-28 20:09:06.000000 python-urbackup-0.1.1/urbackup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:42:14.492144 python-urbackup-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 21:42:12.000000 python-urbackup-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 21:42:12.000000 python-urbackup-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-30 21:42:14.492144 python-urbackup-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-30 21:42:12.000000 python-urbackup-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:42:14.492144 python-urbackup-0.1.2/python_urbackup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-30 21:42:14.000000 python-urbackup-0.1.2/python_urbackup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-30 21:42:14.000000 python-urbackup-0.1.2/python_urbackup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:42:14.000000 python-urbackup-0.1.2/python_urbackup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 21:42:14.000000 python-urbackup-0.1.2/python_urbackup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 21:42:14.000000 python-urbackup-0.1.2/python_urbackup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 21:42:14.496144 python-urbackup-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-30 21:42:13.000000 python-urbackup-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:42:14.492144 python-urbackup-0.1.2/urbackup/
+-rw-r--r--   0 runner    (1001) docker     (127)    12673 2024-04-30 21:42:12.000000 python-urbackup-0.1.2/urbackup/__init__.py
```

### Comparing `python-urbackup-0.1.1/LICENSE` & `python-urbackup-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-urbackup-0.1.1/PKG-INFO` & `python-urbackup-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: python-urbackup
-Version: 0.1.1
-Summary: Python wrapper to access and control an UrBackup server
-Home-page: https://github.com/judahpaul16/python-urbackup
-Author: Judah Paul
-Author-email: me@judahpaul.com
-License: Apache License 2.0
-Keywords: urbackup web api client
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 # Python UrBackup [![urbackup.org](docs/urbackup.png)](https://www.urbackup.org/)
 
 [![PyPI](https://img.shields.io/pypi/v/python-urbackup)](https://pypi.org/project/python-urbackup/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dirconfig)
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/judahpaul16/python-urbackup/workflow.yaml)](https://github.com/judahpaul16/python-urbackup/actions)
 [![Coverage Status](https://coveralls.io/repos/github/judahpaul16/python-urbackup/badge.svg?branch=master&kill_cache=1)](https://coveralls.io/github/judahpaul16/python-urbackup?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/python-urbackup/badge/?version=latest)](https://python-urbackup.readthedocs.io/en/latest/?badge=latest)
@@ -32,87 +9,86 @@
 Python UrBackup is a powerful Python wrapper designed to interact with UrBackup servers. This library allows you to manage backups, restore operations, and monitor the server status programmatically.
 
 *Originally [urbackup-server-web-api-wrapper](https://github.com/uroni/urbackup-server-python-web-api-wrapper)*
 
 ## Installation
 
 Install with:
-
-	pip3 install python-urbackup
-
-To update the "Usage" section of your GitHub README, we can provide a more detailed and structured snippet that reflects the initialization, login, and some common operations with the `urbackup_server` class. Here is the revised "Usage" section that can be added:
+```bash
+pip install python-urbackup
+```
 
 ## Usage
 
 ### Initialization
 
 Create an instance of the `urbackup_server` by specifying the server URL, username, and password. Replace `'your_server_url'`, `'your_username'`, and `'your_password'` with your server details:
 
 ```python
 from urbackup import urbackup_server
 
-backup_server = urbackup_server('your_server_url', 'your_username', 'your_password')
+server = urbackup_server('your_server_url', 'your_username', 'your_password')
 ```
 
 ### Logging In
 
 To perform any operations, you need to log in:
 
 ```python
-if backup_server.login():
+if server.login():
     print("Login successful!")
 else:
     print("Login failed!")
 ```
 
 ### Getting Client Status
 
 Retrieve the status of a specific client:
 
 ```python
-client_status = backup_server.get_client_status('client_name')
+client_status = server.get_client_status('client_name')
 if client_status:
     print(f"Client status: {client_status}")
 else:
     print("Client not found or access denied.")
 ```
 
 ### Downloading an Installer
 
 To download an installer for a new client, specify the file path and the client's name:
 
 ```python
-if backup_server.download_installer('path/to/installer', 'new_client_name'):
+if server.download_installer('path/to/installer', 'new_client_name'):
     print("Installer downloaded successfully.")
 else:
     print("Failed to download installer.")
 ```
 
 ### Starting Backups
 
 You can start different types of backups for a client. Here are examples of starting an incremental file backup and a full file backup:
 
 ```python
-if backup_server.start_incr_file_backup('client_name'):
+if server.start_incr_file_backup('client_name'):
     print("Incremental file backup started successfully.")
 else:
     print("Failed to start incremental file backup.")
 
-if backup_server.start_full_file_backup('client_name'):
+if server.start_full_file_backup('client_name'):
     print("Full file backup started successfully.")
 else:
     print("Failed to start full file backup.")
 ```
 
 ### Managing Clients
 
 Add a new client to the server:
 
 ```python
-new_client = backup_server.add_client('new_client_name')
+new_client = server.add_client('new_client_name')
 if new_client:
     print("New client added:", new_client)
 else:
     print("Failed to add new client.")
 ```
 
 List clients with no file backup in the last three days:
@@ -134,16 +110,59 @@
 
         print("Last file backup at {lastbackup} of client {clientname} is older than three days".format(
               lastbackup=lastbackup, clientname=client["name"] ) )
 ```
 
 For more information, please refer to the [API Reference](https://python-urbackup.readthedocs.io/en/latest/api_reference/).
 
+## UrBackup CLI <img src="data:image/svg+xml,<svg fill='%234D4D4D' role='img' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'><title>Windows Terminal</title><path d='M8.165 6V3h7.665v3H8.165zm-.5-3H1c-.55 0-1 .45-1 1v2h7.665V3zM23 3h-6.67v3H24V4c0-.55-.45-1-1-1zM0 6.5h24V20c0 .55-.45 1-1 1H1c-.55 0-1-.45-1-1V6.5zM11.5 18c0 .3.2.5.5.5h8c.3 0 .5-.2.5-.5v-1.5c0-.3-.2-.5-.5-.5h-8c-.3 0-.5.2-.5.5V18zm-5.2-4.55l-3.1 3.1c-.25.25-.25.6 0 .8l.9.9c.25.25.6.25.8 0l4.4-4.4a.52.52 0 0 0 0-.8l-4.4-4.4c-.2-.2-.6-.2-.8 0l-.9.9c-.25.2-.25.55 0 .8l3.1 3.1z'/></svg>" width=20>
+
+The UrBackup CLI is a command-line interface that allows you to interact with the UrBackup server from a client machine.
+
+*Important Note: For Windows the command-line tool is `urbackupclient_cmd`. Mac and Linux use `urbackupclientctl`.*
+
+CLI options for `urbackupclientctl` and `urbackupclientctl` are as follows:
+
+```sh
+USAGE:
+
+        urbackupclientctl [--help] [--version] <command> [<args>]
+
+Get specific command help with urbackupclientctl <command> --help
+
+        urbackupclientctl start
+                Start an incremental/full image/file backup
+
+        urbackupclientctl status
+                Get current backup status
+
+        urbackupclientctl browse
+                Browse backups and files/folders in backups
+
+        urbackupclientctl restore-start
+                Restore files/folders from backup
+
+        urbackupclientctl set-settings
+                Set backup settings
+
+        urbackupclientctl reset-keep
+                Reset keeping files during incremental backups
+
+        urbackupclientctl add-backupdir
+                Add new directory to backup set
+
+        urbackupclientctl list-backupdirs
+                List directories that are being backed up
+
+        urbackupclientctl remove-backupdir
+                Remove directory from backup set
+```
+
+For more information, please refer to the [UrBackup Administration Documentation](https://www.urbackup.org/administration_manual.html).
+
 ## Contributing 🤝
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests.
 
 ## License 📃
 
 This project is licensed under the Apache License - see the [LICENSE](LICENSE) file for details.
-
-
```

### Comparing `python-urbackup-0.1.1/python_urbackup.egg-info/PKG-INFO` & `python-urbackup-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-urbackup
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper to access and control an UrBackup server
 Home-page: https://github.com/judahpaul16/python-urbackup
 Author: Judah Paul
 Author-email: me@judahpaul.com
 License: Apache License 2.0
 Keywords: urbackup web api client
 Platform: UNKNOWN
@@ -32,87 +32,86 @@
 Python UrBackup is a powerful Python wrapper designed to interact with UrBackup servers. This library allows you to manage backups, restore operations, and monitor the server status programmatically.
 
 *Originally [urbackup-server-web-api-wrapper](https://github.com/uroni/urbackup-server-python-web-api-wrapper)*
 
 ## Installation
 
 Install with:
-
-	pip3 install python-urbackup
-
-To update the "Usage" section of your GitHub README, we can provide a more detailed and structured snippet that reflects the initialization, login, and some common operations with the `urbackup_server` class. Here is the revised "Usage" section that can be added:
+```bash
+pip install python-urbackup
+```
 
 ## Usage
 
 ### Initialization
 
 Create an instance of the `urbackup_server` by specifying the server URL, username, and password. Replace `'your_server_url'`, `'your_username'`, and `'your_password'` with your server details:
 
 ```python
 from urbackup import urbackup_server
 
-backup_server = urbackup_server('your_server_url', 'your_username', 'your_password')
+server = urbackup_server('your_server_url', 'your_username', 'your_password')
 ```
 
 ### Logging In
 
 To perform any operations, you need to log in:
 
 ```python
-if backup_server.login():
+if server.login():
     print("Login successful!")
 else:
     print("Login failed!")
 ```
 
 ### Getting Client Status
 
 Retrieve the status of a specific client:
 
 ```python
-client_status = backup_server.get_client_status('client_name')
+client_status = server.get_client_status('client_name')
 if client_status:
     print(f"Client status: {client_status}")
 else:
     print("Client not found or access denied.")
 ```
 
 ### Downloading an Installer
 
 To download an installer for a new client, specify the file path and the client's name:
 
 ```python
-if backup_server.download_installer('path/to/installer', 'new_client_name'):
+if server.download_installer('path/to/installer', 'new_client_name'):
     print("Installer downloaded successfully.")
 else:
     print("Failed to download installer.")
 ```
 
 ### Starting Backups
 
 You can start different types of backups for a client. Here are examples of starting an incremental file backup and a full file backup:
 
 ```python
-if backup_server.start_incr_file_backup('client_name'):
+if server.start_incr_file_backup('client_name'):
     print("Incremental file backup started successfully.")
 else:
     print("Failed to start incremental file backup.")
 
-if backup_server.start_full_file_backup('client_name'):
+if server.start_full_file_backup('client_name'):
     print("Full file backup started successfully.")
 else:
     print("Failed to start full file backup.")
 ```
 
 ### Managing Clients
 
 Add a new client to the server:
 
 ```python
-new_client = backup_server.add_client('new_client_name')
+new_client = server.add_client('new_client_name')
 if new_client:
     print("New client added:", new_client)
 else:
     print("Failed to add new client.")
 ```
 
 List clients with no file backup in the last three days:
@@ -134,14 +133,59 @@
 
         print("Last file backup at {lastbackup} of client {clientname} is older than three days".format(
               lastbackup=lastbackup, clientname=client["name"] ) )
 ```
 
 For more information, please refer to the [API Reference](https://python-urbackup.readthedocs.io/en/latest/api_reference/).
 
+## UrBackup CLI <img src="data:image/svg+xml,<svg fill='%234D4D4D' role='img' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'><title>Windows Terminal</title><path d='M8.165 6V3h7.665v3H8.165zm-.5-3H1c-.55 0-1 .45-1 1v2h7.665V3zM23 3h-6.67v3H24V4c0-.55-.45-1-1-1zM0 6.5h24V20c0 .55-.45 1-1 1H1c-.55 0-1-.45-1-1V6.5zM11.5 18c0 .3.2.5.5.5h8c.3 0 .5-.2.5-.5v-1.5c0-.3-.2-.5-.5-.5h-8c-.3 0-.5.2-.5.5V18zm-5.2-4.55l-3.1 3.1c-.25.25-.25.6 0 .8l.9.9c.25.25.6.25.8 0l4.4-4.4a.52.52 0 0 0 0-.8l-4.4-4.4c-.2-.2-.6-.2-.8 0l-.9.9c-.25.2-.25.55 0 .8l3.1 3.1z'/></svg>" width=20>
+
+The UrBackup CLI is a command-line interface that allows you to interact with the UrBackup server from a client machine.
+
+*Important Note: For Windows the command-line tool is `urbackupclient_cmd`. Mac and Linux use `urbackupclientctl`.*
+
+CLI options for `urbackupclientctl` and `urbackupclientctl` are as follows:
+
+```sh
+USAGE:
+
+        urbackupclientctl [--help] [--version] <command> [<args>]
+
+Get specific command help with urbackupclientctl <command> --help
+
+        urbackupclientctl start
+                Start an incremental/full image/file backup
+
+        urbackupclientctl status
+                Get current backup status
+
+        urbackupclientctl browse
+                Browse backups and files/folders in backups
+
+        urbackupclientctl restore-start
+                Restore files/folders from backup
+
+        urbackupclientctl set-settings
+                Set backup settings
+
+        urbackupclientctl reset-keep
+                Reset keeping files during incremental backups
+
+        urbackupclientctl add-backupdir
+                Add new directory to backup set
+
+        urbackupclientctl list-backupdirs
+                List directories that are being backed up
+
+        urbackupclientctl remove-backupdir
+                Remove directory from backup set
+```
+
+For more information, please refer to the [UrBackup Administration Documentation](https://www.urbackup.org/administration_manual.html).
+
 ## Contributing 🤝
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests.
 
 ## License 📃
 
 This project is licensed under the Apache License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `python-urbackup-0.1.1/setup.py` & `python-urbackup-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='python-urbackup',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.1',
+    version='0.1.2',
 
     description='Python wrapper to access and control an UrBackup server',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/judahpaul16/python-urbackup',
```

### Comparing `python-urbackup-0.1.1/urbackup/__init__.py` & `python-urbackup-0.1.2/urbackup/__init__.py`

 * *Files identical despite different names*

