# Comparing `tmp/nonebot_plugin_bilifan-0.1.1.tar.gz` & `tmp/nonebot_plugin_bilifan-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilifan-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_bilifan-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_bilifan-0.1.1.tar` & `nonebot_plugin_bilifan-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2023-04-13 11:46:28.243648 nonebot_plugin_bilifan-0.1.1/LICENSE
--rw-r--r--   0        0        0     5992 2023-04-23 12:29:18.448941 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/__init__.py
--rw-r--r--   0        0        0     4993 2023-04-13 14:32:49.994527 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/login/__init__.py
--rw-r--r--   0        0        0     4458 2023-04-19 14:35:41.509222 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/main.py
--rw-r--r--   0        0        0       54 2023-04-13 11:46:28.244641 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/src/__init__.py
--rw-r--r--   0        0        0    17462 2023-04-13 14:33:29.648335 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/src/api.py
--rw-r--r--   0        0        0    17061 2023-04-13 14:33:35.987716 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/src/user.py
--rw-r--r--   0        0        0     2230 2023-04-19 14:34:33.086319 nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/users.yaml
--rw-r--r--   0        0        0     1099 2023-04-23 12:18:53.173460 nonebot_plugin_bilifan-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2043 2023-04-16 08:57:26.125573 nonebot_plugin_bilifan-0.1.1/README.md
--rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.1/setup.py
--rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-13 11:46:28.243648 nonebot_plugin_bilifan-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6582 2023-04-30 14:24:58.392580 nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/__init__.py
+-rw-r--r--   0        0        0     4993 2023-04-13 14:32:49.994527 nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/login/__init__.py
+-rw-r--r--   0        0        0     4458 2023-04-19 14:35:41.509222 nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/main.py
+-rw-r--r--   0        0        0       54 2023-04-13 11:46:28.244641 nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/src/__init__.py
+-rw-r--r--   0        0        0    17462 2023-04-13 14:33:29.648335 nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/src/api.py
+-rw-r--r--   0        0        0    17061 2023-04-13 14:33:35.987716 nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/src/user.py
+-rw-r--r--   0        0        0     2230 2023-04-19 14:34:33.086319 nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/users.yaml
+-rw-r--r--   0        0        0     1099 2023-04-30 14:15:03.477793 nonebot_plugin_bilifan-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2107 2023-04-30 14:25:56.065573 nonebot_plugin_bilifan-0.1.2/README.md
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.2/setup.py
+-rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_bilifan-0.1.1/LICENSE` & `nonebot_plugin_bilifan-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/__init__.py` & `nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import yaml
 
 from .main import *
 from .src import BiliUser
 from .login import get_tv_qrcode_url_and_auth_code,draw_QR,verify_login
 
 from nonebot.log import logger
+from nonebot.permission import SUPERUSER
 from nonebot import on_command
 from nonebot import require,get_bot,get_driver
 from nonebot.matcher import Matcher
 from nonebot.adapters.onebot.v11 import MessageSegment,MessageEvent,Message,GroupMessageEvent,PrivateMessageEvent
 from nonebot.params import CommandArg,RawCommand,CommandStart
 from nonebot.plugin import PluginMetadata
 try:
@@ -23,15 +24,15 @@
 logger.opt(colors=True).info(
     "已检测到软依赖<y>nonebot_plugin_apscheduler</y>, <g>开启定时任务功能</g>"
     if scheduler
     else "未检测到软依赖<y>nonebot_plugin_apscheduler</y>，<r>禁用定时任务功能</r>"
 )
 
 driver = get_driver()
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __plugin_meta__ = PluginMetadata(
     name="bilifan",
     description='b站粉丝牌~',
     usage='自动刷b站粉丝牌',
     extra={
         "version": __version__,
         "author": "Agnes-Digital <Z735803792@163.com>",
@@ -104,33 +105,40 @@
     with CONFIG_PATH.open('r', encoding='utf-8') as f:
         return yaml.safe_load(f) or {}
 
 def save_config(data):
     with CONFIG_PATH.open('w', encoding='utf-8') as f:
         yaml.safe_dump(data, f, allow_unicode=True, default_flow_style=False)
 
+
+
     
 fan_once = on_command('addfan',aliases={'自动粉丝牌'},priority=40,block=False)
 @fan_once.handle()
 async def _(matcher:Matcher,event:MessageEvent,start:str = CommandStart(),command: str = RawCommand()):
     if start:
         command = command.replace(start,'')
     config = load_config()
     if isinstance(event, GroupMessageEvent):
         group_id = event.group_id
     else:
         group_id = event.user_id
-    if event.user_id in config:
-        del config[event.user_id]
-        save_config(config)
-        await matcher.finish(f'已删除{event.user_id}的定时任务')
+        
+    msg_path = Path().joinpath(f'data/bilifan/{event.user_id}/login_info.txt')   
+    if msg_path.is_file: 
+        if event.user_id in config:
+            del config[event.user_id]
+            save_config(config)
+            await matcher.finish(f'已删除{event.user_id}的定时任务')
+        else:
+            config[event.user_id] = group_id
+            save_config(config)
+            await matcher.finish(f'已增加{event.user_id}的定时任务，每天0点执行')
     else:
-        config[event.user_id] = group_id
-        save_config(config)
-        await matcher.finish(f'已增加{event.user_id}的定时任务，每天0点执行')
+        await matcher.finish('你尚未登录，请输入【b站登录】')
         
         
 async def auto_cup():
     config = load_config()
     count = {}
     for user_id, group_id in config.items():
         msg_path = Path().joinpath(f'data/bilifan/{user_id}/login_info.txt')
@@ -147,17 +155,26 @@
         else:
             count_value = count.get(group_id, 0)
             count[group_id] = count_value + 1 
     if count:
         for group_id,num in count.items():
             await get_bot().send_group_msg(group_id=group_id, message=f'今日已完成{num}个自动刷牌子任务')
 
+del_all = on_command('bdel',aliases={'删除全部刷牌子'},block=False,permission=SUPERUSER)
+@del_all.handle()
+async def _(matcher:Matcher):
+    msg_path = Path().joinpath('data/bilifan/config.yaml')
+    os.remove(msg_path)
+    matcher.finish('已删除全部定时刷牌子任务')
+
+
 @driver.on_bot_connect
 async def _():
     users = await read_yaml(Path().joinpath('data/bilifan'))
     cron = users.get('CRON', None)
     try:
         fields = cron.split(" ")
     except AttributeError:
         logger.error('定时格式不正确，不启用定时功能')
         return
-    scheduler.add_job(auto_cup, "cron", hour=fields[0], minute=fields[1],id="auto_cup")
+    scheduler.add_job(auto_cup, "cron", hour=fields[0], minute=fields[1],id="auto_cup")
+
```

### Comparing `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/login/__init__.py` & `nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/login/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/main.py` & `nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/src/api.py` & `nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/src/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/src/user.py` & `nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/src/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.1/nonebot_plugin_bilifan/users.yaml` & `nonebot_plugin_bilifan-0.1.2/nonebot_plugin_bilifan/users.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.1.1/pyproject.toml` & `nonebot_plugin_bilifan-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bilifan"
-version = "0.1.1"
+version = "0.1.2"
 description = "刷bili粉丝牌子的机器人插件"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["bilibili", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_bilifan-0.1.1/README.md` & `nonebot_plugin_bilifan-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件
 
 ## 指令
 
  - b站登录 - 返回b站二维码，扫码登录，绑定qq号
  - 开始刷牌子 - 开始执行命令
  - 自动刷牌子 - 添加或取消定时任务
+ - 删除全部刷牌子 - [超管]删除全部的定时任务
 
 
 </details>
 
 ## 🙈 其他
 
 + 如果本插件对你有帮助，不要忘了点个Star~
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨_ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## éç½® å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶ ## æä»¤ - bç«ç»å½
 - è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å¼å§å·çå­ -
-å¼å§æ§è¡å½ä»¤ - èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡  ## ð
-å¶ä» + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
+å¼å§æ§è¡å½ä»¤ - èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡ -
+å é¤å¨é¨å·çå­ - [è¶ç®¡]å é¤å¨é¨çå®æ¶ä»»å¡  ## ð å¶ä» +
+å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [ç±åçµ](https://
 afdian.net/a/agnes_digital) + [GPL-3.0 License](https://github.com/Agnes4m/
 nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m](https://github.com/
 Agnes4m) ## ð æè°¢ - [æ° B ç«ç²ä¸çå©æ](https://github.com/
 XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»
```

### Comparing `nonebot_plugin_bilifan-0.1.1/setup.py` & `nonebot_plugin_bilifan-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'nonebot_plugin_apscheduler>=0.2.0',
  'pillow>=9.3.0,<10.0.0',
  'pyyaml>=6.0,<7.0',
  'qrcode>=7.4.2,<8.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-bilifan',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '刷bili粉丝牌子的机器人插件',
-    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_bilifan\n_✨自动b站粉丝牌✨_\n\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_bilifan" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_bilifan" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_bilifan">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_bilifan.svg" alt="pypi">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc4-red.svg" alt="NoneBot">\n</div>\n\n\n## 配置\n\n启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件\n\n## 指令\n\n - b站登录 - 返回b站二维码，扫码登录，绑定qq号\n - 开始刷牌子 - 开始执行命令\n - 自动刷牌子 - 添加或取消定时任务\n\n\n</details>\n\n## 🙈 其他\n\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [爱发电](https://afdian.net/a/agnes_digital)\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n## 🌐 感谢\n\n- [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他\n',
+    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_bilifan\n_✨自动b站粉丝牌✨_\n\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_bilifan" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_bilifan" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_bilifan">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_bilifan.svg" alt="pypi">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc4-red.svg" alt="NoneBot">\n</div>\n\n\n## 配置\n\n启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件\n\n## 指令\n\n - b站登录 - 返回b站二维码，扫码登录，绑定qq号\n - 开始刷牌子 - 开始执行命令\n - 自动刷牌子 - 添加或取消定时任务\n - 删除全部刷牌子 - [超管]删除全部的定时任务\n\n\n</details>\n\n## 🙈 其他\n\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [爱发电](https://afdian.net/a/agnes_digital)\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n## 🌐 感谢\n\n- [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他\n',
     'author': 'Agnes_Digital',
     'author_email': 'Z735803792@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_bilifan', 'nonebot_plugin_bilifan.login',
 'nonebot_plugin_bilifan.src'] package_data = \ {'': ['*']} install_requires = \
 ['aiohttp-socks>=0.8.0,<0.9.0', 'aiohttp>=3.8.3,<4.0.0', 'nonebot-adapter-
 onebot>=2.1.5', 'nonebot2>=2.0.0rc4,<3.0.0',
 'nonebot_plugin_apscheduler>=0.2.0', 'pillow>=9.3.0,<10.0.0',
 'pyyaml>=6.0,<7.0', 'qrcode>=7.4.2,<8.0.0'] setup_kwargs = { 'name': 'nonebot-
-plugin-bilifan', 'version': '0.1.1', 'description':
+plugin-bilifan', 'version': '0.1.2', 'description':
 'å·biliç²ä¸çå­çæºå¨äººæä»¶', 'long_description': '
                            \n [AgnesDigitalLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
     \n\n# nonebot_plugin_bilifan\n_â¨èªå¨bç«ç²ä¸çâ¨_\n\n\n_[GitHub
 stars]\n\n\n_[GitHub_issues]\n\n\n_[QQ_Chat_Group]\n\n\n_[pypi]\n\n [python]\n
                                   [NoneBot]\n
 \n\n\n## éç½®\n\nå¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶\n\n## æä»¤\n\n -
 bç«ç»å½ - è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå·\n -
 å¼å§å·çå­ - å¼å§æ§è¡å½ä»¤\n - èªå¨å·çå­ -
-æ·»å æåæ¶å®æ¶ä»»å¡\n\n\n\n\n## ð å¶ä»\n\n+
+æ·»å æåæ¶å®æ¶ä»»å¡\n - å é¤å¨é¨å·çå­ -
+[è¶ç®¡]å é¤å¨é¨çå®æ¶ä»»å¡\n\n\n\n\n## ð å¶ä»\n\n+
 å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~\n+
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é\n+ [ç±åçµ](https://
 afdian.net/a/agnes_digital)\n+ [GPL-3.0 License](https://github.com/Agnes4m/
 nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m](https://github.com/
 Agnes4m)\n \n\n## ð æè°¢\n\n- [æ° B ç«ç²ä¸çå©æ](https://
 github.com/XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»\n', 'author':
 'Agnes_Digital', 'author_email': 'Z735803792@163.com', 'maintainer': 'None',
```

### Comparing `nonebot_plugin_bilifan-0.1.1/PKG-INFO` & `nonebot_plugin_bilifan-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilifan
-Version: 0.1.1
+Version: 0.1.2
 Summary: 刷bili粉丝牌子的机器人插件
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -63,14 +63,15 @@
 启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件
 
 ## 指令
 
  - b站登录 - 返回b站二维码，扫码登录，绑定qq号
  - 开始刷牌子 - 开始执行命令
  - 自动刷牌子 - 添加或取消定时任务
+ - 删除全部刷牌子 - [超管]删除全部的定时任务
 
 
 </details>
 
 ## 🙈 其他
 
 + 如果本插件对你有帮助，不要忘了点个Star~
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.1.2 Summary:
 å·biliç²ä¸çå­çæºå¨äººæä»¶ Home-page: https://github.com/Agnes4m/
 nonebot_plugin_l4d2_server License: GPLv3 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: License :: Other/Proprietary License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -19,14 +19,15 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨_ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## éç½® å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶ ## æä»¤ - bç«ç»å½
 - è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å¼å§å·çå­ -
-å¼å§æ§è¡å½ä»¤ - èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡  ## ð
-å¶ä» + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
+å¼å§æ§è¡å½ä»¤ - èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡ -
+å é¤å¨é¨å·çå­ - [è¶ç®¡]å é¤å¨é¨çå®æ¶ä»»å¡  ## ð å¶ä» +
+å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [ç±åçµ](https://
 afdian.net/a/agnes_digital) + [GPL-3.0 License](https://github.com/Agnes4m/
 nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m](https://github.com/
 Agnes4m) ## ð æè°¢ - [æ° B ç«ç²ä¸çå©æ](https://github.com/
 XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»
```

