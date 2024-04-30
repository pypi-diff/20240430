# Comparing `tmp/interaction_discord_bot-0.1.4.tar.gz` & `tmp/interaction_discord_bot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interaction_discord_bot-0.1.4.tar", last modified: Tue Apr  9 20:06:59 2024, max compression
+gzip compressed data, was "interaction_discord_bot-0.1.9.tar", last modified: Tue Apr 30 18:26:38 2024, max compression
```

## Comparing `interaction_discord_bot-0.1.4.tar` & `interaction_discord_bot-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 appez     (1000) appez     (1000)        0 2024-04-09 20:06:59.514259 interaction_discord_bot-0.1.4/
--rw-r--r--   0 appez     (1000) appez     (1000)      156 2024-04-09 20:06:59.514259 interaction_discord_bot-0.1.4/PKG-INFO
--rw-rw-r--   0 appez     (1000) appez     (1000)        5 2024-04-05 22:01:13.000000 interaction_discord_bot-0.1.4/README.md
-drwxrwxr-x   0 appez     (1000) appez     (1000)        0 2024-04-09 20:06:59.514259 interaction_discord_bot-0.1.4/interaction_discord_bot/
--rw-rw-r--   0 appez     (1000) appez     (1000)        0 2024-04-05 21:26:53.000000 interaction_discord_bot-0.1.4/interaction_discord_bot/__init__.py
--rw-rw-r--   0 appez     (1000) appez     (1000)      865 2024-04-09 20:06:35.000000 interaction_discord_bot-0.1.4/interaction_discord_bot/message.py
-drwxrwxr-x   0 appez     (1000) appez     (1000)        0 2024-04-09 20:06:59.514259 interaction_discord_bot-0.1.4/interaction_discord_bot/modal/
--rw-rw-r--   0 appez     (1000) appez     (1000)        0 2024-04-06 03:11:05.000000 interaction_discord_bot-0.1.4/interaction_discord_bot/modal/__init__.py
--rw-rw-r--   0 appez     (1000) appez     (1000)      985 2024-04-05 21:34:16.000000 interaction_discord_bot-0.1.4/interaction_discord_bot/modal/speakModal.py
-drwxrwxr-x   0 appez     (1000) appez     (1000)        0 2024-04-09 20:06:59.514259 interaction_discord_bot-0.1.4/interaction_discord_bot.egg-info/
--rw-r--r--   0 appez     (1000) appez     (1000)      156 2024-04-09 20:06:59.000000 interaction_discord_bot-0.1.4/interaction_discord_bot.egg-info/PKG-INFO
--rw-rw-r--   0 appez     (1000) appez     (1000)      409 2024-04-09 20:06:59.000000 interaction_discord_bot-0.1.4/interaction_discord_bot.egg-info/SOURCES.txt
--rw-rw-r--   0 appez     (1000) appez     (1000)        1 2024-04-09 20:06:59.000000 interaction_discord_bot-0.1.4/interaction_discord_bot.egg-info/dependency_links.txt
--rw-rw-r--   0 appez     (1000) appez     (1000)        9 2024-04-09 20:06:59.000000 interaction_discord_bot-0.1.4/interaction_discord_bot.egg-info/requires.txt
--rw-rw-r--   0 appez     (1000) appez     (1000)       24 2024-04-09 20:06:59.000000 interaction_discord_bot-0.1.4/interaction_discord_bot.egg-info/top_level.txt
--rw-rw-r--   0 appez     (1000) appez     (1000)       38 2024-04-09 20:06:59.514259 interaction_discord_bot-0.1.4/setup.cfg
--rw-rw-r--   0 appez     (1000) appez     (1000)      271 2024-04-09 20:06:50.000000 interaction_discord_bot-0.1.4/setup.py
+drwxrwxr-x   0 appez     (1000) appez     (1000)        0 2024-04-30 18:26:38.330095 interaction_discord_bot-0.1.9/
+-rw-r--r--   0 appez     (1000) appez     (1000)      156 2024-04-30 18:26:38.330095 interaction_discord_bot-0.1.9/PKG-INFO
+-rw-rw-r--   0 appez     (1000) appez     (1000)        5 2024-04-05 22:01:13.000000 interaction_discord_bot-0.1.9/README.md
+drwxrwxr-x   0 appez     (1000) appez     (1000)        0 2024-04-30 18:26:38.330095 interaction_discord_bot-0.1.9/interaction_discord_bot/
+-rw-rw-r--   0 appez     (1000) appez     (1000)        0 2024-04-05 21:26:53.000000 interaction_discord_bot-0.1.9/interaction_discord_bot/__init__.py
+drwxrwxr-x   0 appez     (1000) appez     (1000)        0 2024-04-30 18:26:38.330095 interaction_discord_bot-0.1.9/interaction_discord_bot/cogs/
+-rw-rw-r--   0 appez     (1000) appez     (1000)        0 2024-04-11 19:34:56.000000 interaction_discord_bot-0.1.9/interaction_discord_bot/cogs/__init__.py
+-rw-rw-r--   0 appez     (1000) appez     (1000)      996 2024-04-13 19:02:05.000000 interaction_discord_bot-0.1.9/interaction_discord_bot/cogs/message.py
+-rw-rw-r--   0 appez     (1000) appez     (1000)      114 2024-04-11 19:49:25.000000 interaction_discord_bot-0.1.9/interaction_discord_bot/init_cog.py
+drwxrwxr-x   0 appez     (1000) appez     (1000)        0 2024-04-30 18:26:38.330095 interaction_discord_bot-0.1.9/interaction_discord_bot/modal/
+-rw-rw-r--   0 appez     (1000) appez     (1000)        0 2024-04-06 03:11:05.000000 interaction_discord_bot-0.1.9/interaction_discord_bot/modal/__init__.py
+-rw-rw-r--   0 appez     (1000) appez     (1000)     1147 2024-04-09 20:54:15.000000 interaction_discord_bot-0.1.9/interaction_discord_bot/modal/speakModal.py
+drwxrwxr-x   0 appez     (1000) appez     (1000)        0 2024-04-30 18:26:38.330095 interaction_discord_bot-0.1.9/interaction_discord_bot.egg-info/
+-rw-r--r--   0 appez     (1000) appez     (1000)      156 2024-04-30 18:26:38.000000 interaction_discord_bot-0.1.9/interaction_discord_bot.egg-info/PKG-INFO
+-rw-rw-r--   0 appez     (1000) appez     (1000)      491 2024-04-30 18:26:38.000000 interaction_discord_bot-0.1.9/interaction_discord_bot.egg-info/SOURCES.txt
+-rw-rw-r--   0 appez     (1000) appez     (1000)        1 2024-04-30 18:26:38.000000 interaction_discord_bot-0.1.9/interaction_discord_bot.egg-info/dependency_links.txt
+-rw-rw-r--   0 appez     (1000) appez     (1000)        9 2024-04-30 18:26:38.000000 interaction_discord_bot-0.1.9/interaction_discord_bot.egg-info/requires.txt
+-rw-rw-r--   0 appez     (1000) appez     (1000)       24 2024-04-30 18:26:38.000000 interaction_discord_bot-0.1.9/interaction_discord_bot.egg-info/top_level.txt
+-rw-rw-r--   0 appez     (1000) appez     (1000)       38 2024-04-30 18:26:38.330095 interaction_discord_bot-0.1.9/setup.cfg
+-rw-rw-r--   0 appez     (1000) appez     (1000)      272 2024-04-11 19:50:14.000000 interaction_discord_bot-0.1.9/setup.py
```

### Comparing `interaction_discord_bot-0.1.4/interaction_discord_bot/message.py` & `interaction_discord_bot-0.1.9/interaction_discord_bot/cogs/message.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from nextcord.ext import commands
 from nextcord import slash_command
-
 from interaction_discord_bot.modal.speakModal import SpeakModal
 
+
 class Interaction(commands.Cog):
-    """Admin cmd"""
-    def __init__(self,bot):
+    """Message command for admin"""
+
+    def __init__(self, bot):
         self.bot = bot
 
-    
-    @slash_command(description="🎙️",dm_permission=False,default_member_permissions= 0)
-    async def speak(self, interaction, message : str = None):
+    @slash_command(description="🎙️", dm_permission=False, default_member_permissions=0)
+    async def speak(self, interaction, message: str = None):
         """Send a message in a channel"""
-        if message :
+        if message:
             try:
                 await interaction.channel.send(message)
-                await interaction.response.send_message("Message sent !",ephemeral=True)
-            except Exception as e:          
-                await interaction.response.send_message(f"Error : {e}",ephemeral=True)
-        else :
-            await interaction.response.send_modal(SpeakModal(self.bot,interaction.channel.id))
+                await interaction.response.send_message(
+                    "Message sent !", ephemeral=True
+                )
+            except Exception as e:
+                await interaction.response.send_message(f"Error : {e}", ephemeral=True)
+        else:
+            await interaction.response.send_modal(
+                SpeakModal(self.bot, interaction.channel.id)
+            )
+        
+def setup(bot):
+    bot.add_cog(Interaction(bot))
```

### Comparing `interaction_discord_bot-0.1.4/interaction_discord_bot/modal/speakModal.py` & `interaction_discord_bot-0.1.9/interaction_discord_bot/modal/speakModal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 from nextcord.ui import Modal, TextInput
 from nextcord import TextInputStyle
 
+
 class SpeakModal(Modal):
-    def __init__(self,bot, channel_id):
-        super().__init__('Speak Modal')
+    def __init__(self, bot, channel_id):
+        super().__init__("Speak Modal")
         self.bot = bot
 
-        self.channel_id = TextInput('Channel ID', placeholder='Channel ID',required=True, default_value=channel_id)
-        self.msg = TextInput('Message', placeholder='Message',required=True, style=TextInputStyle.paragraph)
+        self.channel_id = TextInput(
+            "Channel ID",
+            placeholder="Channel ID",
+            required=True,
+            default_value=channel_id,
+        )
+        self.msg = TextInput(
+            "Message",
+            placeholder="Message",
+            required=True,
+            style=TextInputStyle.paragraph,
+        )
 
         self.add_item(self.msg)
         self.add_item(self.channel_id)
 
     async def callback(self, interaction):
         try:
             channel_id = int(self.channel_id.value)
             text_channel = self.bot.get_channel(channel_id)
             await text_channel.send(self.msg.value)
-            return await interaction.response.send_message(f"Message sent in {text_channel.mention}",ephemeral=True)
-        except Exception as e:          
-            return await interaction.response.send_message(f"Error : {e}",ephemeral=True)
-            
+            return await interaction.response.send_message(
+                f"Message sent in {text_channel.mention}", ephemeral=True
+            )
+        except Exception as e:
+            return await interaction.response.send_message(
+                f"Error : {e}", ephemeral=True
+            )
```

