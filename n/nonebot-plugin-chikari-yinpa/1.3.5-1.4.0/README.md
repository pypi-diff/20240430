# Comparing `tmp/nonebot_plugin_chikari_yinpa-1.3.5.tar.gz` & `tmp/nonebot_plugin_chikari_yinpa-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chikari_yinpa-1.3.5.tar", last modified: Tue Mar 26 04:27:17 2024, max compression
+gzip compressed data, was "nonebot_plugin_chikari_yinpa-1.4.0.tar", last modified: Tue Apr 30 10:05:47 2024, max compression
```

## Comparing `nonebot_plugin_chikari_yinpa-1.3.5.tar` & `nonebot_plugin_chikari_yinpa-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 04:27:17.226733 nonebot_plugin_chikari_yinpa-1.3.5/
--rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_yinpa-1.3.5/LICENSE
--rw-rw-rw-   0        0        0     4734 2024-03-26 04:27:17.226733 nonebot_plugin_chikari_yinpa-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     4033 2024-03-16 14:39:20.000000 nonebot_plugin_chikari_yinpa-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 04:27:17.181424 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/
--rw-rw-rw-   0        0        0     2835 2024-03-26 04:25:41.000000 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/__init__.py
--rw-rw-rw-   0        0        0      684 2024-02-17 04:46:31.000000 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/config.py
--rw-rw-rw-   0        0        0     5987 2024-03-26 04:25:21.000000 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/data_handles.py
--rw-rw-rw-   0        0        0    15008 2024-03-16 15:42:31.000000 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/dicts.py
--rw-rw-rw-   0        0        0    36683 2024-03-26 04:23:31.000000 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/handles.py
--rw-rw-rw-   0        0        0    27338 2024-03-23 16:32:53.000000 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-26 04:27:17.225764 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa.egg-info/
--rw-rw-rw-   0        0        0     4734 2024-03-26 04:27:17.000000 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2024-03-26 04:27:17.000000 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 04:27:17.000000 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-03-26 04:27:17.000000 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-03-26 04:27:17.000000 nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-03-26 04:27:17.227759 nonebot_plugin_chikari_yinpa-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0      783 2024-03-26 04:25:36.000000 nonebot_plugin_chikari_yinpa-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:05:47.306381 nonebot_plugin_chikari_yinpa-1.4.0/
+-rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_yinpa-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     4734 2024-04-30 10:05:47.305405 nonebot_plugin_chikari_yinpa-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4033 2024-03-16 14:39:20.000000 nonebot_plugin_chikari_yinpa-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 10:05:47.297597 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/
+-rw-rw-rw-   0        0        0     2835 2024-04-30 10:05:25.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-02-17 04:46:31.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/config.py
+-rw-rw-rw-   0        0        0     6161 2024-04-30 09:36:41.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/data_handles.py
+-rw-rw-rw-   0        0        0    15078 2024-04-30 09:40:40.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/dicts.py
+-rw-rw-rw-   0        0        0    36824 2024-04-30 10:05:10.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/handles.py
+-rw-rw-rw-   0        0        0    27358 2024-04-30 09:41:35.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 10:05:47.304429 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/
+-rw-rw-rw-   0        0        0     4734 2024-04-30 10:05:47.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2024-04-30 10:05:47.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 10:05:47.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-30 10:05:47.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-04-30 10:05:47.000000 nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-30 10:05:47.307357 nonebot_plugin_chikari_yinpa-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      783 2024-04-30 10:05:28.000000 nonebot_plugin_chikari_yinpa-1.4.0/setup.py
```

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/LICENSE` & `nonebot_plugin_chikari_yinpa-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/PKG-INFO` & `nonebot_plugin_chikari_yinpa-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_yinpa
-Version: 1.3.5
+Version: 1.4.0
 Summary: A plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.3.5
+Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.4.0
 Summary: A plugin for nonebot 2 Home-page: https://github.com/mrqx0195/
 nonebot_plugin_chikari_yinpa Author: mrqx0195 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pillow Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
```

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/README.md` & `nonebot_plugin_chikari_yinpa-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/__init__.py` & `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     usage="",
     config=Config,
     type="application",
     homepage="https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa",
     supported_adapters={"~onebot.v11"}
 )
 
-__version__ = "1.3.5"
+__version__ = "1.4.0"
 
 on_yinpa_control = on_command(
     "yinpa_control",
     aliases={"银趴控制"},
     permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
     priority=10,
     block=False,
```

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/config.py` & `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/data_handles.py` & `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/data_handles.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 if not os.path.exists(plugin_data_file):
     f = open(plugin_data_file,'w')
     f.close
 with open(plugin_data_file,encoding='utf-8')as datafile:
     datastr = datafile.read()
     if not os.path.exists(plugin_data_file) or not datastr:
         f = open(plugin_data_file,'w')
-        init_data = {}
+        init_data = {
+            
+        }
         json.dump(init_data,f,indent=4)
         f.close
         data = init_data
     else:
         data = json.loads(datastr,strict=False)
         
 #配置数据文件初始化及载入
@@ -66,66 +68,71 @@
         Args:
             uid (str): 用户id
             key (str): 数据键值
             value (_type_): 数据
         """
         
         global data
+        DHandles.file_save()
         data[uid][key] = value
         DHandles.file_save()
         return
     
     def configdata_set(key: str,value):
         """设置配置文件
 
         Args:
             key (str): 配置键值
             value (_type_): 数据
         """
         
         global configdata
+        DHandles.file_save()
         configdata[key] = value
         DHandles.file_save()
         return
     
     def group_remove(group_id: int):
         """将群组移出银趴
 
         Args:
             group_id (int): 群组id
         """
         
         global configdata
+        DHandles.file_save()
         configdata["yinpa_enabled_group"].remove(group_id)
         DHandles.file_save()
         return
     
     def user_add(uid: str,dict: dict):
         """将用户加入银趴
 
         Args:
             uid (str): 用户id
             dict (dict): 用户初始数据
         """
         
         global data
+        DHandles.file_save()
         data[uid] = dict
         data[uid]["hp_v"] = (data[uid]["volition"] + 10) * 5
         data[uid]["hp_c"] = (data[uid]["constitution"] + 10) * 10
         DHandles.file_save()
         return
         
     def user_remove(uid: str):
         """将用户移出银趴
 
         Args:
             uid (str): 用户id
         """
         
         global data
+        DHandles.file_save()
         del data[uid]
         DHandles.file_save()
         return
     
     def skill_refresh(uid: str,id: int,value = None,level: int = 1,mode: str = ''):
         """更新技能
```

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/dicts.py` & `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/dicts.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     """银趴常量字典
     """
     
     yinpa_help_dict = {
         "":"Chikari_yinpa 模块帮助\n加入银趴：/yinpa_join <银趴昵称> <银趴种族>\n种族列表：/yinpa_help 种族\n技能列表：/yinpa_help 技能\n状态列表：/yinpa_help 状态\n查询个人信息：/info\n签到：/sign_in\n商店：/shop\n工作：/work",
         "help":"help\n命令：/help [参数]\n命令别称：/银趴帮助\n查询Chikari_yinpa的帮助",
         "sign_in":"sign_in\n命令：/sign_in\n命令别称：/签到 /打卡\n每日打卡，每天可使用一次，增加长度、深度、金钱",
-        "yinpa_join":"join_yinpa\n命令：/yinpa_join <银趴昵称> <银趴种族>\n命令别称：/加入银趴\n加入银趴！\n种族列表参照： /yinpa_help 种族",
+        "yinpa_join":"join_yinpa\n命令：/yinpa_join [银趴昵称] [银趴种族]\n命令别称：/加入银趴\n加入银趴！\n种族列表参照： /yinpa_help 种族\n昵称留空则直接使用群昵称\n种族留空则为随机种族",
         "yinpa_leave":"yinpa_leave\n命令：/yinpa_leave [key]\n命令别称：/离开银趴\n离开银趴！\n首次输入时会返回一个key码，需再次发送带key的命令才能离开",
         "yinpa_control":"yinpa_control\n命令：/yinpa_control <enable/disable>\n命令别称：/银趴控制\n控制本群银趴的开启/关闭",
         "info":"info\n命令：/info [@某人]\n命令别称：/信息 /查询\n查询自己或某人的银趴信息",
         "tou":"tou\n命令：/tou <@某人 或 银趴昵称>\n命令别称：/透 /插入\n透某人",
         "zha":"zha\n命令：/zha <@某人 或 银趴昵称>\n命令别称：/榨 /榨精\n榨某人",
         "chong":"chong\n命令：/chong\n命令别称：/冲 /打胶 /手冲 /撸 /导\n冲一发，能够增加或减少一定长度",
         "kou":"kou\n命令：/kou\n命令别称：/扣 /扣扣 /自慰 /紫薇\n扣一次，能够增加少量深度",
```

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/handles.py` & `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/handles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from nonebot.adapters.onebot.v11 import GroupMessageEvent,Message,MessageSegment
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg
-from nonebot import get_driver,get_plugin_config
+from nonebot import get_driver,get_plugin_config,get_bots
 from time import time
 from hashlib import md5
 from math import sqrt
 
 from .data_handles import data,configdata,DHandles
 from .config import Config
 from .utils import Utils
@@ -39,15 +39,15 @@
         """处理签到
         """
         
         if not Utils.group_enable_check(event.group_id):
             await matcher.finish("本群银趴已禁用")
         if not Utils.yinpa_user_presence_check(event.get_user_id()):
             await matcher.finish("您还未加入银趴！\ntips：请使用 /yinpa_join 或 /加入银趴 加入银趴")
-        uid: str=event.get_user_id()
+        uid: str = event.get_user_id()
         if data[uid]["last_sign_in_time"] < (int)(time() / 86400):
             DHandles.data_set(uid,"last_sign_in_time",(int)(time() / 86400))
             d_pl = Utils.dice(100,(int)(data[uid]['penis_length']) ^ 1)
             d_vd = Utils.dice(100,(int)(data[uid]['vagina_depth']) ^ 2)
             d_m = Utils.dice(100,(int)(data[uid]['money']) ^ 3)
             await matcher.send(f"{data[uid]['name']}签到成功\n长度增加：{data[uid]['penis_length']} + (1d100 / 100) = {data[uid]['penis_length']} + ({d_pl} / 100) = {round(data[uid]['penis_length'] + d_pl / 100,2)}\n深度增加：{data[uid]['vagina_depth']} + (1d100 / 100) = {data[uid]['vagina_depth']} + ({d_vd} / 100) = {round(data[uid]['vagina_depth'] + d_vd / 100,2)}\n金钱增加：{data[uid]['money']} + 1d100 = {data[uid]['money']} + {d_m} = {data[uid]['money'] + d_m}\nps：签到于早上8点刷新")
             DHandles.data_set(uid,'penis_length',round(data[uid]['penis_length'] + d_pl / 100,2))
@@ -63,23 +63,28 @@
         """处理加入银趴
         """
         
         if not Utils.group_enable_check(event.group_id):
             await matcher.finish("本群银趴已禁用，你不准参加银趴！")
         if Utils.yinpa_user_presence_check(event.get_user_id()):
             await matcher.finish("您已加入银趴！\n如果想要重置银趴数据，请使用 /leave_yinpa 或 /离开银趴 离开银趴后再加入")
-        uid: str=event.get_user_id()
+        uid: str = event.get_user_id()
         command: str = args.extract_plain_text()
         arg_list: list = command.split()
         if not len(arg_list) == 2:
-            await matcher.finish("参数错误！\n格式： /yinpa_join <银趴昵称> <银趴种族> \n种族列表参照： /yinpa_help 种族 ")
-        if not arg_list[1].isdigit() or (int)(arg_list[1]) <= 0:
-            await matcher.finish("参数错误！\n种族应为一个正整数（种族编号）\n种族列表参照： /yinpa_help 种族 ")
-        name: str = arg_list[0]
-        species: int = (int)(arg_list[1])
+            bot = get_bots()[event.self_id]
+            name: str = bot.call_api("get_group_member_info",group_id = event.group_id,user_id = uid)["nickname"]
+        else:
+            name: str = arg_list[0]
+        if (int)(arg_list[1]) <= 0:
+            species: int = Utils.dice(7,event.get_user_id())
+        else:
+            if not arg_list[1].isdigit():
+                await matcher.finish("参数错误！\n种族应为一个正整数（种族编号）\n种族列表参照： /yinpa_help 种族 ")
+            species: int = (int)(arg_list[1])
         if not dicts.species_dict.get(species):
             await matcher.finish("参数错误！\n不存在指定的种族\n种族列表参照： /yinpa_help 种族 ")
         if Utils.find_user_name(name):
             await matcher.finish("已经有人使用这个昵称了！")
         DHandles.user_add(uid,{
             'name':name,
             'species':species,
```

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa/utils.py` & `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             skill_text = '无'
         for i in user_data["state"]:
             state_text += dicts.state_dict[i[0]] + f'（等级：{i[2]}）（剩余时间：{(int)(i[1] - time())}秒）' + '；'
         if not state_text:
             state_text = '无'
         text = f"    ID：{uid}\n"\
         f"    昵称：{user_data['name']}\n"\
-        f"    种族：{user_data['species']}\n"\
+        f"    种族：{dicts.species_dict[user_data['species']]}\n"\
         f"    意志HP：{user_data['hp_v']}\n"\
         f"    体质HP：{user_data['hp_c']}\n"\
         f"    长度：{user_data['penis_length']}\n"\
         f"    深度：{user_data['vagina_depth']}\n"\
         f"    力量：{user_data['strength']}（当前：{Utils.get_value(uid,'strength')[0]}）\n"\
         f"    体质：{user_data['constitution']}（当前：{Utils.get_value(uid,'constitution')[0]}）\n"\
         f"    技巧：{user_data['technique']}（当前：{Utils.get_value(uid,'technique')[0]}）\n"\
```

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO` & `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_yinpa
-Version: 1.3.5
+Version: 1.4.0
 Summary: A plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.3.5
+Metadata-Version: 2.1 Name: nonebot_plugin_chikari_yinpa Version: 1.4.0
 Summary: A plugin for nonebot 2 Home-page: https://github.com/mrqx0195/
 nonebot_plugin_chikari_yinpa Author: mrqx0195 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pillow Requires-Dist: nonebot2>=2.2.0 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
```

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt` & `nonebot_plugin_chikari_yinpa-1.4.0/nonebot_plugin_chikari_yinpa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_yinpa-1.3.5/setup.py` & `nonebot_plugin_chikari_yinpa-1.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_chikari_yinpa",
-    version="1.3.5",
+    version="1.4.0",
     author="mrqx0195",
     author_email="2317249571@qq.com",
     description="A plugin for nonebot 2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrqx0195/nonebot_plugin_chikari_yinpa",
     packages=setuptools.find_packages(),
```

