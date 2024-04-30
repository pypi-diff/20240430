# Comparing `tmp/cocorum-0.2.0.tar.gz` & `tmp/cocorum-0.3.0.tar.gz`

## Comparing `cocorum-0.2.0.tar` & `cocorum-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.2.0/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 cocorum-0.2.0/src/cocorum/__init__.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 cocorum-0.2.0/src/cocorum/localvars.py
--rw-r--r--   0        0        0    12924 2020-02-02 00:00:00.000000 cocorum-0.2.0/src/cocorum/ssechat.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cocorum-0.2.0/src/cocorum/utils.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 cocorum-0.2.0/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 cocorum-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 cocorum-0.3.0/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 cocorum-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 cocorum-0.3.0/src/cocorum/__init__.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 cocorum-0.3.0/src/cocorum/localvars.py
+-rw-r--r--   0        0        0    13714 2020-02-02 00:00:00.000000 cocorum-0.3.0/src/cocorum/ssechat.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 cocorum-0.3.0/src/cocorum/utils.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cocorum-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 cocorum-0.3.0/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 cocorum-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 cocorum-0.3.0/PKG-INFO
```

### Comparing `cocorum-0.2.0/.github/workflows/python-publish.yml` & `cocorum-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cocorum-0.2.0/src/cocorum/__init__.py` & `cocorum-0.3.0/src/cocorum/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 #!/usr/bin/env python3
-#Python wrapper for the Rumble.com API
-#S.D.G.
+"""Cocorum: a Python wrapper for the Rumble.com API
+
+S.D.G."""
 
-import requests
 import time
 import calendar
+import requests
 
 from .localvars import *
 from .utils import *
 
-class RumbleAPISubObj(object):
+class RumbleAPISubObj():
     """Abstract class for a Rumble API object"""
     def __init__(self, json):
         """Pass the JSON block for a single Rumble API subobject"""
         self._json = json
+
     def __getitem__(self, key):
         """Get a key from the JSON"""
         return self._json[key]
 
 class RumbleUserAction(RumbleAPISubObj):
     """Abstract class for Rumble user actions"""
     def __init__(self, json):
         """Pass the JSON block for a single Rumble user action"""
-        self._json = json
+        super().__init__(json)
         self.__profile_pic = None
 
     def __eq__(self, other):
         """Is this follower equal to another"""
-        if type(other) == str: #Check if the compared string is our username
+        #Check if the compared string is our username
+        if isinstance(other, str):
             return self.username == other
-        if hasattr(other, "username"): #Check if the compared object has a username and if it matches our own
+
+        #Check if the compared object has a username and if it matches our own
+        if hasattr(other, "username"):
             return self.username == other.username
 
     def __str__(self):
         """Follower as a string"""
         return self.username
 
     @property
@@ -51,15 +56,17 @@
         """The user's profile picture as a bytes string"""
         if not self.profile_pic_url: #The profile picture is blank
             return b''
 
         if not self.__profile_pic: #We never queried the profile pic before
             response = requests.get(self.profile_pic_url)
             if response.status_code != 200:
-                raise Exception("Status code " + str(response.status_code))
+                #TODO make this timeout assignable
+                raise Exception("Status code " + str(response.status_code), DEFAULT_TIMEOUT)
+
             self.__profile_pic = response.content
 
         return self.__profile_pic
 
 class RumbleFollower(RumbleUserAction):
     """Rumble follower"""
     @property
@@ -67,21 +74,29 @@
         """When the follower followed, in seconds since Epoch UTC"""
         return parse_timestamp(self["followed_on"])
 
 class RumbleSubscriber(RumbleUserAction):
     """Rumble subscriber"""
     def __eq__(self, other):
         """Is this subscriber equal to another"""
-        if type(other) == str: #Check if the compared string is our username
+        #Check if the compared string is our username
+        if isinstance(other, str):
             return self.username == other
-        if type(other) in (int, float): #check if the compared number is our amount in cents
+
+        #check if the compared number is our amount in cents
+        if isinstance(other, (int, float)):
             return self.amount_cents == other
-        if type(other) == type(self): #Check if the compared subscriber has the same username and amount
-            return (self.username, self.amount_cents) == (other.username, other.amount_cents)
-        if hasattr(other, "username"): #Check if the compared object has a username and if it matches our own
+
+        #Check if the compared object's username matches our own, if it has one
+        if hasattr(other, "username"):
+            #Check if the compared object's cost amout matches our own, if it has one
+            if hasattr(other, "amount_cents"):
+                self.amount_cents == other.amount_cents
+
+            #Other object has no amount_cents attribute
             return self.username == other.username
 
     @property
     def user(self):
         """AFAIK this is being deprecated, use username instead"""
         return self["user"]
 
@@ -98,61 +113,78 @@
     @property
     def subscribed_on(self):
         """When the subscriber subscribed, in seconds since Epoch UTC"""
         return parse_timestamp(self["subscribed_on"])
 
 class RumbleStreamCategory(RumbleAPISubObj):
     """Category of a Rumble stream"""
+
+    @property
     def slug(self):
         """Return the category's slug, AKA it's ID"""
         return self["slug"]
 
+    @property
     def title(self):
         """Return the category's title"""
         return self["title"]
 
     def __eq__(self, other):
         """Is this category equal to another"""
-        if type(other) == str: #Check if the compared string is our slug or title
+        #Check if the compared string is our slug or title
+        if isinstance(other, str):
             return other in (self.slug, self.title)
-        if type(other) == type(self): #Check if the compared category has the same slug
+
+        #Check if the compared object has the same slug, if it has one
+        if hasattr(other, "slug"):
             return self.slug == other.slug
 
     def __str__(self):
         """The category in string form"""
         return self.title
 
-class RumbleLivestream(object):
+class RumbleLivestream():
     """Rumble livestream"""
     def __init__(self, json, api):
         """Pass the JSON block of a single Rumble livestream"""
         self._json = json
         self.api = api
         self.is_disappeared = False #The livestream is in the API listing
         self.__chat = RumbleLiveChat(self)
 
     def __eq__(self, other):
         """Is this stream equal to another"""
-        if type(other) == str: #Check if the compared string is our stream ID
-            return self.stream_id == other
-        if type(other) in (int, float): #check if the compared number is our chat ID (linked to stream ID)
+        #Check if the compared string is our stream ID
+        if isinstance(other, str):
+            return self.stream_id == other #or self.title == other
+
+        #check if the compared number is our chat ID (linked to stream ID)
+        if isinstance(other, (int, float)):
             return self.chat_id == other
-        if hasattr(other, "stream_id"): #Check if the compared object has the same stream ID
+
+        #Check if the compared object has the same stream ID
+        if hasattr(other, "stream_id"):
             return self.stream_id == other.stream_id
-        if hasattr(other, "chat_id"): #Check if the compared object has the same chat ID
+
+        #Check if the compared object has the same chat ID
+        if hasattr(other, "chat_id"):
             return self.stream_id == other.chat_id
 
     def __str__(self):
         """The livestream in string form"""
         return self.stream_id
 
     def __getitem__(self, key):
         """Return a key from the JSON, refreshing if necessary"""
+        #The livestream has not disappeared from the API listing,
+        #the key requested is not a value that doesn't change,
+        #and it has been api.refresh rate since the last time we refreshed
         if (not self.is_disappeared) and (key not in STATIC_KEYS_STREAM) and (time.time() - self.api.last_refresh_time > self.api.refresh_rate):
             self.api.refresh()
+
         return self._json[key]
 
     @property
     def stream_id(self):
         """The livestream ID"""
         return self["id"]
 
@@ -215,21 +247,28 @@
         """The livestream chat"""
         return self.__chat
 
 class RumbleChatMessage(RumbleUserAction):
     """A single message in a Rumble livestream chat"""
     def __eq__(self, other):
         """Is this message equal to another"""
-        if type(other) == str: #Check if the compared string is our message
+        #Check if the compared string is our message
+        if isinstance(other, str):
             return self.text == other
-        if type(other) == type(self): #Check if the compared message has the same username and text
-            return (self.username, self.text) == (other.username, other.text)
-        if hasattr(other, "text"): #Check if the compared object has the same text
-            if hasattr(other, "username"): #Check if the compared object has the same username
+
+        # #Check if the compared message has the same username and text (not needed)
+        # if type(other) == type(self):
+        #     return (self.username, self.text) == (other.username, other.text)
+
+        #Check if the compared object has the same text
+        if hasattr(other, "text"):
+            #Check if the compared object has the same username, if it has one
+            if hasattr(other, "username"):
                 return (self.username, self.text) == (other.username, other.text)
+
             return self.text == other.text #the other object had no username attribute
 
     def __str__(self):
         """Follower as a string"""
         return self.text
 
     @property
@@ -247,24 +286,35 @@
         """The user's badges"""
         return tuple(self["badges"].values())
 
 class RumbleRant(RumbleChatMessage):
     """A single rant in a Rumble livestream chat"""
     def __eq__(self, other):
         """Is this category equal to another"""
-        if type(other) == str: #Check if the compared string is our message
+        #Check if the compared string is our message
+        if isinstance(other, str):
             return self.text == other
-        if type(other) == type(self): #Check if the compared rant has the same username, amount, and text
-            return (self.username, self.amount_cents, self.text) == (other.username, other.amount_cents, other.text)
-        if hasattr(other, "text"): #Check if the compared object has the same text
-            if hasattr(other, "username"): #Check if the compared object has the same username
-                if hasattr(other, "amount_cents"): #Check if the compared object has the same amount
+
+        # #Check if the compared rant has the same username, amount, and text (unneccesary?)
+        # if type(other) == type(self):
+        #     return (self.username, self.amount_cents, self.text) == (other.username, other.amount_cents, other.text)
+
+        #Check if the compared object has the same text
+        if hasattr(other, "text"):
+            #Check if the compared object has the same username, if it has one
+            if hasattr(other, "username"):
+                #Check if the compared object has the same cost amount, if it has one
+                if hasattr(other, "amount_cents"):
                     return (self.username, self.amount_cents, self.text) == (other.username, other.amount_cents, other.text)
-                return (self.username, self.text) == (other.username, other.text) #Other object has no amount_cents attribute
-            return self.text == other.text #Other object had no username attribute
+
+                #Other object has no amount_cents attribute
+                return (self.username, self.text) == (other.username, other.text)
+
+            #Other object had no username attribute
+            return self.text == other.text
 
     @property
     def expires_on(self):
         """When the rant will expire, in seconds since the Epoch UTC"""
         return self["expires_on"]
 
     @property
@@ -273,15 +323,15 @@
         return self["amount_cents"]
 
     @property
     def amount_dollars(self):
         """The rant amount in dollars"""
         return self["amount_dollars"]
 
-class RumbleLiveChat(object):
+class RumbleLiveChat():
     """Reference for chat of a Rumble livestream"""
     def __init__(self, stream):
         """Pass the JSON block of a single Rumble livestream"""
         self.stream = stream
         self.api = stream.api
         self.last_newmessage_time = 0 #Last time we were checked for "new" messages
         self.last_newrant_time = 0 #Last time we were checked for "new" rants
@@ -308,16 +358,17 @@
         """Chat messages that are newer than the last time this was referenced"""
         rem = self.recent_messages.copy()
         rem.sort(key = lambda x: x.created_on) #Sort the messages so the newest ones are last
 
         if rem[-1].created_on < self.last_newmessage_time: #All messages are older than the last time we checked
             return []
 
-        for i in range(len(rem)):
-            if rem[i].created_on > self.last_newmessage_time:
+        i = 0
+        for i, m in enumerate(rem):
+            if m.created_on > self.last_newmessage_time:
                 break #i is now the index of the oldest new message
 
         self.last_newmessage_time = time.time()
         return rem[i:]
 
     @property
     def latest_rant(self):
@@ -331,33 +382,37 @@
         """Recent chat rants"""
         data = self["recent_rants"].copy()
         return [RumbleRant(json_block) for json_block in data]
 
     @property
     def new_rants(self):
         """Chat rants that are newer than the last time this was referenced"""
-        rem = self.recent_rants.copy()
-        rem.sort(key = lambda x: x.created_on) #Sort the rants so the newest ones are last
+        rera = self.recent_rants.copy()
+        rera.sort(key = lambda x: x.created_on) #Sort the rants so the newest ones are last
 
-        if rem[-1].created_on < self.last_newrant_time: #All rants are older than the last time we checked
+        if rera[-1].created_on < self.last_newrant_time: #All rants are older than the last time we checked
             return []
 
-        for i in range(len(rem)):
-            if rem[i].created_on > self.last_newrant_time:
+        i = 0
+        for i, r in enumerate(rera):
+            if r.created_on > self.last_newrant_time:
                 break #i is now the index of the oldest new rant
 
         self.last_newrant_time = time.time()
-        return rem[i:]
+        return rera[i:]
 
-class RumbleAPI(object):
+class RumbleAPI():
     """Rumble API wrapper"""
-    def __init__(self, api_url, refresh_rate = 10):
+    def __init__(self, api_url, refresh_rate = DEFAULT_REFRESH_RATE, request_timeout = DEFAULT_TIMEOUT):
         """Pass the Rumble API URL, and how long to wait before refreshing on new queries"""
         self.refresh_rate = refresh_rate
+        self.request_timeout = request_timeout
+        self.last_refresh_time = 0
         self.__livestreams = {}
+        self._json = {}
         self.api_url = api_url
 
     @property
     def api_url(self):
         """Our API URL"""
         return self.__api_url
 
@@ -377,30 +432,33 @@
         """Refresh only if we are past the refresh rate"""
         if time.time() - self.last_refresh_time > self.refresh_rate:
             self.refresh()
 
     def refresh(self):
         """Reload data from the API"""
         self.last_refresh_time = time.time()
-        response = requests.get(self.api_url, headers = HEADERS)
+        response = requests.get(self.api_url, headers = HEADERS, timeout = self.request_timeout)
         if response.status_code != 200:
             raise Exception("Status code " + str(response.status_code))
+
         self._json = response.json()
 
         #Remove livestream references that are no longer listed
         listed_ids = [json["id"] for json in self._json["livestreams"]]
-        for stream_id in self.__livestreams.copy().keys():
+        for stream_id in self.__livestreams.copy():
             if stream_id not in listed_ids:
                 self.__livestreams[stream_id].is_disappeared = True
                 del self.__livestreams[stream_id]
 
         #Update livestream references' JSONs in-place
         for json in self._json["livestreams"]:
             try:
-                self.__livestreams[json["id"]]._json = json #Reassign the JSON to the stored livestream
+                #Update the JSON of the stored livestream
+                self.__livestreams[json["id"]]._json = json
+
             except KeyError: #The livestream has not been stored yet
                 self.__livestreams[json["id"]] = RumbleLivestream(json, self)
 
     @property
     def api_type(self):
         """Type of API URL in use, user or channel"""
         return self["type"]
```

### Comparing `cocorum-0.2.0/src/cocorum/ssechat.py` & `cocorum-0.3.0/src/cocorum/ssechat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 #!/usr/bin/env python3
-#Rumble SSE chat display client
-#S.D.G.
+"""Rumble SSE chat display client
+
+S.D.G."""
 
-import sseclient
 import json #For parsing SSE message data
+import requests
+import sseclient
 from .localvars import *
 from .utils import *
 
-class SSEChatObject(object):
+class SSEChatObject():
     """Object in SSE chat API"""
-    def __init__(self, json, chat):
+    def __init__(self, jsondata, chat):
         """Pass the object JSON, and the parent SSEChat object"""
-        self._json = json
+        self._jsondata = jsondata
         self.chat = chat
 
     def __getitem__(self, key):
         """Get a key from the JSON"""
-        return self._json[key]
+        return self._jsondata[key]
 
 class SSEChatter(SSEChatObject):
     """A user or channel in the SSE chat"""
-    def __init__(self, json, chat):
+    def __init__(self, jsondata, chat):
         """Pass the object JSON, and the parent SSEChat object"""
-        super().__init__(json, chat)
+        super().__init__(jsondata, chat)
         self.__profile_pic = None #The stored profile picture of the user or channel as a URL
 
     def __eq__(self, other):
         """Compare this chatter with another"""
-        if type(other) == str:
+        #If the other is a string, check if it matches our username
+        if isinstance(other, str):
             return self.username == other
+
+        #If the other has a username attribute, check if it matches our own
         if hasattr(other, "username"):
             return self.username == other.username
 
     def __str__(self):
         """The chatter in string form"""
         return self.username
 
@@ -46,37 +51,39 @@
         """The user's subpage of Rumble.com"""
         return self["link"]
 
     @property
     def profile_pic_url(self):
         """The URL of the chatter's profile picture, if they have one"""
         try:
-            return self._json["image.1"]
+            return self._jsondata["image.1"]
         except KeyError:
             return None
 
     @property
     def profile_pic(self):
         """The chatter's profile picture as a bytes string"""
         if not self.profile_pic_url: #The profile picture is blank
             return b''
 
         if not self.__profile_pic: #We never queried the profile pic before
-            response = requests.get(self.profile_pic_url)
+            #TODO make the timeout configurable
+            response = requests.get(self.profile_pic_url, timeout = DEFAULT_TIMEOUT)
             if response.status_code != 200:
                 raise Exception("Status code " + str(response.status_code))
+
             self.__profile_pic = response.content
 
         return self.__profile_pic
 
 class SSEChatUser(SSEChatter):
     """User in SSE chat"""
-    def __init__(self, json, chat):
+    def __init__(self, jsondata, chat):
         """Pass the object JSON, and the parent SSEChat object"""
-        super().__init__(json, chat)
+        super().__init__(jsondata, chat)
         self.previous_channel_ids = [] #List of channels the user has appeared as, including the current one
 
     @property
     def user_id(self):
         """The numeric ID of the user"""
         return self["id"]
 
@@ -104,52 +111,55 @@
     @property
     def badges(self):
         """Badges the user has"""
         return [self.chat.badges[badge_slug] for badge_slug in self["badges"]]
 
 class SSEChatChannel(SSEChatter):
     """A channel in the SSE chat"""
-    def __init__(self, json, chat):
+    def __init__(self, jsondata, chat):
         """Pass the object JSON, and the parent SSEChat object"""
-        super().__init__(json, chat)
+        super().__init__(jsondata, chat)
 
         #Find the user who has this channel
         for user in self.chat.users.values():
             if user.channel_id == self.channel_id or self.channel_id in user.previous_channel_ids:
                 self.user = user
                 break
 
     @property
     def is_appearing(self):
         """Is the user of this channel still appearing as it?"""
-        return user.channel_id == self.channel_id #The user channel_id still matches our own
+        return self.user.channel_id == self.channel_id #The user channel_id still matches our own
 
     @property
     def channel_id(self):
         """The ID of this channel"""
         return self["id"]
 
     @property
     def user_id(self):
         """The numeric ID of the user of this channel"""
         return self.user.user_id
 
 class SSEChatUserBadge(SSEChatObject):
     """A badge of a user"""
-    def __init__(self, slug, json, chat):
+    def __init__(self, slug, jsondata, chat):
         """Pass the slug, the object JSON, and the parent SSEChat object"""
-        super().__init__(json, chat)
+        super().__init__(jsondata, chat)
         self.slug = slug #The unique identification for this badge
         self.__icon = None
 
     def __eq__(self, other):
         """Check if this badge is equal to another"""
-        if type(other) == str: #Check if the string is either our slug or our label in any language
+        #Check if the string is either our slug or our label in any language
+        if isinstance(other, str):
             return other in (self.slug, self.label.values())
-        if type(other) == type(self): #Compare the other badge's slug with our own
+
+        #Check if the compared object has the same slug, if it has one
+        if hasattr(other, "slug"):
             return self.slug == other.slug
 
     def __str__(self):
         """The chat user badge in string form"""
         return self.slug
 
     @property
@@ -162,34 +172,42 @@
         """The URL of the badge's icon"""
         return RUMBLE_BASE_URL + self["icons"][BADGE_ICON_SIZE]
 
     @property
     def icon(self):
         """The badge's icon as a bytestring"""
         if not self.__icon: #We never queried the icon before
-            response = requests.get(self.icon_url)
+            #TODO make the timeout configurable
+            response = requests.get(self.icon_url, timeout = DEFAULT_TIMEOUT)
             if response.status_code != 200:
                 raise Exception("Status code " + str(response.status_code))
+
             self.__icon = response.content
 
         return self.__icon
 
 class SSEChatMessage(SSEChatObject):
     """A single chat message from the SSE API"""
     def __eq__(self, other):
         """Compare this chat message with another"""
-        if type(other) == str:
+        if isinstance(other, str):
             return self.text == other
 
+        #Check if the other object's text matches our own, if it has such
         if hasattr(other, "text"):
+            #Check if the other object's user ID matches our own, if it has one
             if hasattr(other, "user_id"):
                 return (self.user_id, self.text) == (other.user_id, other.text)
+
+            #Check if the other object's username matches our own, if it has one
             if hasattr(other, "username"):
                 return (self.user.username, self.text) == (other.username, other.text)
-            return self.text == other.text #No user identifying attributes, but the text does match
+
+            #No user identifying attributes, but the text does match
+            return self.text == other.text
 
     def __str__(self):
         """The chat message in string form"""
         return self.text
 
     @property
     def message_id(self):
@@ -224,21 +242,22 @@
         """Reference to the user who posted this message"""
         return self.chat.users[self.user_id]
 
     @property
     def channel(self):
         """Reference to the channel that posted this message, if there was one"""
         if not self.channel_id:
-            return none
+            return None
+
         return self.chat.channels[self.channel_id]
 
     @property
     def is_rant(self):
         """Is this message a rant?"""
-        return "rant" in self._json.keys()
+        return "rant" in self._jsondata.keys()
 
     @property
     def rant_price_cents(self):
         """The price of the rant, returns 0 if message is not a rant"""
         if not self.is_rant:
             return 0
         return self["rant"]["price_cents"]
@@ -253,15 +272,15 @@
     @property
     def rant_expires_on(self):
         """When the rant expires, returns message creation time if message is not a rant"""
         if not self.is_rant:
             return self.time
         return parse_timestamp(self["rant"]["expires_on"])
 
-class SSEChatAPI(object):
+class SSEChatAPI():
     """Access the Rumble SSE chat api"""
     def __init__(self, chat_id = None, stream_id = None):
         if stream_id: #Stream ID as provided by the API
             self.chat_id = id_stream_to_chat(stream_id)
             if chat_id and self.chat_id != chat_id:
                 raise ValueError("Stream ID and chat ID were both specified but they do not match")
         elif chat_id: #Chat ID as it appears in the popout URL
@@ -276,87 +295,89 @@
         self.channels = {} #Dictionary of channels by channel ID
         self.badges = {}
 
         #Connect to the API
         self.url = SSE_CHAT_URL.format(chat_id = self.chat_id)
         self.client = sseclient.SSEClient(self.url)
         self.chat_running = True
-        self.parse_init_data(self.next_json())
+        self.parse_init_data(self.next_jsondata())
 
-    def next_json(self):
+    def next_jsondata(self):
         """Wait for the next message from the SSE and parse the JSON"""
         if not self.chat_running: #Do not try to query a new message if chat is closed
             return
 
         message = next(self.client, None)
         if not message:
             self.chat_running = False #Chat has been closed
             return
         if not message.data: #Blank SSE event
-            return self.next_json() #Self recursion should work so long as we don't get dozens of blank events in a row
+            #Self recursion should work so long as we don't get dozens of blank events in a row
+            return self.next_jsondata()
+
         return json.loads(message.data)
 
-    def parse_init_data(self, json):
+    def parse_init_data(self, jsondata):
         """Extract initial chat data from the SSE init message JSON"""
-        if json["type"] != "init":
+        if jsondata["type"] != "init":
             raise ValueError("That is not init json")
 
         #Parse pre-connection messages, users, and channels
-        self.update_mailbox(json)
-        self.update_users(json)
-        self.update_channels(json)
+        self.update_mailbox(jsondata)
+        self.update_users(jsondata)
+        self.update_channels(jsondata)
 
         #Load the chat badges
-        self.load_badges(json)
+        self.load_badges(jsondata)
 
-        self.rants_enabled = json["data"]["config"]["rants"]["enable"]
+        self.rants_enabled = jsondata["data"]["config"]["rants"]["enable"]
         #subscription TODO
         #rant levels TODO
-        self.message_length_max = json["data"]["config"]["message_length_max"]
+        self.message_length_max = jsondata["data"]["config"]["message_length_max"]
 
-    def update_mailbox(self, json):
+    def update_mailbox(self, jsondata):
         """Parse chat messages from an SSE data JSON"""
-        self.mailbox += [SSEChatMessage(message_json, self) for message_json in json["data"]["messages"]]
+        self.mailbox += [SSEChatMessage(message_json, self) for message_json in jsondata["data"]["messages"]]
 
-    def update_users(self, json):
+    def update_users(self, jsondata):
         """Update our dictionary of users from an SSE data JSON"""
-        for user_json in json["data"]["users"]:
+        for user_json in jsondata["data"]["users"]:
             try:
-                self.users[user_json["id"]]._json = user_json #Update an existing user's JSON
+                self.users[user_json["id"]]._jsondata = user_json #Update an existing user's JSON
             except KeyError: #User is new
                 self.users[user_json["id"]] = SSEChatUser(user_json, self)
 
-    def update_channels(self, json):
+    def update_channels(self, jsondata):
         """Update our dictionary of channels from an SSE data JSON"""
-        for channel_json in json["data"]["users"]:
+        for channel_json in jsondata["data"]["users"]:
             try:
-                self.channels[channel_json["id"]]._json = channel_json #Update an existing channel's JSON
+                self.channels[channel_json["id"]]._jsondata = channel_json #Update an existing channel's JSON
             except KeyError: #Channel is new
                 self.channels.update({channel_json["id"] : SSEChatChannel(channel_json, self)})
 
-    def load_badges(self, json):
+    def load_badges(self, jsondata):
         """Create our dictionary of badges given a dictionary of badges"""
-        self.badges = {badge_slug : SSEChatUserBadge(badge_slug, json["data"]["config"]["badges"][badge_slug], self) for badge_slug in json["data"]["config"]["badges"].keys()}
+        self.badges = {badge_slug : SSEChatUserBadge(badge_slug, jsondata["data"]["config"]["badges"][badge_slug], self) for badge_slug in jsondata["data"]["config"]["badges"].keys()}
 
     @property
     def stream_id(self):
         """If we don't know our stream ID, figure it out from the chat ID"""
         if not self.__stream_id:
             self.__stream_id = id_chat_to_stream(self.chat_id)
 
         return self.__stream_id
 
     def next_chat_message(self):
         """Return the next chat message (parsing any additional data), waits for it to come in, returns None if chat closed"""
         if not self.mailbox: #We don't already have messages
-            json = self.next_json()
-            if not json: #The chat has closed or a blank event
+            jsondata = self.next_jsondata()
+            if not jsondata: #The chat has closed or a blank event
                 return
-            if json["type"] != "messages":
+            if jsondata["type"] != "messages":
                 raise ValueError("API did not send a messages message")
 
             #Parse messages, users, and channels
-            self.update_mailbox(json)
-            self.update_users(json)
-            self.update_channels(json)
+            self.update_mailbox(jsondata)
+            self.update_users(jsondata)
+            self.update_channels(jsondata)
 
         return self.mailbox.pop(0) #Return the first message in the mailbox, and then remove it from there
```

### Comparing `cocorum-0.2.0/src/cocorum/utils.py` & `cocorum-0.3.0/src/cocorum/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
-#Rumble API utilities
-#S.D.G.
+"""Rumble API utilities
+
+S.D.G."""
 
 import calendar
 import time
 from .localvars import *
 
 def parse_timestamp(timestamp):
     """Parse a Rumble timestamp to seconds since Epoch"""
```

### Comparing `cocorum-0.2.0/LICENSE.txt` & `cocorum-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocorum-0.2.0/README.md` & `cocorum-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cocorum-0.2.0/pyproject.toml` & `cocorum-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cocorum"
-version = "0.2.0"
+version = "0.3.0"
 keywords = ["rumble", "api", "wrapper", "livestream"]
 authors = [
   { name="Wilbur Jaywright", email="zargulthewizard@outlook.com" },
 ]
 description = "An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `cocorum-0.2.0/PKG-INFO` & `cocorum-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cocorum
-Version: 0.2.0
+Version: 0.3.0
 Summary: An unofficial Python wrapper for the Rumble Live Stream API v1.0 (beta)
 Project-URL: Homepage, https://github.com/thelabcat/rumble-api-wrapper-py
 Project-URL: Issues, https://github.com/thelabcat/rumble-api-wrapper-py/issues
 Project-URL: Rumble Live Stream API docs, https://rumblefaq.groovehq.com/help/how-to-use-rumble-s-live-stream-api
 Author-email: Wilbur Jaywright <zargulthewizard@outlook.com>
 License-File: LICENSE.txt
 Keywords: api,livestream,rumble,wrapper
```

