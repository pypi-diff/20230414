# Comparing `tmp/nonebot_plugin_ai_timetable-0.3.0.tar.gz` & `tmp/nonebot_plugin_ai_timetable-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ai_timetable-0.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_ai_timetable-0.3.2.tar", max compression
```

## Comparing `nonebot_plugin_ai_timetable-0.3.0.tar` & `nonebot_plugin_ai_timetable-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-04-02 06:57:08.834132 nonebot_plugin_ai_timetable-0.3.0/LICENSE
--rw-r--r--   0        0        0     7518 2023-04-02 06:57:08.834132 nonebot_plugin_ai_timetable-0.3.0/README.md
--rw-r--r--   0        0        0    10903 2023-04-02 06:57:08.834132 nonebot_plugin_ai_timetable-0.3.0/nonebot_plugin_ai_timetable/__init__.py
--rw-r--r--   0        0        0    16789 2023-04-02 06:57:08.834132 nonebot_plugin_ai_timetable-0.3.0/nonebot_plugin_ai_timetable/utils.py
--rw-r--r--   0        0        0      496 2023-04-02 06:57:08.834132 nonebot_plugin_ai_timetable-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8237 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-14 08:36:46.151410 nonebot_plugin_ai_timetable-0.3.2/LICENSE
+-rw-r--r--   0        0        0     7671 2023-04-14 08:36:46.151410 nonebot_plugin_ai_timetable-0.3.2/README.md
+-rw-r--r--   0        0        0    10863 2023-04-14 08:36:46.151410 nonebot_plugin_ai_timetable-0.3.2/nonebot_plugin_ai_timetable/__init__.py
+-rw-r--r--   0        0        0    16712 2023-04-14 08:36:46.155410 nonebot_plugin_ai_timetable-0.3.2/nonebot_plugin_ai_timetable/utils.py
+-rw-r--r--   0        0        0      496 2023-04-14 08:36:46.155410 nonebot_plugin_ai_timetable-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8390 1970-01-01 00:00:00.000000 nonebot_plugin_ai_timetable-0.3.2/PKG-INFO
```

### Comparing `nonebot_plugin_ai_timetable-0.3.0/LICENSE` & `nonebot_plugin_ai_timetable-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ai_timetable-0.3.0/README.md` & `nonebot_plugin_ai_timetable-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,58 +10,58 @@
 <div align="left">
   
 # 前言
 
    这是本人第一次在github发布的项目，也是第一个python项目，完全是萌新，很多地方写的可能很拉，大佬轻喷
 目前还不是很完善，有什么bug或者建议欢迎提issues
 
-## 安装
+## 💿安装
 
 1. 通过`pip`或`nb`安装；
     - 使用nb(极度推荐)
   
        在机器人目录下命令行使用`nb plugin install nonebot_plugin_ai_timetable`
 
     - 使用pip(不推荐):
   
       ~~既然不推荐就不要想着这样安装了啊喂~~
 
 2. 本地数据保存在`data/ai_timetable/userdata.json`以及`data/ai_timetable/usertable.json`，分别对应用户发送的链接和本地保存的课表
 
-## 简介
+## 📖简介
 
 1. 傻瓜式一键导入小爱课表，让你的bot实现小爱课表的功能
 
 2. 用户课表数据隔离，无需担心课程时间冲突、不同学校课表不同等问题
 
 3. ~~所以为什么不直接用小爱课表呢~~
 
-4. 插件配置
+4. ⚙️插件配置
 
 这些配置都已设好默认值，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项(可选)
 
 |         config          | type  | default |          example           | usage                                                                              |
 | :---------------------: | :---: | :-----: | :------------------------: | :--------------------------------------------------------------------------------- |
 |      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                |
 | TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                           |
 |    TIMETABLE_ALOCK_8    |  int  |   21    |    TIMETABLE_ALOCK_8=16    | 订阅早八的发送时间，必须是0-24的数字.这里发送的都是第二天的，所以建议设置为18-23点 |
-|    TIMETABLE_SEND_TIME    |  int  |   0.5    |    TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
+|    TIMETABLE_SEND_TIME    |  float  |   0.5    |    TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
 
-## 依赖
+## 💿依赖
 
 ```python
 nb plugin install nonebot_plugin_htmlrender
 nb plugin install nonebot_plugin_apscheduler
 ```
 
 若不安装[nonebot_plugin_htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender)插件会无法导入在线课表
 
 不安装[nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler)会无法使用定时任务,其他功能无影响
 
-## 更新日志
+## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
 - 2023-03-05:
 
     修复了无法取消订阅早八的bug
@@ -91,26 +91,31 @@
     修复订阅早八的一些bug
 
 - 2023-03-29:
 
 1. 重构了代码，优化了许多地方~~真的累死了~~
 2. 修复了一些bug，优化了体验
 3. 增加了早八|明日早八的查询
-4. 更新版本后建议重新[导入课表]，避免出现某些bug
+4. 更新版本后建议重新`导入课表`，避免出现某些bug
 
 - 2023-04-02:
 
 1. 修复bug
 2. 优化帮助图片
 3. 定时任务随机延后0-60s，防止风控
 4. 增加订阅指定课程的功能
 
+- 2023-04-14:
+
+1. 修复了订阅课程发送时间错误的bug
+2. 删去了文本中所有奇怪的口癖喵
+
 </details>
 
-## 命令
+## 🎉命令
 
 1. 我的课表|小爱课表|本周课表|下周课表：获取本周|下周的完全课表，使用前须先导入课表，这里的课表是在线课表
 
 2. 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
 
     ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 
@@ -130,15 +135,15 @@
 
 9. 早八|明日早八：查询明天的早八
 
 10. 课表帮助：获取课表帮助
 
 未完待续
 
-## 效果图
+## ⭐效果图
 
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/my_table.jpg)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/alock_8.jpg)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/next_class.jpg)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/someday_classes.jpg)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/someday_classes_pic.jpg)
 
@@ -152,28 +157,28 @@
 - 课表节数按自己需求调，一般教务导入的课表节数可能不符合实际，需要微调
 - 每周起始日建议默认的周一即可（周日起始没测试过可能有bug）
 - 如果导入课表后在小爱课表内修改了课程，直接给bot发送更新课表即可更新本地课表
 - 当你主页的课表和学校课表基本一致时，那么小爱课程表就被调教好了，可以导入了
 
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/settings.jpg)
 
-## 计划
+## 🐦计划
 
 - [x] 查询下节课的信息
 
 - [x] 可选择是否发送图片以避免风控
 
 - [x] 增加更多的配置项
 
 - [x] 重构代码
 
 - [x] 订阅指定的课
 
 - [ ] 完善插件
 
-## 存在的问题
+## 🐛存在的问题
 
  1. 小爱课表分享的链接大概2周后会过期，会使得`我的课表\下周课表`无法使用，需要重新分享，但是仍能使用本地课表，也可以更新本地课表
 
  2. 机器人重启后定时任务会丢失
 
-## 喜欢的话就点个star吧QAQ
+## 喜欢的话就点个star✨吧QAQ
```

#### html2text {}

```diff
@@ -1,58 +1,61 @@
                                    [nonebot]
                          # nonebot-plugin-ai-timetable
             â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨
 # åè¨
 è¿æ¯æ¬äººç¬¬ä¸æ¬¡å¨githubåå¸çé¡¹ç®ï¼ä¹æ¯ç¬¬ä¸ä¸ªpythoné¡¹ç®ï¼å®å¨æ¯èæ°ï¼å¾å¤å°æ¹åçå¯è½å¾æï¼å¤§ä½¬è½»å·
-ç®åè¿ä¸æ¯å¾å®åï¼æä»ä¹bugæèå»ºè®®æ¬¢è¿æissues ## å®è£ 1.
-éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
+ç®åè¿ä¸æ¯å¾å®åï¼æä»ä¹bugæèå»ºè®®æ¬¢è¿æissues ##
+ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨`nb plugin install
 nonebot_plugin_ai_timetable` - ä½¿ç¨pip(ä¸æ¨è):
 ~~æ¢ç¶ä¸æ¨èå°±ä¸è¦æ³çè¿æ ·å®è£äºåå~~ 2.
 æ¬å°æ°æ®ä¿å­å¨`data/ai_timetable/userdata.json`ä»¥å`data/ai_timetable/
 usertable.json`ï¼åå«å¯¹åºç¨æ·åéçé¾æ¥åæ¬å°ä¿å­çè¯¾è¡¨ ##
-ç®ä» 1.
+ðç®ä» 1.
 å»çå¼ä¸é®å¯¼å¥å°ç±è¯¾è¡¨ï¼è®©ä½ çbotå®ç°å°ç±è¯¾è¡¨çåè½ 2.
 ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
-3. ~~æä»¥ä¸ºä»ä¹ä¸ç´æ¥ç¨å°ç±è¯¾è¡¨å¢~~ 4. æä»¶éç½®
+3. ~~æä»¥ä¸ºä»ä¹ä¸ç´æ¥ç¨å°ç±è¯¾è¡¨å¢~~ 4. âï¸æä»¶éç½®
 è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹
 (å¯é) | config | type | default | example | usage | | :--------------------
 -: | :---: | :-----: | :------------------------: | :--------------------------
 ------------------------------------------------------- | | TIMETABLE_PIC |
 bool | true | TIMETABLE_PIC=false | å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/
 æå­åéï¼é»è®¤ä»¥å¾çåé(true) | | TIMETABLE_ALOCK_SOMEDAY | int |
 22 | TIMETABLE_ALOCK_SOMEDAY=15 |
 è®¢éææ¥è¯¾è¡¨çåéæ¶é´ï¼å¿é¡»æ¯0-24çæ°å­ | |
 TIMETABLE_ALOCK_8 | int | 21 | TIMETABLE_ALOCK_8=16 |
 è®¢éæ©å«çåéæ¶é´ï¼å¿é¡»æ¯0-
 24çæ°å­.è¿éåéçé½æ¯ç¬¬äºå¤©çï¼æä»¥å»ºè®®è®¾ç½®ä¸º18-23ç¹ |
-| TIMETABLE_SEND_TIME | int | 0.5 | TIMETABLE_SEND_TIME=1 |
+| TIMETABLE_SEND_TIME | float | 0.5 | TIMETABLE_SEND_TIME=1 |
 è®¢éè¯¾ç¨æååéçæ¶é´ï¼åä½æ¯`å°æ¶`ï¼å¯ä»¥æ¯æ´æ°ä¹å¯ä»¥æ¯å°æ°ï¼å»ºè®®ä¸è¦è®¾çå¤ªå¤§ï¼é¿ååºç°æ æ³é¢æçbug
-| ## ä¾èµ ```python nb plugin install nonebot_plugin_htmlrender nb plugin
+| ## ð¿ä¾èµ ```python nb plugin install nonebot_plugin_htmlrender nb plugin
 install nonebot_plugin_apscheduler ``` è¥ä¸å®è£[nonebot_plugin_htmlrender]
 (https://github.com/kexue-z/nonebot-plugin-
 htmlrender)æä»¶ä¼æ æ³å¯¼å¥å¨çº¿è¯¾è¡¨ ä¸å®è£
 [nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-
-apscheduler)ä¼æ æ³ä½¿ç¨å®æ¶ä»»å¡,å¶ä»åè½æ å½±å ## æ´æ°æ¥å¿
-ç¹å»å±å¼ - 2023-03-05: ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug - 2023-03-
-06: æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 2023-03-07: 1.
+apscheduler)ä¼æ æ³ä½¿ç¨å®æ¶ä»»å¡,å¶ä»åè½æ å½±å ##
+ðæ´æ°æ¥å¿  ç¹å»å±å¼ - 2023-03-05:
+ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug - 2023-03-06:
+æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 2023-03-07: 1.
 ä¿®å¤äºæ¶é´ä¸ä¼èªå·±æ¹åçbug 2. æ°å¢äºä¸è¯¾/ä¸èè¯¾ åè½ 3.
 ä¼åäºä¸äºå±å±±ä»£ç  - 2023-03-08: 1.
 ä¿®æ¹é¨åä»£ç ï¼ä¼åè¯¾è¡¨æ ¼å¼ 2.
 ä¿®å¤äºèæ°ä¸º11çè¯¾ä¼æå¨èæ°ä¸º2çè¯¾ç¨åé¢çbug
 (QAQå¤ªè ¢äºå«éªäºå«éªäº) - 2023-03-11: 1.
 ä¿®å¤äºå¦ææªç»å½å°ç±³è´¦æ·å°±åäº«è¯¾è¡¨æ¶çæ¥é,å¢å éè¯¯æç¤º
 2.
 æ°å¢3é¡¹éç½®é¡¹ï¼ææ¥è¯¾è¡¨å¯éæ©ä»¥å¾çåéï¼é»è®¤ä¸ºå¾çï¼
 - 2023-03-13ï¼ ä¿®å¤è®¢éæ©å«çä¸äºbug - 2023-03-29: 1.
 éæäºä»£ç ï¼ä¼åäºè®¸å¤å°æ¹~~ççç´¯æ­»äº~~ 2.
 ä¿®å¤äºä¸äºbugï¼ä¼åäºä½éª 3. å¢å äºæ©å«|ææ¥æ©å«çæ¥è¯¢
-4. æ´æ°çæ¬åå»ºè®®éæ°[å¯¼å¥è¯¾è¡¨]ï¼é¿ååºç°æäºbug - 2023-04-
+4. æ´æ°çæ¬åå»ºè®®éæ°`å¯¼å¥è¯¾è¡¨`ï¼é¿ååºç°æäºbug - 2023-04-
 02: 1. ä¿®å¤bug 2. ä¼åå¸®å©å¾ç 3. å®æ¶ä»»å¡éæºå»¶å0-
-60sï¼é²æ­¢é£æ§ 4. å¢å è®¢éæå®è¯¾ç¨çåè½  ## å½ä»¤ 1.
+60sï¼é²æ­¢é£æ§ 4. å¢å è®¢éæå®è¯¾ç¨çåè½ - 2023-04-14: 1.
+ä¿®å¤äºè®¢éè¯¾ç¨åéæ¶é´éè¯¯çbug 2.
+å å»äºææ¬ä¸­ææå¥æªçå£çåµ  ## ðå½ä»¤ 1.
 æçè¯¾è¡¨|å°ç±è¯¾è¡¨|æ¬å¨è¯¾è¡¨|ä¸å¨è¯¾è¡¨ï¼è·åæ¬å¨|ä¸å¨çå®å¨è¯¾è¡¨ï¼ä½¿ç¨åé¡»åå¯¼å¥è¯¾è¡¨ï¼è¿éçè¯¾è¡¨æ¯å¨çº¿è¯¾è¡¨
 2.
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
@@ -68,15 +71,15 @@
 (å¯ä¿®æ¹)æéä½ ç¬¬äºå¤©æ¯å¦ææ©å«ï¼ä»¥ä¾¿å³å®ä»ææ¯å¦å¨ç®ï¼å¤å®ä¾æ®æ¯æ¯å¦å­å¨ç¬¬ä¸èè¯¾ï¼
 7. è®¢é|åæ¶è®¢éè¯¾ç¨
 xxxï¼è®¢éè¯¾ç¨åï¼ä¼è®©botå¨ææåç§°éåå«xxxçè¯¾ç¨å¼å§å0.5å°æ¶
 (å¯ä¿®æ¹)åéæéï¼å¦è®¢éè¯¾ç¨
 æ°å­¦åæï¼åæ°å­¦åæåæ°å­¦åæä¹ é¢è¯¾çè¯¾å0.5å°æ¶ä¼èªå¨ååºæé
 8. ä¸è¯¾|ä¸èè¯¾ï¼è·åå½åä¸è¯¾ä¿¡æ¯ï¼è¿åä¸èè¯¾ä¿¡æ¯
 (å¦ææ) 9. æ©å«|ææ¥æ©å«ï¼æ¥è¯¢æå¤©çæ©å« 10.
-è¯¾è¡¨å¸®å©ï¼è·åè¯¾è¡¨å¸®å© æªå®å¾ç»­ ## ææå¾ ![Image text]
+è¯¾è¡¨å¸®å©ï¼è·åè¯¾è¡¨å¸®å© æªå®å¾ç»­ ## â­ææå¾ ![Image text]
 (https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
 my_table.jpg) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
 timetable/blob/main/resource/alock_8.jpg) ![Image text](https://github.com/
 maoxig/nonebot-plugin-ai-timetable/blob/main/resource/next_class.jpg) ![Image
 text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
 someday_classes.jpg) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
 timetable/blob/main/resource/someday_classes_pic.jpg) ###
@@ -89,12 +92,14 @@
 -
 æ¯å¨èµ·å§æ¥å»ºè®®é»è®¤çå¨ä¸å³å¯ï¼å¨æ¥èµ·å§æ²¡æµè¯è¿å¯è½æbugï¼
 -
 å¦æå¯¼å¥è¯¾è¡¨åå¨å°ç±è¯¾è¡¨åä¿®æ¹äºè¯¾ç¨ï¼ç´æ¥ç»botåéæ´æ°è¯¾è¡¨å³å¯æ´æ°æ¬å°è¯¾è¡¨
 -
 å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è°æå¥½äºï¼å¯ä»¥å¯¼å¥äº
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
-resource/settings.jpg) ## è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
+resource/settings.jpg) ## ð¦è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
 å¯éæ©æ¯å¦åéå¾çä»¥é¿åé£æ§ - [x] å¢å æ´å¤çéç½®é¡¹ - [x]
-éæä»£ç  - [x] è®¢éæå®çè¯¾ - [ ] å®åæä»¶ ## å­å¨çé®é¢ 1.
+éæä»£ç  - [x] è®¢éæå®çè¯¾ - [ ] å®åæä»¶ ## ðå­å¨çé®é¢
+1.
 å°ç±è¯¾è¡¨åäº«çé¾æ¥å¤§æ¦2å¨åä¼è¿æï¼ä¼ä½¿å¾`æçè¯¾è¡¨\ä¸å¨è¯¾è¡¨`æ æ³ä½¿ç¨ï¼éè¦éæ°åäº«ï¼ä½æ¯ä»è½ä½¿ç¨æ¬å°è¯¾è¡¨ï¼ä¹å¯ä»¥æ´æ°æ¬å°è¯¾è¡¨
-2. æºå¨äººéå¯åå®æ¶ä»»å¡ä¼ä¸¢å¤± ## åæ¬¢çè¯å°±ç¹ä¸ªstarå§QAQ
+2. æºå¨äººéå¯åå®æ¶ä»»å¡ä¼ä¸¢å¤± ##
+åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§QAQ
```

### Comparing `nonebot_plugin_ai_timetable-0.3.0/nonebot_plugin_ai_timetable/__init__.py` & `nonebot_plugin_ai_timetable-0.3.2/nonebot_plugin_ai_timetable/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,81 +74,81 @@
 
 
 @someday_table.handle()
 async def _(event: MessageEvent, key: str = RegexMatched()):
     """发送某天的课表"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await someday_table.finish('你还没有导入课表喵,发送/导入课表来导入吧！', at_sender=True)
+        await someday_table.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
     else:
         if timetable_pic:
             pic = await AiTimetable.someday_table(uid=uid, key=key)
             await someday_table.finish(MessageSegment.image(pic))
         else:
             await someday_table.finish(await AiTimetable.someday_table(uid=uid, key=key))
 
 
 @renew_table.handle()  # 更新本地课表
 async def _(event: MessageEvent):
     uid = event.get_user_id()
     if uid not in userdata:
-        await renew_table.finish('你还没有导入课表喵,发送/导入课表来导入吧！', at_sender=True)
+        await renew_table.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
     else:
         msg = await AiTimetable.renew_table(uid=uid)
         await renew_table.finish(msg, at_sender=True)
 
 
 @send_next_class.handle()  # 发送本节课、以及下节课信息
 async def _(event: MessageEvent):
     uid = event.get_user_id()
     if uid not in userdata:
-        await send_next_class.finish('你还没有导入课表喵,发送/导入课表来导入吧！', at_sender=True)
+        await send_next_class.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
     else:
         msg = "现在时间是"+datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         msg += AiTimetable.now_class(uid)
         msg += AiTimetable.next_class(uid)
         await send_next_class.finish(msg, at_sender=True)
 
 
 @next_morningclass.handle()
 async def _(bot: Bot, event: MessageEvent):
     """发送早八"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await send_next_class.finish('你还没有导入课表喵,发送/导入课表来导入吧！', at_sender=True)
+        await send_next_class.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
     else:
         await AiTimetable.post_alock_morningclass(uid=uid, bot=bot, event=event)
 
 #-----------以下为定时任务----------------#
 
 
 @add_alock_someday.handle()
 async def _(bot: Bot, event: MessageEvent, key: str = RegexMatched()):
     """订阅课表"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await add_alock_someday.finish('你还没有导入课表喵,发送/导入课表来导入吧！', at_sender=True)
+        await add_alock_someday.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
     else:
         if scheduler:
             send_day = (AiTimetable.weekday_int(key)+5) % 7
             if scheduler.get_job(str(uid+"post_alock"+str(send_day))):
-                await add_alock_someday.finish("出错了喵！你好像已经订阅过这天的课表了呢", at_sender=True)
+                await add_alock_someday.finish("出错了！你好像已经订阅过这天的课表了呢", at_sender=True)
             scheduler.add_job(AiTimetable.post_alock, "cron", hour=timetable_alock_someday, second=random.randint(0, 60), id=str(
                 uid+"post_alock"+str(send_day)), day_of_week=send_day, misfire_grace_time=60, kwargs={"key": key, "uid": uid, "bot": bot, "event": event})
             await add_alock_someday.finish("定时提醒添加成功！", at_sender=True)
         else:
             await add_alock_someday.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
 
 
 @remove_alock_someday.handle()
 async def _(bot: Bot, event: MessageEvent, key: str = RegexMatched()):
     """删除订阅课表"""
     uid = event.get_user_id()
     if uid not in userdata:
-        await add_alock_someday.finish('你还没有导入课表,发送//导入课表来导入吧！', at_sender=True)
+        await add_alock_someday.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
     else:
         if scheduler:
             send_day = (AiTimetable.weekday_int(key)+5) % 7
             if scheduler.get_job(str(uid+"post_alock"+str(send_day))):
                 scheduler.remove_job(str(uid+"post_alock"+str(send_day)))
                 await remove_alock_someday.finish("定时提醒删除成功！", at_sender=True)
             else:
@@ -159,24 +159,24 @@
 #-----------以下为订阅早八----------------#
 
 
 @add_alock_morningcalss.handle()
 async def _(bot: Bot, event: MessageEvent):
     uid = event.get_user_id()
     if uid not in userdata:
-        await add_alock_morningcalss.finish('你还没有导入课表喵,发送/导入课表来导入吧！', at_sender=True)
+        await add_alock_morningcalss.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
     else:
         if scheduler:
             if scheduler.get_job(str(uid+"post_alock_morningclass")):
-                await add_alock_morningcalss.finish("出错了喵！你好像已经订阅过早八提醒了呢", at_sender=True)
+                await add_alock_morningcalss.finish("出错了！你好像已经订阅过早八提醒了呢", at_sender=True)
             scheduler.add_job(AiTimetable.post_alock_morningclass, "cron", hour=timetable_alock_8, second=random.randint(
                 0, 60), id=str(uid+"post_alock_morningclass"), misfire_grace_time=60, kwargs={"uid": uid, "bot": bot, "event": event})
             await add_alock_morningcalss.finish("定时提醒添加成功！", at_sender=True)
         else:
-            await add_alock_morningcalss.finish("apscheduler插件未载入,无法添加定时提醒喵", at_sender=True)
+            await add_alock_morningcalss.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
 
 
 @remove_alock_morningclass.handle()
 async def _(event: MessageEvent):
     uid = event.get_user_id()
     if uid not in userdata:
         await add_alock_morningcalss.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
@@ -193,37 +193,37 @@
 
 @sub_class.handle()
 async def _(matcher:Matcher,args: Message = CommandArg()):
     if args.extract_plain_text():
         matcher.set_arg("text",args)
 
 
-@sub_class.got("text", prompt="请告诉我课程名喵~")
+@sub_class.got("text", prompt="请告诉我课程名~")
 async def sub_handler(bot: Bot, event: MessageEvent,text:str=ArgPlainText()):
     uid = event.get_user_id()
     if uid not in userdata:
         await sub_class.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
     else:
         if scheduler:
             msg = AiTimetable.sub_class(uid=uid, key=text, event=event, bot=bot)
             await sub_class.finish(msg, at_sender=True)
         else:
-            await sub_class.finish("apscheduler插件未载入,无法添加定时提醒喵", at_sender=True)
+            await sub_class.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
 
 
 @remove_sub_class.handle()
 async def _(matcher:Matcher,args: Message = CommandArg()):
     if args.extract_plain_text():
         matcher.set_arg("text",args)
 
 
-@remove_sub_class.got("text", prompt="请告诉我课程名喵~")
+@remove_sub_class.got("text", prompt="请告诉我课程名~")
 async def remove_sub_handler(event: MessageEvent,text:str=ArgPlainText()):
     uid = event.get_user_id()
     if uid not in userdata:
         await remove_sub_class.finish('你还没有导入课表,发送/导入课表来导入吧！', at_sender=True)
     else:
         if scheduler:
             msg = AiTimetable.remove_sub_class(uid=uid, key=text)
             await remove_sub_class.finish(msg, at_sender=True)
         else:
-            await remove_sub_class.finish("apscheduler插件未载入,无法添加定时提醒喵", at_sender=True)
+            await remove_sub_class.finish("apscheduler插件未载入,无法添加定时提醒", at_sender=True)
```

### Comparing `nonebot_plugin_ai_timetable-0.3.0/nonebot_plugin_ai_timetable/utils.py` & `nonebot_plugin_ai_timetable-0.3.2/nonebot_plugin_ai_timetable/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import random
 
 
 config = get_driver().config
 timetable_pic: bool = getattr(config, "timetable_pic", True)
 timetable_alock_someday: int = getattr(config, "timetable_alock_someday", 22)
 timetable_alock_8: int = getattr(config, "timetable_alock_8", 21)
-timetable_send_time:int=getattr(config,"timetable_send_time",0.5)
+timetable_send_time:float=getattr(config,"timetable_send_time",0.5)
 
 if os.path.exists("data/ai_timetable/userdata.json"):
     with open("data/ai_timetable/userdata.json", 'r', encoding='utf-8') as f:
         userdata = json.load(f)
 else:
     if not os.path.exists("data/ai_timetable"):
         os.makedirs("data/ai_timetable")
@@ -78,15 +78,15 @@
             if str(presentweek) in courses["weeks"].split(",") and today == courses["day"]:
                 next_class_section = int(courses["sections"].split(",")[0])
                 next_class_section_end = int(
                     courses["sections"].split(",")[-1])
                 if eval(usertable[uid]["data"]["setting"]["sectionTimes"])[next_class_section-1]["s"] > now_time:
                     return "\n你今天的下一节课程信息为：\n"+eval(usertable[uid]["data"]["setting"]["sectionTimes"])[next_class_section-1]["s"]+"-"+eval(usertable[uid]["data"]["setting"]["sectionTimes"])[next_class_section_end-1]["e"]+"\n"+courses["name"]+"\n@"+courses["position"]+"\n"+courses["teacher"]
                 #这里是因为之前已经按照顺序排好了课程,所以第一个找到的就是下节课
-        return "\n你今天接下来没有课了呢,好好享受吧喵~"
+        return "\n你今天接下来没有课了呢,好好休息吧"
     @classmethod
     def now_class(cls, uid) -> str:
         """ 
         构造出当前课程信息
         """
         presentweek = int((time.time() - int(
             usertable[uid]["data"]["setting"]['startSemester'][0:10]))//604800)+1
@@ -97,21 +97,21 @@
         for course_time in eval(usertable[uid]["data"]["setting"]["sectionTimes"]):
             if course_time["s"] < now_time < course_time["e"]:
                 now_section = course_time["i"]
         if now_section:
             count = 0
             for courses in usertable[uid]["data"]["courses"]:
                 if (str(presentweek) in courses["weeks"].split(",")) and (today == courses["day"]) and (str(now_section) in courses["sections"].split(",")):
-                    msg += "\n你现在在上的课程信息如下喵:\n"+eval(usertable[uid]["data"]["setting"]["sectionTimes"])[int(courses["sections"].split(",")[0])-1]["s"]+"-"+eval(
+                    msg += "\n你现在在上的课程信息如下:\n"+eval(usertable[uid]["data"]["setting"]["sectionTimes"])[int(courses["sections"].split(",")[0])-1]["s"]+"-"+eval(
                         usertable[uid]["data"]["setting"]["sectionTimes"])[int(courses["sections"].split(",")[-1])-1]["e"]+'\n'+courses["name"]+"\n@"+courses["position"]+"\n"+courses["teacher"]
                     count += 1
             if not count:
-                msg += "\n你现在没有课呢,空闲时间好好休息吧喵~"
+                msg += "\n你现在没有课呢,空闲时间好好休息吧"
         else:
-            msg += "\n你现在没有课呢,空闲时间好好休息吧喵~"
+            msg += "\n你现在没有课呢,空闲时间好好休息吧"
         return msg
     @classmethod
     def table_msg(cls, key, uid) -> str:
         """
         构造今日课表信息
         """
         presentweek = int((time.time() - int(
@@ -124,15 +124,15 @@
         elif someday > 7:
             someday -= 7
             presentweek += 1
             # 构造发送的信息
         if timetable_pic:
             msg = "|时间|课程|地点|\n| :-----| :----: | :----: |"
         else:
-            msg = "你要的课表来咯喵"
+            msg = "课表来了~"
         for courses in usertable[uid]["data"]["courses"]:
             if(courses["day"] == someday) and (str(presentweek) in courses["weeks"].split(',')):
 
                 sections = courses["sections"].split(",")
                 startsection = int(sections[0])
                 endsection = int(sections[-1])
                 starttime = eval(usertable[uid]["data"]["setting"]["sectionTimes"])[
@@ -191,15 +191,15 @@
                         usertable.update({uid:res.json()})
                         #更新课表
                         usertable[uid]["data"]["courses"].sort(
                     key=lambda x: int(x["sections"].split(",")[0]))
                         #对课表排序
                         await cls.write_table()
                         await cls.write_data()
-                        return "成功导入课表喵"
+                        return "成功导入课表！"
                 else:
                     return "出错了，可能是没有在小爱课表内登录账户"
         except Exception as e:
             logger.warning(f"获取课表时出错：{e}")
             return f"出错了：{e}"
             
     @classmethod
@@ -211,17 +211,17 @@
                 usertable.update({uid:res.json()})
                         #更新课表
                 usertable[uid]["data"]["courses"].sort(
                     key=lambda x: int(x["sections"].split(",")[0]))
                         #对课表排序
                 await cls.write_table()
                 await cls.write_data()
-                return "更新成功喵"
+                return "更新成功"
         except Exception as e:
-            return f"出错了喵：{e}"
+            return f"{e}"
 
     @classmethod
     async def someday_table(cls,uid,key): 
         """某天的课表"""
         try:
             msg=cls.table_msg(uid=uid,key=key)
             if not timetable_pic:
@@ -239,26 +239,26 @@
             someday=cls.weekday_int("明")
             someweek=int((time.time() - int(
                 usertable[uid]["data"]["setting"]['startSemester'][0:10]))//604800)
             if someday==8:#星期天发送时时第二天是星期一,周数加1
                 someday=1
                 someweek=someweek+1  
             count=0
-            msg="我来了喵!"
+            msg = "现在时间是"+datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             for courses in usertable[uid]["data"]["courses"]:
                 if (courses["day"] == someday) and str(someweek) in courses["weeks"].split(",") and "1" in courses["sections"].split(","):
                     count+=1
                     msg+='\n'+courses["name"] + '\n@' + courses["position"]+'\n'+courses["teacher"]
             if count==0:
                 msg+="\n你明天没有早八呢！享受夜生活吧！"
             else:
                 msg+=f"\n你明天有{count}节早八呢！今晚早点休息吧！"
             await bot.send(event,message=msg,at_sender=True)
         except ActionFailed as e:
-            logger.warning(f"发送消息给{event.get_user_id}失败：{e}")
+            logger.warning(f"发送消息给{event.get_user_id()}失败：{e}")
     @classmethod
     async def post_alock(cls,**kwargs):
         """发送第二天课程消息"""
         key,uid,bot,event=kwargs["key"],kwargs["uid"],kwargs["bot"],kwargs["event"]
         if "一" in key:
             key="明"
         msg=cls.table_msg(key=key,uid=uid)
@@ -280,48 +280,44 @@
             # 遍历当前天的所有存在的课
             if key in courses["name"]:
                 i+=1
                 if scheduler.get_job(job_id=uid+courses["name"]+str(i)):
                     continue
                 else:
                     class_section = int(courses["sections"].split(",")[0])
-                    starttime = eval(usertable[uid]["data"]["setting"]["sectionTimes"])[
-                        class_section-1]["s"]#获取课程开始时间
+                    starttime = eval(usertable[uid]["data"]["setting"]["sectionTimes"])[class_section-1]["s"]#获取课程开始时间
                     hours = int(timetable_send_time)#从设置中获取提前的小时数
                     minutes = int((timetable_send_time - hours) * 60)#从设置中获取提前的分钟数
                     time_obj = datetime.datetime.strptime(starttime, "%H:%M")#将字符串转换为datetime
                     new_time_obj = time_obj - datetime.timedelta(hours=hours, minutes=minutes)#进行时间的运算
                     sub_hour=new_time_obj.hour#获取发送时间的小时
                     sub_minute=new_time_obj.minute#获取发送时间的分钟
-                    sub_day=courses["day"]
-                    scheduler.add_job(cls.send_sub_class,"cron",id=uid+courses["name"]+str(i), hour=sub_hour, minute=sub_minute, day_of_week=sub_day, second=random.randint(
-                        0, 60), misfire_grace_time=60, kwargs={"uid": uid, "bot": bot, "event": event,"course":{"name":courses["name"],"position":courses["position"],"teacher":courses["teacher"]}})
-        return f"成功订阅了{i}节课喵~"
+                    sub_day=courses["day"]-1
+                    scheduler.add_job(cls.send_sub_class,"cron",id=uid+courses["name"]+str(i), hour=sub_hour, minute=sub_minute, day_of_week=sub_day, second=random.randint(0, 60), misfire_grace_time=60, kwargs={"uid": uid, "bot": bot, "event": event,"course":{"name":courses["name"],"position":courses["position"],"teacher":courses["teacher"]}})
+        return f"成功订阅了{i}节课~"
     
     @classmethod
     def remove_sub_class(cls,**kwargs):
         uid,key=kwargs["uid"],kwargs["key"]
         i=0
         for courses in usertable[uid]["data"]["courses"]:
             # 遍历当前天的所有存在的课
             if key in courses["name"]:
                 i+=1
                 if scheduler.get_job(job_id=uid+courses["name"]+str(i)):
                     scheduler.remove_job(job_id=uid+courses["name"]+str(i))
                 else:
                     continue
-                
-                
-        return f"成功取消订阅{i}节课喵~"
+        return f"成功取消订阅{i}节课~"
     @classmethod
     async def send_sub_class(cls,**kwargs):
         """发送订阅课程"""
         uid,bot,event,course=kwargs["uid"],kwargs["bot"],kwargs["event"],kwargs["course"]
         try:
             msg = "现在时间是"+datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-            msg+="\n还有{}小时，你订阅的课程就要开始啦！课程信息如下喵：\n{}\n{}\n{}".format(timetable_send_time,course["name"],course["position"],course["teacher"])
+            msg+="\n还有{}小时，你订阅的课程就要开始啦！课程信息如下:\n{}\n{}\n{}".format(timetable_send_time,course["name"],course["position"],course["teacher"])
             await bot.send(event, message=MessageSegment.at(uid)+msg, at_sender=True)
         except ActionFailed as e:
-            logger.warning(f"发送消息给{event.get_user_id}失败：{e}")
+            logger.warning(f"发送消息给{event.get_user_id()}失败：{e}")
```

### Comparing `nonebot_plugin_ai_timetable-0.3.0/PKG-INFO` & `nonebot_plugin_ai_timetable-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ai-timetable
-Version: 0.3.0
+Version: 0.3.2
 Summary: 小爱课程表
 Author: maoxiog
 Author-email: 674550338@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -29,58 +29,58 @@
 <div align="left">
   
 # 前言
 
    这是本人第一次在github发布的项目，也是第一个python项目，完全是萌新，很多地方写的可能很拉，大佬轻喷
 目前还不是很完善，有什么bug或者建议欢迎提issues
 
-## 安装
+## 💿安装
 
 1. 通过`pip`或`nb`安装；
     - 使用nb(极度推荐)
   
        在机器人目录下命令行使用`nb plugin install nonebot_plugin_ai_timetable`
 
     - 使用pip(不推荐):
   
       ~~既然不推荐就不要想着这样安装了啊喂~~
 
 2. 本地数据保存在`data/ai_timetable/userdata.json`以及`data/ai_timetable/usertable.json`，分别对应用户发送的链接和本地保存的课表
 
-## 简介
+## 📖简介
 
 1. 傻瓜式一键导入小爱课表，让你的bot实现小爱课表的功能
 
 2. 用户课表数据隔离，无需担心课程时间冲突、不同学校课表不同等问题
 
 3. ~~所以为什么不直接用小爱课表呢~~
 
-4. 插件配置
+4. ⚙️插件配置
 
 这些配置都已设好默认值，如果想要修改配置，在机器人目录下的.env.*里面可以填写以下选项(可选)
 
 |         config          | type  | default |          example           | usage                                                                              |
 | :---------------------: | :---: | :-----: | :------------------------: | :--------------------------------------------------------------------------------- |
 |      TIMETABLE_PIC      | bool  |  true   |    TIMETABLE_PIC=false     | 可选择某日课表以图片/文字发送，默认以图片发送(true)                                |
 | TIMETABLE_ALOCK_SOMEDAY |  int  |   22    | TIMETABLE_ALOCK_SOMEDAY=15 | 订阅某日课表的发送时间，必须是0-24的数字                                           |
 |    TIMETABLE_ALOCK_8    |  int  |   21    |    TIMETABLE_ALOCK_8=16    | 订阅早八的发送时间，必须是0-24的数字.这里发送的都是第二天的，所以建议设置为18-23点 |
-|    TIMETABLE_SEND_TIME    |  int  |   0.5    |    TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
+|    TIMETABLE_SEND_TIME    |  float  |   0.5    |    TIMETABLE_SEND_TIME=1    | 订阅课程提前发送的时间，单位是`小时`，可以是整数也可以是小数，建议不要设的太大，避免出现无法预料的bug |
 
-## 依赖
+## 💿依赖
 
 ```python
 nb plugin install nonebot_plugin_htmlrender
 nb plugin install nonebot_plugin_apscheduler
 ```
 
 若不安装[nonebot_plugin_htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender)插件会无法导入在线课表
 
 不安装[nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-apscheduler)会无法使用定时任务,其他功能无影响
 
-## 更新日志
+## 🌙更新日志
 
 <details>
 <summary>点击展开</summary>
 
 - 2023-03-05:
 
     修复了无法取消订阅早八的bug
@@ -110,26 +110,31 @@
     修复订阅早八的一些bug
 
 - 2023-03-29:
 
 1. 重构了代码，优化了许多地方~~真的累死了~~
 2. 修复了一些bug，优化了体验
 3. 增加了早八|明日早八的查询
-4. 更新版本后建议重新[导入课表]，避免出现某些bug
+4. 更新版本后建议重新`导入课表`，避免出现某些bug
 
 - 2023-04-02:
 
 1. 修复bug
 2. 优化帮助图片
 3. 定时任务随机延后0-60s，防止风控
 4. 增加订阅指定课程的功能
 
+- 2023-04-14:
+
+1. 修复了订阅课程发送时间错误的bug
+2. 删去了文本中所有奇怪的口癖喵
+
 </details>
 
-## 命令
+## 🎉命令
 
 1. 我的课表|小爱课表|本周课表|下周课表：获取本周|下周的完全课表，使用前须先导入课表，这里的课表是在线课表
 
 2. 导入课表：需要有小爱课表分享出来的链接，打开小爱课程表，手动添加课程或从教务导入(已适配了大部分高校)课程后
 
     ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 
@@ -149,15 +154,15 @@
 
 9. 早八|明日早八：查询明天的早八
 
 10. 课表帮助：获取课表帮助
 
 未完待续
 
-## 效果图
+## ⭐效果图
 
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/my_table.jpg)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/alock_8.jpg)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/next_class.jpg)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/someday_classes.jpg)
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/someday_classes_pic.jpg)
 
@@ -171,29 +176,29 @@
 - 课表节数按自己需求调，一般教务导入的课表节数可能不符合实际，需要微调
 - 每周起始日建议默认的周一即可（周日起始没测试过可能有bug）
 - 如果导入课表后在小爱课表内修改了课程，直接给bot发送更新课表即可更新本地课表
 - 当你主页的课表和学校课表基本一致时，那么小爱课程表就被调教好了，可以导入了
 
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/settings.jpg)
 
-## 计划
+## 🐦计划
 
 - [x] 查询下节课的信息
 
 - [x] 可选择是否发送图片以避免风控
 
 - [x] 增加更多的配置项
 
 - [x] 重构代码
 
 - [x] 订阅指定的课
 
 - [ ] 完善插件
 
-## 存在的问题
+## 🐛存在的问题
 
  1. 小爱课表分享的链接大概2周后会过期，会使得`我的课表\下周课表`无法使用，需要重新分享，但是仍能使用本地课表，也可以更新本地课表
 
  2. 机器人重启后定时任务会丢失
 
-## 喜欢的话就点个star吧QAQ
+## 喜欢的话就点个star✨吧QAQ
```

#### html2text {}

```diff
@@ -1,68 +1,71 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.3.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ai-timetable Version: 0.3.2 Summary:
 å°ç±è¯¾ç¨è¡¨ Author: maoxiog Author-email: 674550338@qq.com Requires-Python:
 >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0) Requires-Dist: nonebot-
 plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-htmlrender
 (>=0.2.0,<0.3.0) Requires-Dist: nonebot2 (>=2.0.0rc1,<3.0.0) Description-
 Content-Type: text/markdown
                                    [nonebot]
                          # nonebot-plugin-ai-timetable
             â¨*åºäºNonebot2çå¯¹æ¥å°ç±è¯¾ç¨è¡¨çæä»¶*â¨
 # åè¨
 è¿æ¯æ¬äººç¬¬ä¸æ¬¡å¨githubåå¸çé¡¹ç®ï¼ä¹æ¯ç¬¬ä¸ä¸ªpythoné¡¹ç®ï¼å®å¨æ¯èæ°ï¼å¾å¤å°æ¹åçå¯è½å¾æï¼å¤§ä½¬è½»å·
-ç®åè¿ä¸æ¯å¾å®åï¼æä»ä¹bugæèå»ºè®®æ¬¢è¿æissues ## å®è£ 1.
-éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
+ç®åè¿ä¸æ¯å¾å®åï¼æä»ä¹bugæèå»ºè®®æ¬¢è¿æissues ##
+ð¿å®è£ 1. éè¿`pip`æ`nb`å®è£ï¼ - ä½¿ç¨nb(æåº¦æ¨è)
 å¨æºå¨äººç®å½ä¸å½ä»¤è¡ä½¿ç¨`nb plugin install
 nonebot_plugin_ai_timetable` - ä½¿ç¨pip(ä¸æ¨è):
 ~~æ¢ç¶ä¸æ¨èå°±ä¸è¦æ³çè¿æ ·å®è£äºåå~~ 2.
 æ¬å°æ°æ®ä¿å­å¨`data/ai_timetable/userdata.json`ä»¥å`data/ai_timetable/
 usertable.json`ï¼åå«å¯¹åºç¨æ·åéçé¾æ¥åæ¬å°ä¿å­çè¯¾è¡¨ ##
-ç®ä» 1.
+ðç®ä» 1.
 å»çå¼ä¸é®å¯¼å¥å°ç±è¯¾è¡¨ï¼è®©ä½ çbotå®ç°å°ç±è¯¾è¡¨çåè½ 2.
 ç¨æ·è¯¾è¡¨æ°æ®éç¦»ï¼æ éæå¿è¯¾ç¨æ¶é´å²çªãä¸åå­¦æ ¡è¯¾è¡¨ä¸åç­é®é¢
-3. ~~æä»¥ä¸ºä»ä¹ä¸ç´æ¥ç¨å°ç±è¯¾è¡¨å¢~~ 4. æä»¶éç½®
+3. ~~æä»¥ä¸ºä»ä¹ä¸ç´æ¥ç¨å°ç±è¯¾è¡¨å¢~~ 4. âï¸æä»¶éç½®
 è¿äºéç½®é½å·²è®¾å¥½é»è®¤å¼ï¼å¦ææ³è¦ä¿®æ¹éç½®ï¼å¨æºå¨äººç®å½ä¸ç.env.*éé¢å¯ä»¥å¡«åä»¥ä¸éé¡¹
 (å¯é) | config | type | default | example | usage | | :--------------------
 -: | :---: | :-----: | :------------------------: | :--------------------------
 ------------------------------------------------------- | | TIMETABLE_PIC |
 bool | true | TIMETABLE_PIC=false | å¯éæ©ææ¥è¯¾è¡¨ä»¥å¾ç/
 æå­åéï¼é»è®¤ä»¥å¾çåé(true) | | TIMETABLE_ALOCK_SOMEDAY | int |
 22 | TIMETABLE_ALOCK_SOMEDAY=15 |
 è®¢éææ¥è¯¾è¡¨çåéæ¶é´ï¼å¿é¡»æ¯0-24çæ°å­ | |
 TIMETABLE_ALOCK_8 | int | 21 | TIMETABLE_ALOCK_8=16 |
 è®¢éæ©å«çåéæ¶é´ï¼å¿é¡»æ¯0-
 24çæ°å­.è¿éåéçé½æ¯ç¬¬äºå¤©çï¼æä»¥å»ºè®®è®¾ç½®ä¸º18-23ç¹ |
-| TIMETABLE_SEND_TIME | int | 0.5 | TIMETABLE_SEND_TIME=1 |
+| TIMETABLE_SEND_TIME | float | 0.5 | TIMETABLE_SEND_TIME=1 |
 è®¢éè¯¾ç¨æååéçæ¶é´ï¼åä½æ¯`å°æ¶`ï¼å¯ä»¥æ¯æ´æ°ä¹å¯ä»¥æ¯å°æ°ï¼å»ºè®®ä¸è¦è®¾çå¤ªå¤§ï¼é¿ååºç°æ æ³é¢æçbug
-| ## ä¾èµ ```python nb plugin install nonebot_plugin_htmlrender nb plugin
+| ## ð¿ä¾èµ ```python nb plugin install nonebot_plugin_htmlrender nb plugin
 install nonebot_plugin_apscheduler ``` è¥ä¸å®è£[nonebot_plugin_htmlrender]
 (https://github.com/kexue-z/nonebot-plugin-
 htmlrender)æä»¶ä¼æ æ³å¯¼å¥å¨çº¿è¯¾è¡¨ ä¸å®è£
 [nonebot_plugin_apscheduler](https://github.com/nonebot/plugin-
-apscheduler)ä¼æ æ³ä½¿ç¨å®æ¶ä»»å¡,å¶ä»åè½æ å½±å ## æ´æ°æ¥å¿
-ç¹å»å±å¼ - 2023-03-05: ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug - 2023-03-
-06: æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 2023-03-07: 1.
+apscheduler)ä¼æ æ³ä½¿ç¨å®æ¶ä»»å¡,å¶ä»åè½æ å½±å ##
+ðæ´æ°æ¥å¿  ç¹å»å±å¼ - 2023-03-05:
+ä¿®å¤äºæ æ³åæ¶è®¢éæ©å«çbug - 2023-03-06:
+æ°å¢äºç§èè®¢éè¯¾è¡¨|æ©å«çåè½ - 2023-03-07: 1.
 ä¿®å¤äºæ¶é´ä¸ä¼èªå·±æ¹åçbug 2. æ°å¢äºä¸è¯¾/ä¸èè¯¾ åè½ 3.
 ä¼åäºä¸äºå±å±±ä»£ç  - 2023-03-08: 1.
 ä¿®æ¹é¨åä»£ç ï¼ä¼åè¯¾è¡¨æ ¼å¼ 2.
 ä¿®å¤äºèæ°ä¸º11çè¯¾ä¼æå¨èæ°ä¸º2çè¯¾ç¨åé¢çbug
 (QAQå¤ªè ¢äºå«éªäºå«éªäº) - 2023-03-11: 1.
 ä¿®å¤äºå¦ææªç»å½å°ç±³è´¦æ·å°±åäº«è¯¾è¡¨æ¶çæ¥é,å¢å éè¯¯æç¤º
 2.
 æ°å¢3é¡¹éç½®é¡¹ï¼ææ¥è¯¾è¡¨å¯éæ©ä»¥å¾çåéï¼é»è®¤ä¸ºå¾çï¼
 - 2023-03-13ï¼ ä¿®å¤è®¢éæ©å«çä¸äºbug - 2023-03-29: 1.
 éæäºä»£ç ï¼ä¼åäºè®¸å¤å°æ¹~~ççç´¯æ­»äº~~ 2.
 ä¿®å¤äºä¸äºbugï¼ä¼åäºä½éª 3. å¢å äºæ©å«|ææ¥æ©å«çæ¥è¯¢
-4. æ´æ°çæ¬åå»ºè®®éæ°[å¯¼å¥è¯¾è¡¨]ï¼é¿ååºç°æäºbug - 2023-04-
+4. æ´æ°çæ¬åå»ºè®®éæ°`å¯¼å¥è¯¾è¡¨`ï¼é¿ååºç°æäºbug - 2023-04-
 02: 1. ä¿®å¤bug 2. ä¼åå¸®å©å¾ç 3. å®æ¶ä»»å¡éæºå»¶å0-
-60sï¼é²æ­¢é£æ§ 4. å¢å è®¢éæå®è¯¾ç¨çåè½  ## å½ä»¤ 1.
+60sï¼é²æ­¢é£æ§ 4. å¢å è®¢éæå®è¯¾ç¨çåè½ - 2023-04-14: 1.
+ä¿®å¤äºè®¢éè¯¾ç¨åéæ¶é´éè¯¯çbug 2.
+å å»äºææ¬ä¸­ææå¥æªçå£çåµ  ## ðå½ä»¤ 1.
 æçè¯¾è¡¨|å°ç±è¯¾è¡¨|æ¬å¨è¯¾è¡¨|ä¸å¨è¯¾è¡¨ï¼è·åæ¬å¨|ä¸å¨çå®å¨è¯¾è¡¨ï¼ä½¿ç¨åé¡»åå¯¼å¥è¯¾è¡¨ï¼è¿éçè¯¾è¡¨æ¯å¨çº¿è¯¾è¡¨
 2.
 å¯¼å¥è¯¾è¡¨ï¼éè¦æå°ç±è¯¾è¡¨åäº«åºæ¥çé¾æ¥ï¼æå¼å°ç±è¯¾ç¨è¡¨ï¼æå¨æ·»å è¯¾ç¨æä»æå¡å¯¼å¥
 (å·²ééäºå¤§é¨åé«æ ¡)è¯¾ç¨å ![Image text](https://github.com/maoxig/
 nonebot-plugin-ai-timetable/blob/main/resource/export.jpg)
 å¨åºæ¬è®¾ç½®éæå¼å§ä¸è¯¾æ¶é´ç­è°æ´å¥½ä¹å
 (å°¤å¶æ¯æ¶é´ãèæ°)ï¼æåäº«è¯¾è¡¨å¾å°çé¾æ¥åéç»botå³å¯å¯¼å¥æ¬å°
@@ -78,15 +81,15 @@
 (å¯ä¿®æ¹)æéä½ ç¬¬äºå¤©æ¯å¦ææ©å«ï¼ä»¥ä¾¿å³å®ä»ææ¯å¦å¨ç®ï¼å¤å®ä¾æ®æ¯æ¯å¦å­å¨ç¬¬ä¸èè¯¾ï¼
 7. è®¢é|åæ¶è®¢éè¯¾ç¨
 xxxï¼è®¢éè¯¾ç¨åï¼ä¼è®©botå¨ææåç§°éåå«xxxçè¯¾ç¨å¼å§å0.5å°æ¶
 (å¯ä¿®æ¹)åéæéï¼å¦è®¢éè¯¾ç¨
 æ°å­¦åæï¼åæ°å­¦åæåæ°å­¦åæä¹ é¢è¯¾çè¯¾å0.5å°æ¶ä¼èªå¨ååºæé
 8. ä¸è¯¾|ä¸èè¯¾ï¼è·åå½åä¸è¯¾ä¿¡æ¯ï¼è¿åä¸èè¯¾ä¿¡æ¯
 (å¦ææ) 9. æ©å«|ææ¥æ©å«ï¼æ¥è¯¢æå¤©çæ©å« 10.
-è¯¾è¡¨å¸®å©ï¼è·åè¯¾è¡¨å¸®å© æªå®å¾ç»­ ## ææå¾ ![Image text]
+è¯¾è¡¨å¸®å©ï¼è·åè¯¾è¡¨å¸®å© æªå®å¾ç»­ ## â­ææå¾ ![Image text]
 (https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
 my_table.jpg) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
 timetable/blob/main/resource/alock_8.jpg) ![Image text](https://github.com/
 maoxig/nonebot-plugin-ai-timetable/blob/main/resource/next_class.jpg) ![Image
 text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/resource/
 someday_classes.jpg) ![Image text](https://github.com/maoxig/nonebot-plugin-ai-
 timetable/blob/main/resource/someday_classes_pic.jpg) ###
@@ -99,12 +102,14 @@
 -
 æ¯å¨èµ·å§æ¥å»ºè®®é»è®¤çå¨ä¸å³å¯ï¼å¨æ¥èµ·å§æ²¡æµè¯è¿å¯è½æbugï¼
 -
 å¦æå¯¼å¥è¯¾è¡¨åå¨å°ç±è¯¾è¡¨åä¿®æ¹äºè¯¾ç¨ï¼ç´æ¥ç»botåéæ´æ°è¯¾è¡¨å³å¯æ´æ°æ¬å°è¯¾è¡¨
 -
 å½ä½ ä¸»é¡µçè¯¾è¡¨åå­¦æ ¡è¯¾è¡¨åºæ¬ä¸è´æ¶ï¼é£ä¹å°ç±è¯¾ç¨è¡¨å°±è¢«è°æå¥½äºï¼å¯ä»¥å¯¼å¥äº
 ![Image text](https://github.com/maoxig/nonebot-plugin-ai-timetable/blob/main/
-resource/settings.jpg) ## è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
+resource/settings.jpg) ## ð¦è®¡å - [x] æ¥è¯¢ä¸èè¯¾çä¿¡æ¯ - [x]
 å¯éæ©æ¯å¦åéå¾çä»¥é¿åé£æ§ - [x] å¢å æ´å¤çéç½®é¡¹ - [x]
-éæä»£ç  - [x] è®¢éæå®çè¯¾ - [ ] å®åæä»¶ ## å­å¨çé®é¢ 1.
+éæä»£ç  - [x] è®¢éæå®çè¯¾ - [ ] å®åæä»¶ ## ðå­å¨çé®é¢
+1.
 å°ç±è¯¾è¡¨åäº«çé¾æ¥å¤§æ¦2å¨åä¼è¿æï¼ä¼ä½¿å¾`æçè¯¾è¡¨\ä¸å¨è¯¾è¡¨`æ æ³ä½¿ç¨ï¼éè¦éæ°åäº«ï¼ä½æ¯ä»è½ä½¿ç¨æ¬å°è¯¾è¡¨ï¼ä¹å¯ä»¥æ´æ°æ¬å°è¯¾è¡¨
-2. æºå¨äººéå¯åå®æ¶ä»»å¡ä¼ä¸¢å¤± ## åæ¬¢çè¯å°±ç¹ä¸ªstarå§QAQ
+2. æºå¨äººéå¯åå®æ¶ä»»å¡ä¼ä¸¢å¤± ##
+åæ¬¢çè¯å°±ç¹ä¸ªstarâ¨å§QAQ
```

