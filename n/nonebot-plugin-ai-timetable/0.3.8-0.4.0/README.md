# Comparing `tmp/nonebot_plugin_ai_timetable-0.3.8.tar.gz` & `tmp/nonebot_plugin_ai_timetable-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ai_timetable-0.3.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_ai_timetable-0.4.0.tar", max compression
```

## Comparing `nonebot_plugin_ai_timetable-0.3.8.tar` & `nonebot_plugin_ai_timetable-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-04-28 11:46:30.776628 nonebot_plugin_ai_timetable-0.3.8/LICENSE
--rw-r--r--   0        0        0     8925 2024-04-28 11:46:30.776628 nonebot_plugin_ai_timetable-0.3.8/README.md
--rw-r--r--   0        0        0    12197 2024-04-28 11:46:30.776628 nonebot_plugin_ai_timetable-0.3.8/nonebot_plugin_ai_timetable/__init__.py
--rw-r--r--   0        0        0      339 2024-04-28 11:46:30.776628 nonebot_plugin_ai_timetable-0.3.8/nonebot_plugin_ai_timetable/config.py
--rw-r--r--   0        0        0    20688 2024-04-28 11:46:30.776628 nonebot_plugin_ai_timetable-0.3.8/nonebot_plugin_ai_timetable/utils.py
--rw-r--r--   0        0        0      511 2024-04-28 11:46:30.776628 nonebot_plugin_ai_timetable-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     9692 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/LICENSE
+-rw-r--r--   0        0        0    10826 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/README.md
+-rw-r--r--   0        0        0     6237 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/__init__.py
+-rw-r--r--   0        0        0      332 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/config.py
+-rw-r--r--   0        0        0     6420 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/data_manager.py
+-rw-r--r--   0        0        0     9714 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/manager.py
+-rw-r--r--   0        0        0     2799 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/migrations/f67eb52d6a0f_init.py
+-rw-r--r--   0        0        0     1774 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/model.py
+-rw-r--r--   0        0        0     8203 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/nonebot_plugin_ai_timetable/reminder.py
+-rw-r--r--   0        0        0      549 2024-04-30 13:28:16.527808 nonebot_plugin_ai_timetable-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11637 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_ai_timetable-0.3.8/LICENSE` & `nonebot_plugin_ai_timetable-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ai_timetable-0.3.8/README.md` & `nonebot_plugin_ai_timetable-0.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+  <a href="https://nonebot.dev/"><img src="https://nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
 
 # nonebot-plugin-ai-timetable
 
 ✨*基于Nonebot2的对接小爱课程表的插件*✨
   
@@ -19,31 +19,33 @@
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 <div align="left">
 
 ## 💿安装
 
 1. 通过`pip`或`nb`安装；
-    - 使用nb(极度推荐)
+    - 使用nb(推荐)
   
        在机器人目录下命令行使用`nb plugin install nonebot_plugin_ai_timetable`
 
     - 使用pip:
   
       `pip plugin install nonebot_plugin_ai_timetable`
 
       然后在机器人`pyproject.toml`里的`plugins = []`列表追加`"nonebot_plugin_ai_timetable"`
 
-2. 本地数据保存在`data/ai_timetable/userdata.json`以及`data/ai_timetable/usertable.json`，分别对应用户发送的链接和本地保存的课表
+2. 数据存储使用[plugin-orm](https://github.com/nonebot/plugin-orm), 接入数据库，方便管理
+
+3. 第一次使用使用[plugin-orm](https://github.com/nonebot/plugin-orm)时，需要用`nb orm upgrade`升级数据库
 
 ## 📖简介
 
 1. 傻瓜式一键导入小爱课表，让你的bot实现小爱课表的功能
 
-2. 用户课表数据隔离，无需担心课程时间冲突、不同学校课表不同等问题
+2. 用户课表数据隔离，基于[plugin-rom](https://github.com/nonebot/plugin-orm), 接入数据库，无需担心课程时间冲突、不同学校课表不同等问题
 
 3. 适配多平台，即使是电报涩涩群也要好好学习！🥵🥵
 
 ## ⚙️插件配置
 
 这些配置都已设好默认值，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项(可选)
 
@@ -51,25 +53,37 @@
 | :---------------------: | :---: | :-----: | :------------------------: | :---------------------------------------------------------------------------------------------------- |
 |      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                                   |
 | TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                                              |
 |    TIMETABLE_ALOCK_8    |  int  |   21    |    TIMETABLE_ALOCK_8=16    | 订阅早八的发送时间，必须是0-24的数字.这里发送的都是第二天的，所以建议设置为18-23点                    |
 |   TIMETABLE_SEND_TIME   | float |   0.5   |   TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
 
 ## 💿依赖
-
+插件依赖会在安装时自动安装，如果安装失败，你可以按照以下指令手动再次安装
 ```python
 nb plugin install nonebot_plugin_htmlrender
 nb plugin install nonebot_plugin_apscheduler
 nb plugin install nonebot_plugin_alconna
+nb plugin install nonebot_plugin_orm
 ```
+
 ## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
+- 0.4.0 / 2024-04-30:
+   1. 重构完成，将所有数据迁移到官方数据库插件[plugin-orm](https://github.com/nonebot/plugin-orm)，之前的数据失效
+   2. 修改了插件触发指令和相关逻辑
+   3. 重构所有代码，优化处理逻辑
+   >该版本是破坏性更新，且仍在测试中，有任何疑问欢迎issue或pr
+
+- 0.3.8 / 2024-04-28:
+   1. 修复设置错误
+   2. 重构代码
+
 - 0.3.7 / 2024-04-24:
    1. 更新Nonebot2版本至2.2.0
    2. 基于 [nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna) 适配多平台
    3. 放宽httpx限制，移除onebot依赖
 
 - 0.3.6 / 2023-09-02:
    1. 适配nonebot2.0.1版本：移除过时的RegexMatch方法
@@ -125,52 +139,48 @@
 - 0.1.4 / 2023-03-05:
    1. 修复了无法取消订阅早八的bug
 
 </details>
 
 ## 🎉命令
 
-1. 我的课表|小爱课表|本周课表|下周课表：获取本周|下周的完全课表，使用前须先导入课表，这里的课表是在线课表
+1. 课表帮助：获取本条帮助
 
 2. 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
 
     ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 
     在基本设置里把开始上课时间等调整好之后(尤其是时间、节数)，把分享课表得到的链接发送给bot即可导入本地(分享前需要登录小米账户 [#1](https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1))
 
 3. 更新课表；如果在小爱课程表里修改了课程，发送该条指令即可更新本地的课表，无需重新导入
   
-4. (昨天|今天|明天|后天|周X|星期x|)(课表|有啥课|上啥课)：查询指定天的课表，其中查询周x课表查询的是本周的
-
-5. 订阅|取消订阅某天课表：导入本地课表后，发送订阅xx课表，如`订阅周一课表`，就可以在这天的前一天晚上10点(可修改)定时推送第二天要上的课
+4. 查询课表+[参数]：查询[参数]的课表，参数支持[本周/下周、周x、昨天/今天/明天/后天、早八、课程名]
 
-6. 订阅|取消订阅早八：会让bot在前一天晚上9点(可修改)提醒你第二天是否有早八，以便决定今晚是否嗨皮（判定依据是是否存在第一节课）
+5. 添加课程提醒+[参数]：参数支持[周x、早八、课程名]
 
-7. 订阅|取消订阅课程 xxx：订阅课程后，会让bot在所有名称里包含xxx的课程开始前0.5小时(可修改)发送提醒，如订阅课程 数学分析，则数学分析和数学分析习题课的课前0.5小时会自动发出提醒
+6. 删除课程提醒+[参数]：参数支持[全部、周x、早八、课程名]
 
-8. 上课|下节课：获取当前上课信息，返回下节课信息(如果有)
+7. 查看课程提醒：查看当前已经添加的课程提醒
 
-9. 早八|明日早八：查询明天的早八
-
-10. 课表帮助：获取课表帮助
-
-未完待续
 
 ## ⭐效果图
 
-![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/my_table.jpg)
-![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/alock_8.jpg)
-![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/next_class.jpg)
-![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/someday_classes.jpg)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/update.png)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query.png)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder.png)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder1.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/someday_classes_pic.jpg)
 
 ### 关于小爱课程表内的一些说明
 
 如下图
 
+- 第一次使用本插件时，需要用`nb orm upgrade`升级数据库
 - 首先要登录上小米账户,否则可能获取到错误的课表信息 [#1](https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1)
 - 设置好开始上课时间
 - 设置好课程时间，可以修改每节课具体的时间，
 - 课表节数按自己需求调，一般教务导入的课表节数可能不符合实际，需要微调
 - 每周起始日建议默认的周一即可（周日起始没测试过可能有bug）
 - 如果导入课表后在小爱课表内修改了课程，直接给bot发送更新课表即可更新本地课表
 - 当你主页的课表和学校课表基本一致时，那么小爱课程表就被调教好了，可以导入了
@@ -187,22 +197,36 @@
 
 - [x] 重构代码
 
 - [x] 订阅指定的课
 
 - [x] 多平台适配, 基于 [nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna) 
 
-- [ ] 支持定时任务本地存储
+- [x] 支持定时任务本地存储
 
-- [ ] 适配[plugin-rom](https://github.com/nonebot/plugin-orm), 接入数据库
+- [x] 适配[plugin-orm](https://github.com/nonebot/plugin-orm), 接入数据库
 
 - [ ] 适配更多课表、脱离小爱课表
 
 - [ ] 完善插件
 
 ## 🐛存在的问题
 
- 1. 小爱课表分享的链接大概2周后会过期，会使得`我的课表\下周课表`无法使用，需要重新分享，但是仍能使用本地课表，也可以更新本地课表
+ ### 关于定时任务的持久化存储问题：
+
+众所周知，使用apscheduler添加的定时任务，会在bot重启后丢失，这是因为使用[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的scheduler，默认使用的JobStore(即保存任务的方式)，是MemoryJobStore，也就是存在内存中，因此会导致重启丢任务。
+
+因此参考[apscheduler](https://apscheduler.readthedocs.io/en/latest/userguide.html#configuring-the-scheduler)，你可以在bot的配置文件中添加配置项，让[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的scheduler的默认 JobStore 改为使用数据库，这样就可以持久化存储任务，而不需要额外修改任何东西。
+
+然而，很不幸的是，在apscheduler4.0版本之前，所支持的数据库类JobStore都是使用**同步**引擎的，然而[plugin-orm](https://github.com/nonebot/plugin-orm)所采用的是异步引擎，因此你暂时还不能这样做。
 
- 2. 机器人重启后定时任务会丢失
+所以，暂时还无法解决定时任务的持久化存储问题，除非apscheduler正式发版4.0（目前还是alpha版本），你可以再等待，本插件会持续跟进更新。
 
-## 喜欢的话就点个star✨吧QAQ
+## 🎉致谢
+- 感谢[nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender)提供的渲染工具
+- 感谢[plugin-orm](https://github.com/nonebot/plugin-orm)提供的异步数据库接口
+- 感谢[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)提供的定时任务接口
+- 感谢[nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna)
+- 感谢[Matcha](https://github.com/A-kirami/matcha)提供的简单好用的测试平台
+### 喜欢的话就点个star✨吧
+或者, 你也可以看我写的其他插件
+[nonebot-plugin-manga-translator](https://github.com/maoxig/nonebot-plugin-manga-translator)一个支持多api, 方便好用的图片/漫画翻译插件
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
                                    _[_n_o_n_e_b_o_t_]
                          # nonebot-plugin-ai-timetable
 â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨_[_n_o_n_e_b_o_t_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
-## ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
+## ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æ¨è)
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨`nb plugin install
 nonebot_plugin_ai_timetable` - ä½¿ç¨pip: `pip plugin install
 nonebot_plugin_ai_timetable` ç¶åå¨æºå¨äºº`pyproject.toml`éç`plugins =
-[]`åè¡¨è¿½å `"nonebot_plugin_ai_timetable"` 2. æ¬å°æ°æ®ä¿å­å¨`data/
-ai_timetable/userdata.json`ä»¥å`data/ai_timetable/
-usertable.json`ï¼åå«å¯¹åºç¨æ·åéçé¾æ¥åæ¬å°ä¿å­çè¯¾è¡¨ ##
-ðç®ä» 1.
+[]`åè¡¨è¿½å `"nonebot_plugin_ai_timetable"` 2. æ°æ®å­å¨ä½¿ç¨[plugin-
+orm](https://github.com/nonebot/plugin-orm), æ¥å¥æ°æ®åºï¼æ¹ä¾¿ç®¡ç 3.
+ç¬¬ä¸æ¬¡ä½¿ç¨ä½¿ç¨[plugin-orm](https://github.com/nonebot/plugin-
+orm)æ¶ï¼éè¦ç¨`nb orm upgrade`åçº§æ°æ®åº ## ðç®ä» 1.
 å»çå¼ä¸é®å¯¼å¥å°ç±è¯¾è¡¨ï¼è®©ä½ çbotå®ç°å°ç±è¯¾è¡¨çåè½ 2.
-ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
+ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼åºäº[plugin-rom](https://github.com/nonebot/
+plugin-orm),
+æ¥å¥æ°æ®åºï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
 3. ééå¤å¹³å°ï¼å³ä½¿æ¯çµæ¥æ¶©æ¶©ç¾¤ä¹è¦å¥½å¥½å­¦ä¹ ï¼ð¥µð¥µ ##
 âï¸æä»¶éç½®
 è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹
 (å¯é) | config | type | default | example | usage | | :--------------------
 -: | :---: | :-----: | :------------------------: | :--------------------------
 -------------------------------------------------------------------------- | |
 TIMETABLE_PIC | bool | true | TIMETABLE_PIC=false |
@@ -23,18 +25,26 @@
 TIMETABLE_ALOCK_SOMEDAY | int | 22 | TIMETABLE_ALOCK_SOMEDAY=15 |
 è®¢éææ¥è¯¾è¡¨çåéæ¶é´ï¼å¿é¡»æ¯0-24çæ°å­ | |
 TIMETABLE_ALOCK_8 | int | 21 | TIMETABLE_ALOCK_8=16 |
 è®¢éæ©å«çåéæ¶é´ï¼å¿é¡»æ¯0-
 24çæ°å­.è¿éåéçé½æ¯ç¬¬äºå¤©çï¼æä»¥å»ºè®®è®¾ç½®ä¸º18-23ç¹ |
 | TIMETABLE_SEND_TIME | float | 0.5 | TIMETABLE_SEND_TIME=1 |
 è®¢éè¯¾ç¨æååéçæ¶é´ï¼åä½æ¯`å°æ¶`ï¼å¯ä»¥æ¯æ´æ°ä¹å¯ä»¥æ¯å°æ°ï¼å»ºè®®ä¸è¦è®¾çå¤ªå¤§ï¼é¿ååºç°æ æ³é¢æçbug
-| ## ð¿ä¾èµ ```python nb plugin install nonebot_plugin_htmlrender nb plugin
-install nonebot_plugin_apscheduler nb plugin install nonebot_plugin_alconna ```
-## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 0.3.7 / 2024-04-24: 1.
-æ´æ°Nonebot2çæ¬è³2.2.0 2. åºäº [nonebot-plugin-alconna](https://
+| ## ð¿ä¾èµ
+æä»¶ä¾èµä¼å¨å®è£æ¶èªå¨å®è£ï¼å¦æå®è£å¤±è´¥ï¼ä½ å¯ä»¥æç§ä»¥ä¸æä»¤æå¨åæ¬¡å®è£
+```python nb plugin install nonebot_plugin_htmlrender nb plugin install
+nonebot_plugin_apscheduler nb plugin install nonebot_plugin_alconna nb plugin
+install nonebot_plugin_orm ``` ## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 0.4.0 / 2024-
+04-30: 1. éæå®æï¼å°æææ°æ®è¿ç§»å°å®æ¹æ°æ®åºæä»¶[plugin-
+orm](https://github.com/nonebot/plugin-orm)ï¼ä¹åçæ°æ®å¤±æ 2.
+ä¿®æ¹äºæä»¶è§¦åæä»¤åç¸å³é»è¾ 3.
+éæææä»£ç ï¼ä¼åå¤çé»è¾
+>è¯¥çæ¬æ¯ç ´åæ§æ´æ°ï¼ä¸ä»å¨æµè¯ä¸­ï¼æä»»ä½çé®æ¬¢è¿issueæpr
+- 0.3.8 / 2024-04-28: 1. ä¿®å¤è®¾ç½®éè¯¯ 2. éæä»£ç  - 0.3.7 / 2024-04-
+24: 1. æ´æ°Nonebot2çæ¬è³2.2.0 2. åºäº [nonebot-plugin-alconna](https://
 github.com/nonebot/plugin-alconna) ééå¤å¹³å° 3.
 æ¾å®½httpxéå¶ï¼ç§»é¤onebotä¾èµ - 0.3.6 / 2023-09-02: 1.
 éénonebot2.0.1çæ¬ï¼ç§»é¤è¿æ¶çRegexMatchæ¹æ³
 >å¦æ´æ°æ¬æä»¶åæ¥åæ¶æ¯æ ååºï¼è¯·æ´æ°ä½ çnonebotçæ¬æåéå°æ§çæ¬ä½¿ç¨
 - 0.3.5 / 2023-08-10: 1. æ ¼å¼åä»£ç  2. ä¼åéç½®è¯»å 3.
 æ´æ°æä»¶åæ°æ® - 0.3.5 / 2023-06-09: 1. æ´æ°httpxä¾èµçæ¬ - 0.3.3
 / 2023-04-23: 1. ä¿®å¤å®æ¶æééå¤åéçbug 2. ä¿®æ¹å¸®å© - 0.3.2 /
@@ -52,46 +62,39 @@
 - 0.1.8 / 2023-03-08: 1. ä¿®æ¹é¨åä»£ç ï¼ä¼åè¯¾è¡¨æ ¼å¼ 2.
 ä¿®å¤äºèæ°ä¸º11çè¯¾ä¼æå¨èæ°ä¸º2çè¯¾ç¨åé¢çbug
 (QAQå¤ªè ¢äºå«éªäºå«éªäº) - 0.1.7 / 2023-03-07: 1.
 ä¿®å¤äºæ¶é´ä¸ä¼èªå·±æ¹åçbug 2. æ°å¢äºä¸è¯¾/ä¸èè¯¾åè½ 3.
 ä¼åäºä¸äºå±å±±ä»£ç  - 0.1.5 / 2023-03-06: 1.
 æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 0.1.4 / 2023-03-05: 1.
 ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug ## ðå½ä»¤ 1.
-æçè¯¾è¡¨|å°ç±è¯¾è¡¨|æ¬å¨è¯¾è¡¨|ä¸å¨è¯¾è¡¨ï¼è·åæ¬å¨|ä¸å¨çå®å¨è¯¾è¡¨ï¼ä½¿ç¨åé¡»åå¯¼å¥è¯¾è¡¨ï¼è¿éçè¯¾è¡¨æ¯å¨çº¿è¯¾è¡¨
-2.
+è¯¾è¡¨å¸®å©ï¼è·åæ¬æ¡å¸®å© 2.
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
 (åäº«åéè¦ç»å½å°ç±³è´¦æ· [#1](https://github.com/maoxig/nonebot-
 plugin-ai-timetable/issues/1)) 3.
 æ´æ°è¯¾è¡¨ï¼å¦æå¨å°ç±è¯¾ç¨è¡¨éä¿®æ¹äºè¯¾ç¨ï¼åéè¯¥æ¡æä»¤å³å¯æ´æ°æ¬å°çè¯¾è¡¨ï¼æ ééæ°å¯¼å¥
-4. (æ¨å¤©|ä»å¤©|æå¤©|åå¤©|å¨X|ææx|)
-(è¯¾è¡¨|æå¥è¯¾|ä¸å¥è¯¾)ï¼æ¥è¯¢æå®å¤©çè¯¾è¡¨ï¼å¶ä¸­æ¥è¯¢å¨xè¯¾è¡¨æ¥è¯¢çæ¯æ¬å¨ç
-5.
-è®¢é|åæ¶è®¢éæå¤©è¯¾è¡¨ï¼å¯¼å¥æ¬å°è¯¾è¡¨åï¼åéè®¢éxxè¯¾è¡¨ï¼å¦`è®¢éå¨ä¸è¯¾è¡¨`ï¼å°±å¯ä»¥å¨è¿å¤©çåä¸å¤©æä¸10ç¹
-(å¯ä¿®æ¹)å®æ¶æ¨éç¬¬äºå¤©è¦ä¸çè¯¾ 6.
-è®¢é|åæ¶è®¢éæ©å«ï¼ä¼è®©botå¨åä¸å¤©æä¸9ç¹
-(å¯ä¿®æ¹)æéä½ ç¬¬äºå¤©æ¯å¦ææ©å«ï¼ä»¥ä¾¿å³å®ä»ææ¯å¦å¨ç®ï¼å¤å®ä¾æ®æ¯æ¯å¦å­å¨ç¬¬ä¸èè¯¾ï¼
-7. è®¢é|åæ¶è®¢éè¯¾ç¨
-xxxï¼è®¢éè¯¾ç¨åï¼ä¼è®©botå¨ææåç§°éåå«xxxçè¯¾ç¨å¼å§å0.5å°æ¶
-(å¯ä¿®æ¹)åéæéï¼å¦è®¢éè¯¾ç¨
-æ°å­¦åæï¼åæ°å­¦åæåæ°å­¦åæä¹ é¢è¯¾çè¯¾å0.5å°æ¶ä¼èªå¨ååºæé
-8. ä¸è¯¾|ä¸èè¯¾ï¼è·åå½åä¸è¯¾ä¿¡æ¯ï¼è¿åä¸èè¯¾ä¿¡æ¯
-(å¦ææ) 9. æ©å«|ææ¥æ©å«ï¼æ¥è¯¢æå¤©çæ©å« 10.
-è¯¾è¡¨å¸®å©ï¼è·åè¯¾è¡¨å¸®å© æªå®å¾ç»­ ## â­ææå¾ ![Image text]
+4. æ¥è¯¢è¯¾è¡¨+[åæ°]ï¼æ¥è¯¢[åæ°]çè¯¾è¡¨ï¼åæ°æ¯æ[æ¬å¨/
+ä¸å¨ãå¨xãæ¨å¤©/ä»å¤©/æå¤©/åå¤©ãæ©å«ãè¯¾ç¨å] 5.
+æ·»å è¯¾ç¨æé+[åæ°]ï¼åæ°æ¯æ[å¨xãæ©å«ãè¯¾ç¨å] 6.
+å é¤è¯¾ç¨æé+[åæ°]ï¼åæ°æ¯æ[å¨é¨ãå¨xãæ©å«ãè¯¾ç¨å]
+7. æ¥çè¯¾ç¨æéï¼æ¥çå½åå·²ç»æ·»å çè¯¾ç¨æé ## â­ææå¾
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
+resource/update.png) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
+timetable/blob/main/resource/query.png) ![Image text](https://github.com/
+maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png) ![Image text]
 (https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
-my_table.jpg) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
-timetable/blob/main/resource/alock_8.jpg) ![Image text](https://github.com/
-maoxig/nonebot-plugin-ai-timetable/blob/main/resource/next_class.jpg) ![Image
+query1.png) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
+timetable/blob/main/resource/reminder.png) ![Image text](https://github.com/
+maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder1.png) ![Image
 text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
-someday_classes.jpg) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
-timetable/blob/main/resource/someday_classes_pic.jpg) ###
-å³äºå°ç±è¯¾ç¨è¡¨åçä¸äºè¯´æ å¦ä¸å¾ -
+someday_classes_pic.jpg) ### å³äºå°ç±è¯¾ç¨è¡¨åçä¸äºè¯´æ å¦ä¸å¾
+- ç¬¬ä¸æ¬¡ä½¿ç¨æ¬æä»¶æ¶ï¼éè¦ç¨`nb orm upgrade`åçº§æ°æ®åº -
 é¦åè¦ç»å½ä¸å°ç±³è´¦æ·,å¦åå¯è½è·åå°éè¯¯çè¯¾è¡¨ä¿¡æ¯ [#1]
 (https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1) -
 è®¾ç½®å¥½å¼å§ä¸è¯¾æ¶é´ -
 è®¾ç½®å¥½è¯¾ç¨æ¶é´ï¼å¯ä»¥ä¿®æ¹æ¯èè¯¾å·ä½çæ¶é´ï¼ -
 è¯¾è¡¨èæ°æèªå·±éæ±è°ï¼ä¸è¬æå¡å¯¼å¥çè¯¾è¡¨èæ°å¯è½ä¸ç¬¦åå®éï¼éè¦å¾®è°
 -
 æ¯å¨èµ·å§æ¥å»ºè®®é»è®¤çå¨ä¸å³å¯ï¼å¨æ¥èµ·å§æ²¡æµè¯è¿å¯è½æbugï¼
@@ -99,15 +102,36 @@
 å¦æå¯¼å¥è¯¾è¡¨åå¨å°ç±è¯¾è¡¨åä¿®æ¹äºè¯¾ç¨ï¼ç´æ¥ç»botåéæ´æ°è¯¾è¡¨å³å¯æ´æ°æ¬å°è¯¾è¡¨
 -
 å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è°æå¥½äºï¼å¯ä»¥å¯¼å¥äº
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
 resource/settings.jpg) ## ð¦è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
 å¯éæ©æ¯å¦åéå¾çä»¥é¿åé£æ§ - [x] å¢å æ´å¤çéç½®é¡¹ - [x]
 éæä»£ç  - [x] è®¢éæå®çè¯¾ - [x] å¤å¹³å°éé, åºäº [nonebot-
-plugin-alconna](https://github.com/nonebot/plugin-alconna) - [ ]
-æ¯æå®æ¶ä»»å¡æ¬å°å­å¨ - [ ] éé[plugin-rom](https://github.com/
+plugin-alconna](https://github.com/nonebot/plugin-alconna) - [x]
+æ¯æå®æ¶ä»»å¡æ¬å°å­å¨ - [x] éé[plugin-orm](https://github.com/
 nonebot/plugin-orm), æ¥å¥æ°æ®åº - [ ]
 ééæ´å¤è¯¾è¡¨ãè±ç¦»å°ç±è¯¾è¡¨ - [ ] å®åæä»¶ ##
-ðå­å¨çé®é¢ 1.
-å°ç±è¯¾è¡¨åäº«çé¾æ¥å¤§æ¦2å¨åä¼è¿æï¼ä¼ä½¿å¾`æçè¯¾è¡¨\ä¸å¨è¯¾è¡¨`æ æ³ä½¿ç¨ï¼éè¦éæ°åäº«ï¼ä½æ¯ä»è½ä½¿ç¨æ¬å°è¯¾è¡¨ï¼ä¹å¯ä»¥æ´æ°æ¬å°è¯¾è¡¨
-2. æºå¨äººéå¯åå®æ¶ä»»å¡ä¼ä¸¢å¤± ##
-åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§QAQ
+ðå­å¨çé®é¢ ### å³äºå®æ¶ä»»å¡çæä¹åå­å¨é®é¢ï¼
+ä¼æå¨ç¥ï¼ä½¿ç¨apscheduleræ·»å çå®æ¶ä»»å¡ï¼ä¼å¨botéå¯åä¸¢å¤±ï¼è¿æ¯å ä¸ºä½¿ç¨
+[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-
+apscheduler)åå»ºåºæ¥çschedulerï¼é»è®¤ä½¿ç¨çJobStore
+(å³ä¿å­ä»»å¡çæ¹å¼)ï¼æ¯MemoryJobStoreï¼ä¹å°±æ¯å­å¨åå­ä¸­ï¼å æ­¤ä¼å¯¼è´éå¯ä¸¢ä»»å¡ã
+å æ­¤åè[apscheduler](https://apscheduler.readthedocs.io/en/latest/
+userguide.html#configuring-the-
+scheduler)ï¼ä½ å¯ä»¥å¨botçéç½®æä»¶ä¸­æ·»å éç½®é¡¹ï¼è®©[nonebot-
+plugin-apscheduler](https://github.com/nonebot/plugin-
+apscheduler)åå»ºåºæ¥çschedulerçé»è®¤ JobStore
+æ¹ä¸ºä½¿ç¨æ°æ®åºï¼è¿æ ·å°±å¯ä»¥æä¹åå­å¨ä»»å¡ï¼èä¸éè¦é¢å¤ä¿®æ¹ä»»ä½ä¸è¥¿ã
+ç¶èï¼å¾ä¸å¹¸çæ¯ï¼å¨apscheduler4.0çæ¬ä¹åï¼ææ¯æçæ°æ®åºç±»JobStoreé½æ¯ä½¿ç¨**åæ­¥**å¼æçï¼ç¶è
+[plugin-orm](https://github.com/nonebot/plugin-
+orm)æéç¨çæ¯å¼æ­¥å¼æï¼å æ­¤ä½ ææ¶è¿ä¸è½è¿æ ·åã
+æä»¥ï¼ææ¶è¿æ æ³è§£å³å®æ¶ä»»å¡çæä¹åå­å¨é®é¢ï¼é¤éapscheduleræ­£å¼åç4.0ï¼ç®åè¿æ¯alphaçæ¬ï¼ï¼ä½ å¯ä»¥åç­å¾ï¼æ¬æä»¶ä¼æç»­è·è¿æ´æ°ã
+## ðè´è°¢ - æè°¢[nonebot-plugin-htmlrender](https://github.com/kexue-z/
+nonebot-plugin-htmlrender)æä¾çæ¸²æå·¥å· - æè°¢[plugin-orm](https://
+github.com/nonebot/plugin-orm)æä¾çå¼æ­¥æ°æ®åºæ¥å£ - æè°¢[nonebot-
+plugin-apscheduler](https://github.com/nonebot/plugin-
+apscheduler)æä¾çå®æ¶ä»»å¡æ¥å£ - æè°¢[nonebot-plugin-alconna](https:
+//github.com/nonebot/plugin-alconna) - æè°¢[Matcha](https://github.com/A-
+kirami/matcha)æä¾çç®åå¥½ç¨çæµè¯å¹³å° ###
+åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ æè, ä½ ä¹å¯ä»¥çæåçå¶ä»æä»¶
+[nonebot-plugin-manga-translator](https://github.com/maoxig/nonebot-plugin-
+manga-translator)ä¸ä¸ªæ¯æå¤api, æ¹ä¾¿å¥½ç¨çå¾ç/æ¼«ç»ç¿»è¯æä»¶
```

### Comparing `nonebot_plugin_ai_timetable-0.3.8/PKG-INFO` & `nonebot_plugin_ai_timetable-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ai-timetable
-Version: 0.3.8
+Version: 0.4.0
 Summary: 小爱课程表
 Author: maoxiog
 Author-email: 674550338@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
 Requires-Dist: nonebot-plugin-alconna (>=0.40.1,<1.0.0)
-Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<1.0.0)
+Requires-Dist: nonebot-plugin-htmlrender (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot-plugin-orm (>=0.7.1)
 Requires-Dist: nonebot2 (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+  <a href="https://nonebot.dev/"><img src="https://nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 <div align="center">
 
 # nonebot-plugin-ai-timetable
 
 ✨*基于Nonebot2的对接小爱课程表的插件*✨
   
@@ -39,31 +40,33 @@
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 <div align="left">
 
 ## 💿安装
 
 1. 通过`pip`或`nb`安装；
-    - 使用nb(极度推荐)
+    - 使用nb(推荐)
   
        在机器人目录下命令行使用`nb plugin install nonebot_plugin_ai_timetable`
 
     - 使用pip:
   
       `pip plugin install nonebot_plugin_ai_timetable`
 
       然后在机器人`pyproject.toml`里的`plugins = []`列表追加`"nonebot_plugin_ai_timetable"`
 
-2. 本地数据保存在`data/ai_timetable/userdata.json`以及`data/ai_timetable/usertable.json`，分别对应用户发送的链接和本地保存的课表
+2. 数据存储使用[plugin-orm](https://github.com/nonebot/plugin-orm), 接入数据库，方便管理
+
+3. 第一次使用使用[plugin-orm](https://github.com/nonebot/plugin-orm)时，需要用`nb orm upgrade`升级数据库
 
 ## 📖简介
 
 1. 傻瓜式一键导入小爱课表，让你的bot实现小爱课表的功能
 
-2. 用户课表数据隔离，无需担心课程时间冲突、不同学校课表不同等问题
+2. 用户课表数据隔离，基于[plugin-rom](https://github.com/nonebot/plugin-orm), 接入数据库，无需担心课程时间冲突、不同学校课表不同等问题
 
 3. 适配多平台，即使是电报涩涩群也要好好学习！🥵🥵
 
 ## ⚙️插件配置
 
 这些配置都已设好默认值，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项(可选)
 
@@ -71,25 +74,37 @@
 | :---------------------: | :---: | :-----: | :------------------------: | :---------------------------------------------------------------------------------------------------- |
 |      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                                   |
 | TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                                              |
 |    TIMETABLE_ALOCK_8    |  int  |   21    |    TIMETABLE_ALOCK_8=16    | 订阅早八的发送时间，必须是0-24的数字.这里发送的都是第二天的，所以建议设置为18-23点                    |
 |   TIMETABLE_SEND_TIME   | float |   0.5   |   TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
 
 ## 💿依赖
-
+插件依赖会在安装时自动安装，如果安装失败，你可以按照以下指令手动再次安装
 ```python
 nb plugin install nonebot_plugin_htmlrender
 nb plugin install nonebot_plugin_apscheduler
 nb plugin install nonebot_plugin_alconna
+nb plugin install nonebot_plugin_orm
 ```
+
 ## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
+- 0.4.0 / 2024-04-30:
+   1. 重构完成，将所有数据迁移到官方数据库插件[plugin-orm](https://github.com/nonebot/plugin-orm)，之前的数据失效
+   2. 修改了插件触发指令和相关逻辑
+   3. 重构所有代码，优化处理逻辑
+   >该版本是破坏性更新，且仍在测试中，有任何疑问欢迎issue或pr
+
+- 0.3.8 / 2024-04-28:
+   1. 修复设置错误
+   2. 重构代码
+
 - 0.3.7 / 2024-04-24:
    1. 更新Nonebot2版本至2.2.0
    2. 基于 [nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna) 适配多平台
    3. 放宽httpx限制，移除onebot依赖
 
 - 0.3.6 / 2023-09-02:
    1. 适配nonebot2.0.1版本：移除过时的RegexMatch方法
@@ -145,52 +160,48 @@
 - 0.1.4 / 2023-03-05:
    1. 修复了无法取消订阅早八的bug
 
 </details>
 
 ## 🎉命令
 
-1. 我的课表|小爱课表|本周课表|下周课表：获取本周|下周的完全课表，使用前须先导入课表，这里的课表是在线课表
+1. 课表帮助：获取本条帮助
 
 2. 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
 
     ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 
     在基本设置里把开始上课时间等调整好之后(尤其是时间、节数)，把分享课表得到的链接发送给bot即可导入本地(分享前需要登录小米账户 [#1](https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1))
 
 3. 更新课表；如果在小爱课程表里修改了课程，发送该条指令即可更新本地的课表，无需重新导入
   
-4. (昨天|今天|明天|后天|周X|星期x|)(课表|有啥课|上啥课)：查询指定天的课表，其中查询周x课表查询的是本周的
-
-5. 订阅|取消订阅某天课表：导入本地课表后，发送订阅xx课表，如`订阅周一课表`，就可以在这天的前一天晚上10点(可修改)定时推送第二天要上的课
+4. 查询课表+[参数]：查询[参数]的课表，参数支持[本周/下周、周x、昨天/今天/明天/后天、早八、课程名]
 
-6. 订阅|取消订阅早八：会让bot在前一天晚上9点(可修改)提醒你第二天是否有早八，以便决定今晚是否嗨皮（判定依据是是否存在第一节课）
+5. 添加课程提醒+[参数]：参数支持[周x、早八、课程名]
 
-7. 订阅|取消订阅课程 xxx：订阅课程后，会让bot在所有名称里包含xxx的课程开始前0.5小时(可修改)发送提醒，如订阅课程 数学分析，则数学分析和数学分析习题课的课前0.5小时会自动发出提醒
+6. 删除课程提醒+[参数]：参数支持[全部、周x、早八、课程名]
 
-8. 上课|下节课：获取当前上课信息，返回下节课信息(如果有)
+7. 查看课程提醒：查看当前已经添加的课程提醒
 
-9. 早八|明日早八：查询明天的早八
-
-10. 课表帮助：获取课表帮助
-
-未完待续
 
 ## ⭐效果图
 
-![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/my_table.jpg)
-![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/alock_8.jpg)
-![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/next_class.jpg)
-![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/someday_classes.jpg)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/update.png)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query.png)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder.png)
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder1.png)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/someday_classes_pic.jpg)
 
 ### 关于小爱课程表内的一些说明
 
 如下图
 
+- 第一次使用本插件时，需要用`nb orm upgrade`升级数据库
 - 首先要登录上小米账户,否则可能获取到错误的课表信息 [#1](https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1)
 - 设置好开始上课时间
 - 设置好课程时间，可以修改每节课具体的时间，
 - 课表节数按自己需求调，一般教务导入的课表节数可能不符合实际，需要微调
 - 每周起始日建议默认的周一即可（周日起始没测试过可能有bug）
 - 如果导入课表后在小爱课表内修改了课程，直接给bot发送更新课表即可更新本地课表
 - 当你主页的课表和学校课表基本一致时，那么小爱课程表就被调教好了，可以导入了
@@ -207,23 +218,37 @@
 
 - [x] 重构代码
 
 - [x] 订阅指定的课
 
 - [x] 多平台适配, 基于 [nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna) 
 
-- [ ] 支持定时任务本地存储
+- [x] 支持定时任务本地存储
 
-- [ ] 适配[plugin-rom](https://github.com/nonebot/plugin-orm), 接入数据库
+- [x] 适配[plugin-orm](https://github.com/nonebot/plugin-orm), 接入数据库
 
 - [ ] 适配更多课表、脱离小爱课表
 
 - [ ] 完善插件
 
 ## 🐛存在的问题
 
- 1. 小爱课表分享的链接大概2周后会过期，会使得`我的课表\下周课表`无法使用，需要重新分享，但是仍能使用本地课表，也可以更新本地课表
+ ### 关于定时任务的持久化存储问题：
+
+众所周知，使用apscheduler添加的定时任务，会在bot重启后丢失，这是因为使用[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的scheduler，默认使用的JobStore(即保存任务的方式)，是MemoryJobStore，也就是存在内存中，因此会导致重启丢任务。
+
+因此参考[apscheduler](https://apscheduler.readthedocs.io/en/latest/userguide.html#configuring-the-scheduler)，你可以在bot的配置文件中添加配置项，让[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)创建出来的scheduler的默认 JobStore 改为使用数据库，这样就可以持久化存储任务，而不需要额外修改任何东西。
+
+然而，很不幸的是，在apscheduler4.0版本之前，所支持的数据库类JobStore都是使用**同步**引擎的，然而[plugin-orm](https://github.com/nonebot/plugin-orm)所采用的是异步引擎，因此你暂时还不能这样做。
 
- 2. 机器人重启后定时任务会丢失
+所以，暂时还无法解决定时任务的持久化存储问题，除非apscheduler正式发版4.0（目前还是alpha版本），你可以再等待，本插件会持续跟进更新。
 
-## 喜欢的话就点个star✨吧QAQ
+## 🎉致谢
+- 感谢[nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender)提供的渲染工具
+- 感谢[plugin-orm](https://github.com/nonebot/plugin-orm)提供的异步数据库接口
+- 感谢[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-apscheduler)提供的定时任务接口
+- 感谢[nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna)
+- 感谢[Matcha](https://github.com/A-kirami/matcha)提供的简单好用的测试平台
+### 喜欢的话就点个star✨吧
+或者, 你也可以看我写的其他插件
+[nonebot-plugin-manga-translator](https://github.com/maoxig/nonebot-plugin-manga-translator)一个支持多api, 方便好用的图片/漫画翻译插件
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.3.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.4.0 Summary:
 å°ç±è¯¾ç¨è¡¨ Author: maoxiog Author-email: 674550338@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-
 plugin-alconna (>=0.40.1,<1.0.0) Requires-Dist: nonebot-plugin-apscheduler
-(>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot2 (>=2.2.0,<3.0.0) Description-Content-Type: text/
-markdown
+(>=0.2.0,<1.0.0) Requires-Dist: nonebot-plugin-htmlrender (>=0.3.0,<0.4.0)
+Requires-Dist: nonebot-plugin-orm (>=0.7.1) Requires-Dist: nonebot2
+(>=2.2.0,<3.0.0) Description-Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
                          # nonebot-plugin-ai-timetable
 â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨_[_n_o_n_e_b_o_t_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
-## ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
+## ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æ¨è)
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨`nb plugin install
 nonebot_plugin_ai_timetable` - ä½¿ç¨pip: `pip plugin install
 nonebot_plugin_ai_timetable` ç¶åå¨æºå¨äºº`pyproject.toml`éç`plugins =
-[]`åè¡¨è¿½å `"nonebot_plugin_ai_timetable"` 2. æ¬å°æ°æ®ä¿å­å¨`data/
-ai_timetable/userdata.json`ä»¥å`data/ai_timetable/
-usertable.json`ï¼åå«å¯¹åºç¨æ·åéçé¾æ¥åæ¬å°ä¿å­çè¯¾è¡¨ ##
-ðç®ä» 1.
+[]`åè¡¨è¿½å `"nonebot_plugin_ai_timetable"` 2. æ°æ®å­å¨ä½¿ç¨[plugin-
+orm](https://github.com/nonebot/plugin-orm), æ¥å¥æ°æ®åºï¼æ¹ä¾¿ç®¡ç 3.
+ç¬¬ä¸æ¬¡ä½¿ç¨ä½¿ç¨[plugin-orm](https://github.com/nonebot/plugin-
+orm)æ¶ï¼éè¦ç¨`nb orm upgrade`åçº§æ°æ®åº ## ðç®ä» 1.
 å»çå¼ä¸é®å¯¼å¥å°ç±è¯¾è¡¨ï¼è®©ä½ çbotå®ç°å°ç±è¯¾è¡¨çåè½ 2.
-ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
+ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼åºäº[plugin-rom](https://github.com/nonebot/
+plugin-orm),
+æ¥å¥æ°æ®åºï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
 3. ééå¤å¹³å°ï¼å³ä½¿æ¯çµæ¥æ¶©æ¶©ç¾¤ä¹è¦å¥½å¥½å­¦ä¹ ï¼ð¥µð¥µ ##
 âï¸æä»¶éç½®
 è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹
 (å¯é) | config | type | default | example | usage | | :--------------------
 -: | :---: | :-----: | :------------------------: | :--------------------------
 -------------------------------------------------------------------------- | |
 TIMETABLE_PIC | bool | true | TIMETABLE_PIC=false |
@@ -34,18 +36,26 @@
 TIMETABLE_ALOCK_SOMEDAY | int | 22 | TIMETABLE_ALOCK_SOMEDAY=15 |
 è®¢éææ¥è¯¾è¡¨çåéæ¶é´ï¼å¿é¡»æ¯0-24çæ°å­ | |
 TIMETABLE_ALOCK_8 | int | 21 | TIMETABLE_ALOCK_8=16 |
 è®¢éæ©å«çåéæ¶é´ï¼å¿é¡»æ¯0-
 24çæ°å­.è¿éåéçé½æ¯ç¬¬äºå¤©çï¼æä»¥å»ºè®®è®¾ç½®ä¸º18-23ç¹ |
 | TIMETABLE_SEND_TIME | float | 0.5 | TIMETABLE_SEND_TIME=1 |
 è®¢éè¯¾ç¨æååéçæ¶é´ï¼åä½æ¯`å°æ¶`ï¼å¯ä»¥æ¯æ´æ°ä¹å¯ä»¥æ¯å°æ°ï¼å»ºè®®ä¸è¦è®¾çå¤ªå¤§ï¼é¿ååºç°æ æ³é¢æçbug
-| ## ð¿ä¾èµ ```python nb plugin install nonebot_plugin_htmlrender nb plugin
-install nonebot_plugin_apscheduler nb plugin install nonebot_plugin_alconna ```
-## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 0.3.7 / 2024-04-24: 1.
-æ´æ°Nonebot2çæ¬è³2.2.0 2. åºäº [nonebot-plugin-alconna](https://
+| ## ð¿ä¾èµ
+æä»¶ä¾èµä¼å¨å®è£æ¶èªå¨å®è£ï¼å¦æå®è£å¤±è´¥ï¼ä½ å¯ä»¥æç§ä»¥ä¸æä»¤æå¨åæ¬¡å®è£
+```python nb plugin install nonebot_plugin_htmlrender nb plugin install
+nonebot_plugin_apscheduler nb plugin install nonebot_plugin_alconna nb plugin
+install nonebot_plugin_orm ``` ## ðæ´æ°æ¥å¿ ç¹å»å±å¼ - 0.4.0 / 2024-
+04-30: 1. éæå®æï¼å°æææ°æ®è¿ç§»å°å®æ¹æ°æ®åºæä»¶[plugin-
+orm](https://github.com/nonebot/plugin-orm)ï¼ä¹åçæ°æ®å¤±æ 2.
+ä¿®æ¹äºæä»¶è§¦åæä»¤åç¸å³é»è¾ 3.
+éæææä»£ç ï¼ä¼åå¤çé»è¾
+>è¯¥çæ¬æ¯ç ´åæ§æ´æ°ï¼ä¸ä»å¨æµè¯ä¸­ï¼æä»»ä½çé®æ¬¢è¿issueæpr
+- 0.3.8 / 2024-04-28: 1. ä¿®å¤è®¾ç½®éè¯¯ 2. éæä»£ç  - 0.3.7 / 2024-04-
+24: 1. æ´æ°Nonebot2çæ¬è³2.2.0 2. åºäº [nonebot-plugin-alconna](https://
 github.com/nonebot/plugin-alconna) ééå¤å¹³å° 3.
 æ¾å®½httpxéå¶ï¼ç§»é¤onebotä¾èµ - 0.3.6 / 2023-09-02: 1.
 éénonebot2.0.1çæ¬ï¼ç§»é¤è¿æ¶çRegexMatchæ¹æ³
 >å¦æ´æ°æ¬æä»¶åæ¥åæ¶æ¯æ ååºï¼è¯·æ´æ°ä½ çnonebotçæ¬æåéå°æ§çæ¬ä½¿ç¨
 - 0.3.5 / 2023-08-10: 1. æ ¼å¼åä»£ç  2. ä¼åéç½®è¯»å 3.
 æ´æ°æä»¶åæ°æ® - 0.3.5 / 2023-06-09: 1. æ´æ°httpxä¾èµçæ¬ - 0.3.3
 / 2023-04-23: 1. ä¿®å¤å®æ¶æééå¤åéçbug 2. ä¿®æ¹å¸®å© - 0.3.2 /
@@ -63,46 +73,39 @@
 - 0.1.8 / 2023-03-08: 1. ä¿®æ¹é¨åä»£ç ï¼ä¼åè¯¾è¡¨æ ¼å¼ 2.
 ä¿®å¤äºèæ°ä¸º11çè¯¾ä¼æå¨èæ°ä¸º2çè¯¾ç¨åé¢çbug
 (QAQå¤ªè ¢äºå«éªäºå«éªäº) - 0.1.7 / 2023-03-07: 1.
 ä¿®å¤äºæ¶é´ä¸ä¼èªå·±æ¹åçbug 2. æ°å¢äºä¸è¯¾/ä¸èè¯¾åè½ 3.
 ä¼åäºä¸äºå±å±±ä»£ç  - 0.1.5 / 2023-03-06: 1.
 æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 0.1.4 / 2023-03-05: 1.
 ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug ## ðå½ä»¤ 1.
-æçè¯¾è¡¨|å°ç±è¯¾è¡¨|æ¬å¨è¯¾è¡¨|ä¸å¨è¯¾è¡¨ï¼è·åæ¬å¨|ä¸å¨çå®å¨è¯¾è¡¨ï¼ä½¿ç¨åé¡»åå¯¼å¥è¯¾è¡¨ï¼è¿éçè¯¾è¡¨æ¯å¨çº¿è¯¾è¡¨
-2.
+è¯¾è¡¨å¸®å©ï¼è·åæ¬æ¡å¸®å© 2.
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
 (åäº«åéè¦ç»å½å°ç±³è´¦æ· [#1](https://github.com/maoxig/nonebot-
 plugin-ai-timetable/issues/1)) 3.
 æ´æ°è¯¾è¡¨ï¼å¦æå¨å°ç±è¯¾ç¨è¡¨éä¿®æ¹äºè¯¾ç¨ï¼åéè¯¥æ¡æä»¤å³å¯æ´æ°æ¬å°çè¯¾è¡¨ï¼æ ééæ°å¯¼å¥
-4. (æ¨å¤©|ä»å¤©|æå¤©|åå¤©|å¨X|ææx|)
-(è¯¾è¡¨|æå¥è¯¾|ä¸å¥è¯¾)ï¼æ¥è¯¢æå®å¤©çè¯¾è¡¨ï¼å¶ä¸­æ¥è¯¢å¨xè¯¾è¡¨æ¥è¯¢çæ¯æ¬å¨ç
-5.
-è®¢é|åæ¶è®¢éæå¤©è¯¾è¡¨ï¼å¯¼å¥æ¬å°è¯¾è¡¨åï¼åéè®¢éxxè¯¾è¡¨ï¼å¦`è®¢éå¨ä¸è¯¾è¡¨`ï¼å°±å¯ä»¥å¨è¿å¤©çåä¸å¤©æä¸10ç¹
-(å¯ä¿®æ¹)å®æ¶æ¨éç¬¬äºå¤©è¦ä¸çè¯¾ 6.
-è®¢é|åæ¶è®¢éæ©å«ï¼ä¼è®©botå¨åä¸å¤©æä¸9ç¹
-(å¯ä¿®æ¹)æéä½ ç¬¬äºå¤©æ¯å¦ææ©å«ï¼ä»¥ä¾¿å³å®ä»ææ¯å¦å¨ç®ï¼å¤å®ä¾æ®æ¯æ¯å¦å­å¨ç¬¬ä¸èè¯¾ï¼
-7. è®¢é|åæ¶è®¢éè¯¾ç¨
-xxxï¼è®¢éè¯¾ç¨åï¼ä¼è®©botå¨ææåç§°éåå«xxxçè¯¾ç¨å¼å§å0.5å°æ¶
-(å¯ä¿®æ¹)åéæéï¼å¦è®¢éè¯¾ç¨
-æ°å­¦åæï¼åæ°å­¦åæåæ°å­¦åæä¹ é¢è¯¾çè¯¾å0.5å°æ¶ä¼èªå¨ååºæé
-8. ä¸è¯¾|ä¸èè¯¾ï¼è·åå½åä¸è¯¾ä¿¡æ¯ï¼è¿åä¸èè¯¾ä¿¡æ¯
-(å¦ææ) 9. æ©å«|ææ¥æ©å«ï¼æ¥è¯¢æå¤©çæ©å« 10.
-è¯¾è¡¨å¸®å©ï¼è·åè¯¾è¡¨å¸®å© æªå®å¾ç»­ ## â­ææå¾ ![Image text]
+4. æ¥è¯¢è¯¾è¡¨+[åæ°]ï¼æ¥è¯¢[åæ°]çè¯¾è¡¨ï¼åæ°æ¯æ[æ¬å¨/
+ä¸å¨ãå¨xãæ¨å¤©/ä»å¤©/æå¤©/åå¤©ãæ©å«ãè¯¾ç¨å] 5.
+æ·»å è¯¾ç¨æé+[åæ°]ï¼åæ°æ¯æ[å¨xãæ©å«ãè¯¾ç¨å] 6.
+å é¤è¯¾ç¨æé+[åæ°]ï¼åæ°æ¯æ[å¨é¨ãå¨xãæ©å«ãè¯¾ç¨å]
+7. æ¥çè¯¾ç¨æéï¼æ¥çå½åå·²ç»æ·»å çè¯¾ç¨æé ## â­ææå¾
+![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
+resource/update.png) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
+timetable/blob/main/resource/query.png) ![Image text](https://github.com/
+maoxig/nonebot-plugin-ai-timetable/blob/main/resource/query1.png) ![Image text]
 (https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
-my_table.jpg) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
-timetable/blob/main/resource/alock_8.jpg) ![Image text](https://github.com/
-maoxig/nonebot-plugin-ai-timetable/blob/main/resource/next_class.jpg) ![Image
+query1.png) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
+timetable/blob/main/resource/reminder.png) ![Image text](https://github.com/
+maoxig/nonebot-plugin-ai-timetable/blob/main/resource/reminder1.png) ![Image
 text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
-someday_classes.jpg) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
-timetable/blob/main/resource/someday_classes_pic.jpg) ###
-å³äºå°ç±è¯¾ç¨è¡¨åçä¸äºè¯´æ å¦ä¸å¾ -
+someday_classes_pic.jpg) ### å³äºå°ç±è¯¾ç¨è¡¨åçä¸äºè¯´æ å¦ä¸å¾
+- ç¬¬ä¸æ¬¡ä½¿ç¨æ¬æä»¶æ¶ï¼éè¦ç¨`nb orm upgrade`åçº§æ°æ®åº -
 é¦åè¦ç»å½ä¸å°ç±³è´¦æ·,å¦åå¯è½è·åå°éè¯¯çè¯¾è¡¨ä¿¡æ¯ [#1]
 (https://github.com/maoxig/nonebot-plugin-ai-timetable/issues/1) -
 è®¾ç½®å¥½å¼å§ä¸è¯¾æ¶é´ -
 è®¾ç½®å¥½è¯¾ç¨æ¶é´ï¼å¯ä»¥ä¿®æ¹æ¯èè¯¾å·ä½çæ¶é´ï¼ -
 è¯¾è¡¨èæ°æèªå·±éæ±è°ï¼ä¸è¬æå¡å¯¼å¥çè¯¾è¡¨èæ°å¯è½ä¸ç¬¦åå®éï¼éè¦å¾®è°
 -
 æ¯å¨èµ·å§æ¥å»ºè®®é»è®¤çå¨ä¸å³å¯ï¼å¨æ¥èµ·å§æ²¡æµè¯è¿å¯è½æbugï¼
@@ -110,15 +113,36 @@
 å¦æå¯¼å¥è¯¾è¡¨åå¨å°ç±è¯¾è¡¨åä¿®æ¹äºè¯¾ç¨ï¼ç´æ¥ç»botåéæ´æ°è¯¾è¡¨å³å¯æ´æ°æ¬å°è¯¾è¡¨
 -
 å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è°æå¥½äºï¼å¯ä»¥å¯¼å¥äº
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
 resource/settings.jpg) ## ð¦è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
 å¯éæ©æ¯å¦åéå¾çä»¥é¿åé£æ§ - [x] å¢å æ´å¤çéç½®é¡¹ - [x]
 éæä»£ç  - [x] è®¢éæå®çè¯¾ - [x] å¤å¹³å°éé, åºäº [nonebot-
-plugin-alconna](https://github.com/nonebot/plugin-alconna) - [ ]
-æ¯æå®æ¶ä»»å¡æ¬å°å­å¨ - [ ] éé[plugin-rom](https://github.com/
+plugin-alconna](https://github.com/nonebot/plugin-alconna) - [x]
+æ¯æå®æ¶ä»»å¡æ¬å°å­å¨ - [x] éé[plugin-orm](https://github.com/
 nonebot/plugin-orm), æ¥å¥æ°æ®åº - [ ]
 ééæ´å¤è¯¾è¡¨ãè±ç¦»å°ç±è¯¾è¡¨ - [ ] å®åæä»¶ ##
-ðå­å¨çé®é¢ 1.
-å°ç±è¯¾è¡¨åäº«çé¾æ¥å¤§æ¦2å¨åä¼è¿æï¼ä¼ä½¿å¾`æçè¯¾è¡¨\ä¸å¨è¯¾è¡¨`æ æ³ä½¿ç¨ï¼éè¦éæ°åäº«ï¼ä½æ¯ä»è½ä½¿ç¨æ¬å°è¯¾è¡¨ï¼ä¹å¯ä»¥æ´æ°æ¬å°è¯¾è¡¨
-2. æºå¨äººéå¯åå®æ¶ä»»å¡ä¼ä¸¢å¤± ##
-åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§QAQ
+ðå­å¨çé®é¢ ### å³äºå®æ¶ä»»å¡çæä¹åå­å¨é®é¢ï¼
+ä¼æå¨ç¥ï¼ä½¿ç¨apscheduleræ·»å çå®æ¶ä»»å¡ï¼ä¼å¨botéå¯åä¸¢å¤±ï¼è¿æ¯å ä¸ºä½¿ç¨
+[nonebot-plugin-apscheduler](https://github.com/nonebot/plugin-
+apscheduler)åå»ºåºæ¥çschedulerï¼é»è®¤ä½¿ç¨çJobStore
+(å³ä¿å­ä»»å¡çæ¹å¼)ï¼æ¯MemoryJobStoreï¼ä¹å°±æ¯å­å¨åå­ä¸­ï¼å æ­¤ä¼å¯¼è´éå¯ä¸¢ä»»å¡ã
+å æ­¤åè[apscheduler](https://apscheduler.readthedocs.io/en/latest/
+userguide.html#configuring-the-
+scheduler)ï¼ä½ å¯ä»¥å¨botçéç½®æä»¶ä¸­æ·»å éç½®é¡¹ï¼è®©[nonebot-
+plugin-apscheduler](https://github.com/nonebot/plugin-
+apscheduler)åå»ºåºæ¥çschedulerçé»è®¤ JobStore
+æ¹ä¸ºä½¿ç¨æ°æ®åºï¼è¿æ ·å°±å¯ä»¥æä¹åå­å¨ä»»å¡ï¼èä¸éè¦é¢å¤ä¿®æ¹ä»»ä½ä¸è¥¿ã
+ç¶èï¼å¾ä¸å¹¸çæ¯ï¼å¨apscheduler4.0çæ¬ä¹åï¼ææ¯æçæ°æ®åºç±»JobStoreé½æ¯ä½¿ç¨**åæ­¥**å¼æçï¼ç¶è
+[plugin-orm](https://github.com/nonebot/plugin-
+orm)æéç¨çæ¯å¼æ­¥å¼æï¼å æ­¤ä½ ææ¶è¿ä¸è½è¿æ ·åã
+æä»¥ï¼ææ¶è¿æ æ³è§£å³å®æ¶ä»»å¡çæä¹åå­å¨é®é¢ï¼é¤éapscheduleræ­£å¼åç4.0ï¼ç®åè¿æ¯alphaçæ¬ï¼ï¼ä½ å¯ä»¥åç­å¾ï¼æ¬æä»¶ä¼æç»­è·è¿æ´æ°ã
+## ðè´è°¢ - æè°¢[nonebot-plugin-htmlrender](https://github.com/kexue-z/
+nonebot-plugin-htmlrender)æä¾çæ¸²æå·¥å· - æè°¢[plugin-orm](https://
+github.com/nonebot/plugin-orm)æä¾çå¼æ­¥æ°æ®åºæ¥å£ - æè°¢[nonebot-
+plugin-apscheduler](https://github.com/nonebot/plugin-
+apscheduler)æä¾çå®æ¶ä»»å¡æ¥å£ - æè°¢[nonebot-plugin-alconna](https:
+//github.com/nonebot/plugin-alconna) - æè°¢[Matcha](https://github.com/A-
+kirami/matcha)æä¾çç®åå¥½ç¨çæµè¯å¹³å° ###
+åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§ æè, ä½ ä¹å¯ä»¥çæåçå¶ä»æä»¶
+[nonebot-plugin-manga-translator](https://github.com/maoxig/nonebot-plugin-
+manga-translator)ä¸ä¸ªæ¯æå¤api, æ¹ä¾¿å¥½ç¨çå¾ç/æ¼«ç»ç¿»è¯æä»¶
```

