# Comparing `tmp/librus_apix-0.7.3.tar.gz` & `tmp/librus_apix-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.7.3.tar", last modified: Mon Apr 29 07:53:49 2024, max compression
+gzip compressed data, was "librus_apix-0.7.4.tar", last modified: Tue Apr 30 10:49:02 2024, max compression
```

## Comparing `librus_apix-0.7.3.tar` & `librus_apix-0.7.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:53:49.473608 librus_apix-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 07:53:47.000000 librus_apix-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-29 07:53:49.473608 librus_apix-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-29 07:53:47.000000 librus_apix-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:53:49.469608 librus_apix-0.7.3/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/get_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-29 07:53:47.000000 librus_apix-0.7.3/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:53:49.473608 librus_apix-0.7.3/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-29 07:53:49.000000 librus_apix-0.7.3/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-29 07:53:49.000000 librus_apix-0.7.3/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:53:49.000000 librus_apix-0.7.3/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 07:53:49.000000 librus_apix-0.7.3/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 07:53:49.000000 librus_apix-0.7.3/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-29 07:53:47.000000 librus_apix-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-29 07:53:49.473608 librus_apix-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:53:47.000000 librus_apix-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:49:02.389091 librus_apix-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 10:48:59.000000 librus_apix-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-30 10:49:02.389091 librus_apix-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-30 10:48:59.000000 librus_apix-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:49:02.389091 librus_apix-0.7.4/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/get_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-30 10:48:59.000000 librus_apix-0.7.4/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 10:49:02.389091 librus_apix-0.7.4/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-30 10:49:02.000000 librus_apix-0.7.4/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-30 10:49:02.000000 librus_apix-0.7.4/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 10:49:02.000000 librus_apix-0.7.4/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 10:49:02.000000 librus_apix-0.7.4/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-30 10:49:02.000000 librus_apix-0.7.4/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-30 10:48:59.000000 librus_apix-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-30 10:49:02.389091 librus_apix-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 10:48:59.000000 librus_apix-0.7.4/setup.py
```

### Comparing `librus_apix-0.7.3/LICENSE` & `librus_apix-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.3/README.md` & `librus_apix-0.7.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,19 +92,21 @@
   details = homework_detail(token, href)
   print(details)
 
 ```
 
 ### Sending Messages
 ```py
-from librus_apix.messages import get_recipients, send_message
+from librus_apix.messages import recipient_groups, get_recipients, send_message
 
-recipients = get_recipients(token, "teachers")
+groups = recipient_groups(token)
+recipients = get_recipients(token, groups[0])
 my_recipient = recipients["John Brown"]
 my_second_recipient = recipients["Barbara Brown"]
+
 sent = send_message(token,
                    "Message Title",
                    "Message\n content",
                    "teachers",
                    [my_recipient, my_second_recipient]
 )
 if sent == True:
```

### Comparing `librus_apix-0.7.3/librus_apix/announcements.py` & `librus_apix-0.7.4/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.3/librus_apix/attendance.py` & `librus_apix-0.7.4/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.3/librus_apix/completed_lessons.py` & `librus_apix-0.7.4/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.3/librus_apix/get_token.py` & `librus_apix-0.7.4/librus_apix/get_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         attendance_url: Optional[str] = urls.ATTENDANCE_URL,
         attendance_details_url: Optional[str] = urls.ATTENDANCE_DETAILS_URL,
         schedule_url: Optional[str] = urls.SCHEDULE_URL,
         homework_url: Optional[str] = urls.HOMEWORK_URL,
         homework_details_url: Optional[str] = urls.HOMEWORK_DETAILS_URL,
         info_url: Optional[str] = urls.INFO_URL,
         recipients_url: Optional[str] = urls.RECIPIENTS_URL,
+        recipient_groups_url: Optional[str] = urls.RECIPIENT_GROUPS_URL,
         completed_lessons_url: Optional[str] = urls.COMPLETED_LESSONS_URL,
         gateway_api_attendance: Optional[str] = urls.GATEWAY_API_ATTENDANCE,
         proxy: Optional[dict[str, str]] = {},
     ):
         self._session = Session()
         if not API_Key:
             self.cookies = {}
@@ -51,14 +52,15 @@
         self.SCHEDULE_URL = schedule_url
         self.HOMEWORK_URL = homework_url
         self.HOMEWORK_DETAILS_URL = homework_details_url
         self.INFO_URL = info_url
         self.COMPLETED_LESSONS_URL = completed_lessons_url
         self.GATEWAY_API_ATTENDANCE = gateway_api_attendance
         self.RECIPIENTS_URL = recipients_url
+        self.RECIPIENT_GROUPS_URL = recipient_groups_url
 
     def refresh_oauth(self) -> str:
         with self._session as s:
             s.headers = urls.HEADERS
             s.cookies = cookiejar_from_dict(self.cookies)
             response: Response = s.get(
                 "https://synergia.librus.pl/refreshToken", proxies=self.proxy
@@ -99,14 +101,15 @@
     attendance_url: Optional[str] = urls.ATTENDANCE_URL,
     attendance_details_url: Optional[str] = urls.ATTENDANCE_DETAILS_URL,
     schedule_url: Optional[str] = urls.SCHEDULE_URL,
     homework_url: Optional[str] = urls.HOMEWORK_URL,
     homework_details_url: Optional[str] = urls.HOMEWORK_DETAILS_URL,
     info_url: Optional[str] = urls.INFO_URL,
     recipients_url: Optional[str] = urls.RECIPIENTS_URL,
+    recipient_groups_url: Optional[str] = urls.RECIPIENT_GROUPS_URL,
     completed_lessons_url: Optional[str] = urls.COMPLETED_LESSONS_URL,
     gateway_api_attendance: Optional[str] = urls.GATEWAY_API_ATTENDANCE,
     proxy: Optional[dict[str, str]] = {},
 ) -> Token:
     with Session() as s:
         s.headers = urls.HEADERS
         maint_check = s.get(api_url, proxies=proxy)
@@ -144,13 +147,14 @@
             attendance_url,
             attendance_details_url,
             schedule_url,
             homework_url,
             homework_details_url,
             info_url,
             recipients_url,
+            recipient_groups_url,
             completed_lessons_url,
             gateway_api_attendance,
             proxy=proxy,
         )
 
         return token
```

### Comparing `librus_apix-0.7.3/librus_apix/grades.py` & `librus_apix-0.7.4/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.3/librus_apix/homework.py` & `librus_apix-0.7.4/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.3/librus_apix/messages.py` & `librus_apix-0.7.4/librus_apix/messages.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,33 +12,28 @@
     author: str
     title: str
     date: str
     href: str
     unread: bool
     has_attachment: bool
 
+def recipient_groups(token) -> List[str]:
+    soup = no_access_check(
+        BeautifulSoup(token.get(token.RECIPIENT_GROUPS_URL).text, "lxml")
+    )
+    groups = []
+    trs = soup.select("table.message-recipients > tbody > tr")
+    for tr in trs:
+        radio = tr.select_one("input.recipiantTypeRadio")
+        if radio is None:
+            raise ParseError("Error getting groups (radio)")
+        groups.append(radio.attrs.get("value", ""))
+    return groups
 
-def recipient_groups():
-    return {
-        "teachers": "nauczyciel",
-        "tutors": "wychowawca",
-        "parent_council": "szkolna_rada_rodzicow",
-        "pedagogue": "pedagog",
-        "admin": "admin",
-        "secretary": "sekretariat",
-    }
-
-
-def get_recipients(token: Token, group: str = "teachers"):
-    groups = recipient_groups()
-    if group not in groups:
-        raise ValueError(
-            f"{group} group is not available. Available groups: {' | '.join(groups.keys())}"
-        )
-    group = groups[group]
+def get_recipients(token: Token, group: str):
     payload = {
         "typAdresata": group,
         "poprzednia": 5,
         "tabZaznaczonych": "",
         "czyWirtualneKlasy": False,
         "idGrupy": 0,
     }
@@ -54,41 +49,28 @@
     return teachers
 
 
 def send_message(
     token: Token,
     title: str,
     content: str,
-    recipient_group: str,
     recipient_ids: list[str],
 ):
-    """
-    librus' amazing requests include all possible teacher ids for the group inside the payload.
-    The recipients are differentiated by lack of '_hid' in the key.
-    It might not be needed but I would rather not send a test message to everyone in school accidentally.
-    if anyone is willing to give it a test, good luck.
-    """
-    all_recipients_ids = list(get_recipients(token, recipient_group).values())
     payload = {
         "filtrUzytkownikow": 0,
         "idPojemnika": "",
-        "adresat": recipient_groups().get(recipient_group, ""),
-        "DoKogo_hid": list(
-            filter(lambda id: id not in recipient_ids, all_recipients_ids)
-        ),
-        "DoKogo": list(filter(lambda id: id in recipient_ids, all_recipients_ids)),
+        "DoKogo": recipient_ids,
         "Rodzaj": 0,
         "temat": title,
         "tresc": content,
         "poprzednia": 5,
         "fileStorageIdentifier": "",
         "wyslij": "Wyślij",
     }
     sent_message = token.post(token.SEND_MESSAGE_URL, data=payload)
-
     if sent_message.status_code == 200:
         return True
 
     return False
 
 
 def message_content(token: Token, content_url: str) -> str:
```

### Comparing `librus_apix-0.7.3/librus_apix/schedule.py` & `librus_apix-0.7.4/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.3/librus_apix/student_information.py` & `librus_apix-0.7.4/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.3/librus_apix/timetable.py` & `librus_apix-0.7.4/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.3/librus_apix/urls.py` & `librus_apix-0.7.4/librus_apix/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 }
 BASE_URL = "https://synergia.librus.pl"
 API_URL = "https://api.librus.pl"
 GRADES_URL = BASE_URL + "/przegladaj_oceny/uczen"
 TIMETABLE_URL = f"{BASE_URL}/przegladaj_plan_lekcji"
 ANNOUNCEMENTS_URL = f"{BASE_URL}/ogloszenia"
 MESSAGE_URL = f"{BASE_URL}/wiadomosci/1/5"
+RECIPIENT_GROUPS_URL = f"{BASE_URL}/wiadomosci/2/6"
 RECIPIENTS_URL = f"{BASE_URL}/getRecipients"
 SEND_MESSAGE_URL = f"{BASE_URL}/wiadomosci/1/6"
 ATTENDANCE_URL = f"{BASE_URL}/przegladaj_nb/uczen"
 ATTENDANCE_DETAILS_URL = f"{BASE_URL}/przegladaj_nb/szczegoly/"
 SCHEDULE_URL = f"{BASE_URL}/terminarz/"
 HOMEWORK_URL = f"{BASE_URL}/moje_zadania"
 HOMEWORK_DETAILS_URL = f"{BASE_URL}/moje_zadania/podglad/"
```

### Comparing `librus_apix-0.7.3/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.7.4/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-0.7.3/setup.cfg` & `librus_apix-0.7.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = 0.7.3
+version = 0.7.4
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

