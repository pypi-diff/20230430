# Comparing `tmp/nonebot_plugin_megumin-0.0.4-py3-none-any.whl.zip` & `tmp/nonebot_plugin_megumin-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 6261 bytes, number of entries: 6
--rw-r--r--  2.0 fat     5175 b- defN 80-Jan-01 00:00 nonebot_plugin_megumin/__init__.py
+Zip file size: 6281 bytes, number of entries: 6
+-rw-r--r--  2.0 fat     5220 b- defN 80-Jan-01 00:00 nonebot_plugin_megumin/__init__.py
 -rw-r--r--  2.0 fat      491 b- defN 80-Jan-01 00:00 nonebot_plugin_megumin/cfg.py
--rw-r--r--  2.0 fat     2925 b- defN 80-Jan-01 00:00 nonebot_plugin_megumin/charm.py
--rw-r--r--  2.0 fat     3419 b- defN 80-Jan-01 00:00 nonebot_plugin_megumin-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 nonebot_plugin_megumin-0.0.4.dist-info/WHEEL
-?rw-r--r--  2.0 fat      515 b- defN 16-Jan-01 00:00 nonebot_plugin_megumin-0.0.4.dist-info/RECORD
-6 files, 12613 bytes uncompressed, 5323 bytes compressed:  57.8%
+-rw-r--r--  2.0 fat     2928 b- defN 80-Jan-01 00:00 nonebot_plugin_megumin/charm.py
+-rw-r--r--  2.0 fat     3419 b- defN 80-Jan-01 00:00 nonebot_plugin_megumin-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 nonebot_plugin_megumin-0.0.5.dist-info/WHEEL
+?rw-r--r--  2.0 fat      515 b- defN 16-Jan-01 00:00 nonebot_plugin_megumin-0.0.5.dist-info/RECORD
+6 files, 12661 bytes uncompressed, 5343 bytes compressed:  57.8%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: nonebot_plugin_megumin/cfg.py
 Comment: 
 
 Filename: nonebot_plugin_megumin/charm.py
 Comment: 
 
-Filename: nonebot_plugin_megumin-0.0.4.dist-info/METADATA
+Filename: nonebot_plugin_megumin-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: nonebot_plugin_megumin-0.0.4.dist-info/WHEEL
+Filename: nonebot_plugin_megumin-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: nonebot_plugin_megumin-0.0.4.dist-info/RECORD
+Filename: nonebot_plugin_megumin-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nonebot_plugin_megumin/__init__.py

```diff
@@ -4,49 +4,56 @@
 from pathlib import Path
 from .charm import *
 from .cfg import *
 import asyncio
 import random
 import time
 
-
 driver = get_driver()
+
+
 @driver.on_startup
 def 魔法文件们():
     主目录 = Path.cwd()
     魔法目录 = 主目录.joinpath("data/explosion")
 
     if not 魔法目录.exists():
         logger.info(f"\033[31m 没有找到配置目录 {魔法目录} ")
 
     AAC = list(魔法目录.glob("*.aac"))
-    if len(AAC) == 0:
+    if not AAC:
         logger.info(f"\033[31m 配置目录 {魔法目录} 中没有音频文件 ")
 
     MP4 = list(魔法目录.glob("*.mp4"))
-    if len(MP4) == 0:
+    if not MP4:
         logger.info(f"\033[31m 配置目录 {魔法目录} 中没有视频文件 ")
 
+
 玩家吟唱 = {}
 补魔次数 = {}
 视频次数 = {}
 无魔防刷屏 = {}
 
-ex = on_command("爆裂魔法", aliases = {"惠惠", "explosion", "来一发", "爆烈魔法", "暴烈魔法", "献上爆炎"}, permission=GROUP, priority=90)
+ex = on_command("爆裂魔法",
+                aliases={"惠惠", "explosion", "来一发", "爆烈魔法", "暴烈魔法", "献上爆炎"},
+                permission=GROUP,
+                priority=90)
+
+
 @ex.handle()
 async def 施法(event: GroupMessageEvent):
     玩家 = event.user_id
     群 = event.group_id
     今天 = await 时间()
 
     if 玩家吟唱.get(玩家, {}).get(今天, 0) >= 释放极限:
         if 无魔防刷屏.get(玩家, {}).get(今天, 0) >= 6:
             return
         if 补魔次数.get(玩家, {}).get(今天, 0) >= 补魔极限:
-            await ex.send(f"你今天已经施展过了，下次再来吧~")
+            await ex.send("你今天已经施展过了，下次再来吧~")
             无魔防刷屏.setdefault(玩家, {})
             无魔防刷屏[玩家][今天] = 无魔防刷屏[玩家].get(今天, 0) + 1
             return
         await ex.send(f"你今天已经释放{释放极限}次了，请恢复魔力后再来吧~")
         无魔防刷屏.setdefault(玩家, {})
         无魔防刷屏[玩家][今天] = 无魔防刷屏[玩家].get(今天, 0) + 1
         return
@@ -95,15 +102,17 @@
     await ex.send(魔咒)
 
     玩家吟唱.setdefault(玩家, {})
     玩家吟唱[玩家][今天] = 玩家吟唱[玩家].get(今天, 0) + 1
     logger.info(f"\033[32m 玩家 {玩家} 施展了一次语音爆裂魔法 ")
 
 
-exp = on_command("补魔", aliases = {"补充魔力", "恢复魔力"}, priority=90)
+exp = on_command("补魔", aliases={"补充魔力", "恢复魔力"}, priority=90)
+
+
 @exp.handle()
 async def 恢复(event: GroupMessageEvent):
     玩家 = event.user_id
 
     今天 = await 时间()
 
     if 补魔次数.get(玩家, {}).get(今天, 0) >= 补魔极限:
@@ -118,21 +127,24 @@
     补魔次数.setdefault(玩家, {})
     补魔次数[玩家][今天] = 补魔次数[玩家].get(今天, 0) + 1
     logger.info(f"\033[32m 玩家 {玩家} 为自己补魔 ")
 
 
 async def 时间():
     日期 = time.localtime(time.time())
-    今天 = time.strftime("%Y-%m-%d", 日期)
-    return 今天
+    return time.strftime("%Y-%m-%d", 日期)
+
+
+exhelp = on_command("爆裂魔法帮助", aliases={"爆裂魔法help", "补魔帮助"}, priority=90)
 
 
-exhelp = on_command("爆裂魔法帮助", aliases = {"爆裂魔法help", "补魔帮助"}, priority=90)
 @exhelp.handle()
 async def 帮助(event: GroupMessageEvent):
     玩家 = event.user_id
     今天 = await 时间()
     if 无魔防刷屏.get(玩家, {}).get(今天, 0) >= 6:
         return
-    await exp.send(f"吾名惠惠！\n乃浪漫炽热【爆裂魔法】支配者\n每日{释放极限}发的惊人力量！\n以{补魔极限}次【补魔】引渡魔力本源！\n为你之群聊献上爆炎！\n『Explosion！』\n\n详细介绍：https://github.com/youlanan/nonebot_plugin_megumin")
+    await exp.send(
+        f"吾名惠惠！\n乃浪漫炽热【爆裂魔法】支配者\n每日{释放极限}发的惊人力量！\n以{补魔极限}次【补魔】引渡魔力本源！\n为你之群聊献上爆炎！\n『Explosion！』\n\n详细介绍：https://github.com/youlanan/nonebot_plugin_megumin"
+    )
     无魔防刷屏.setdefault(玩家, {})
-    无魔防刷屏[玩家][今天] = 无魔防刷屏[玩家].get(今天, 0) + 1
+    无魔防刷屏[玩家][今天] = 无魔防刷屏[玩家].get(今天, 0) + 1
```

## nonebot_plugin_megumin/cfg.py

```diff
@@ -1,8 +1,7 @@
-
 混合发送 = 2
 '''
 设置施法模式
 - 设为 2 时,该群每日首次触发时发送视频，之后为语音+文本
 - 设为 1 时，只发送视频，设为 0 时，只发送语音+文本
 '''
 
@@ -12,8 +11,8 @@
 - 关于玩家或分群的触发上限：次日自动刷新，重启后清空
 '''
 
 补魔极限 = 1
 '''
 设置每个玩家每天可自行补魔次数
 - 关于补魔上限：次日自动刷新，重启后清空
-'''
+'''
```

## nonebot_plugin_megumin/charm.py

```diff
@@ -1,29 +1,27 @@
 吟唱词 = {
-    "其一.aac":"比黑色更黑、比黑暗更暗的漆黑\n在此寄托吾真红的金光吧！\n觉醒之时已然来临\n真理坠入无缪境界\n化为无形扭曲 显现吧！\n跃动吧！起舞吧！欢涌吧！\n吾之力量洪流渴望崩坏\n渴望无可匹敌的崩坏！\n将万象化作灰烬\n自深渊降临吧！\n这正是人类最强威力的攻击手段\n这就是究极攻击魔法！\n『Explosion！！』",
-    "其二.aac":"被光明笼罩的漆黑啊\n身披夜之衣的爆炎啊\n以红魔族之名 显现原初崩坏吧！\n于终焉王国之地\n引渡力量本源之物啊!\n在吾之前展现吧！\n『Explosion！』",
-    "其三.aac":"赤红之黑炎\n万界之君王\n天地之火咆哮之时\n吾乃万象升温之理\n崩坏破坏之别名！\n业火铁锤降临吾身！\n『Explosion！！』",
-    "其四.aac":"吾名惠惠\n红魔族第一的魔法师\n兼爆裂魔法的操纵者\n好好见识我的力量吧\n『Explosion！』",
-    "其五.aac":"以吾真红之流动\n颠覆白色之世界\n『Explosion！』",
-    "其六.aac":"比黑更黑、比暗更暗的漆黑\n在此寄托吾真红的金光吧\n觉醒之时已然来临\n真理坠入无缪境界\n化为无形扭曲显现\n『Explosion！』",
-    "其七.aac":"被光明笼罩的漆黑\n藏于夜色中的爆炎\n其它的暂且不提\n说到爆裂魔法，我不想输给任何人！\n要上了\n吾之究极破坏魔法——\n『Explosion！！』",
-    "其八.aac":"现世空蝉悄然侵入反逆天楼\n于吾身前造访乃是寂静神雷\n时机已到！\n现在，\n以狂热之力惊醒沉寂，\n显现吧！贯穿一切！\n『Explosion！』",
-    "其九.aac":"环绕于我的乖逸精灵\n深渊的血肉狂然咆哮\n现在\n成为红色波动的一部分吧\n穿刺吧\n『Explosion！』",
-    "其十.aac":"吾名惠惠\n乃至高全能的支配者\n立于魔力高天上施与号令之人！\n...\n降临吧，降临吧，\n烈焰之军势啊\n回应吾之所求，显现你的力量吧\n『Explosion...\n诶？？（惠惠震惊.jpg）』",
-    "其十一.aac":"「吾名悠悠！\n红魔族第一 最强的魔法使！」\n吾名惠惠！\n红魔族第一 最强的魔法使！\n悠悠那时候挽回了我研习爆裂魔法的机会\n所以才有了今天的我！\n「因为有惠惠这位劲敌\n我才一路成长至今！\n『Light of Saber！！』」\n振翅吧风暴！嘶吼吧烈焰！\n爆裂魔法是浪漫！\n是将不可能变为可能\n最强的魔法！\n『Explosion！！』",
-    "米米.aac":"吾乃米米！\n红魔族第一的魔性妹妹\n凌驾魔王军干部之人！\n(*^ - ^*)"
-} 
+    "其一.aac":
+    "比黑色更黑、比黑暗更暗的漆黑\n在此寄托吾真红的金光吧！\n觉醒之时已然来临\n真理坠入无缪境界\n化为无形扭曲 显现吧！\n跃动吧！起舞吧！欢涌吧！\n吾之力量洪流渴望崩坏\n渴望无可匹敌的崩坏！\n将万象化作灰烬\n自深渊降临吧！\n这正是人类最强威力的攻击手段\n这就是究极攻击魔法！\n『Explosion！！』",
+    "其二.aac":
+    "被光明笼罩的漆黑啊\n身披夜之衣的爆炎啊\n以红魔族之名 显现原初崩坏吧！\n于终焉王国之地\n引渡力量本源之物啊!\n在吾之前展现吧！\n『Explosion！』",
+    "其三.aac":
+    "赤红之黑炎\n万界之君王\n天地之火咆哮之时\n吾乃万象升温之理\n崩坏破坏之别名！\n业火铁锤降临吾身！\n『Explosion！！』",
+    "其四.aac": "吾名惠惠\n红魔族第一的魔法师\n兼爆裂魔法的操纵者\n好好见识我的力量吧\n『Explosion！』",
+    "其五.aac": "以吾真红之流动\n颠覆白色之世界\n『Explosion！』",
+    "其六.aac":
+    "比黑更黑、比暗更暗的漆黑\n在此寄托吾真红的金光吧\n觉醒之时已然来临\n真理坠入无缪境界\n化为无形扭曲显现\n『Explosion！』",
+    "其七.aac":
+    "被光明笼罩的漆黑\n藏于夜色中的爆炎\n其它的暂且不提\n说到爆裂魔法，我不想输给任何人！\n要上了\n吾之究极破坏魔法——\n『Explosion！！』",
+    "其八.aac":
+    "现世空蝉悄然侵入反逆天楼\n于吾身前造访乃是寂静神雷\n时机已到！\n现在，\n以狂热之力惊醒沉寂，\n显现吧！贯穿一切！\n『Explosion！』",
+    "其九.aac": "环绕于我的乖逸精灵\n深渊的血肉狂然咆哮\n现在\n成为红色波动的一部分吧\n穿刺吧\n『Explosion！』",
+    "其十.aac":
+    "吾名惠惠\n乃至高全能的支配者\n立于魔力高天上施与号令之人！\n...\n降临吧，降临吧，\n烈焰之军势啊\n回应吾之所求，显现你的力量吧\n『Explosion...\n诶？？（惠惠震惊.jpg）』",
+    "其十一.aac":
+    "「吾名悠悠！\n红魔族第一 最强的魔法使！」\n吾名惠惠！\n红魔族第一 最强的魔法使！\n悠悠那时候挽回了我研习爆裂魔法的机会\n所以才有了今天的我！\n「因为有惠惠这位劲敌\n我才一路成长至今！\n『Light of Saber！！』」\n振翅吧风暴！嘶吼吧烈焰！\n爆裂魔法是浪漫！\n是将不可能变为可能\n最强的魔法！\n『Explosion！！』",
+    "米米.aac": "吾乃米米！\n红魔族第一的魔性妹妹\n凌驾魔王军干部之人！\n(*^ - ^*)"
+}
 
 高端吟唱体验 = [
-    "其一.mp4",
-    "其二.mp4",
-    "其三.mp4",
-    "其四.mp4",
-    "其五.mp4",
-    "其六.mp4",
-    "其七.mp4",
-    "其八.mp4",
-    "其九.mp4",
-    "其十.mp4",
-    "其十一.mp4",
-    "米米.mp4"
-]
+    "其一.mp4", "其二.mp4", "其三.mp4", "其四.mp4", "其五.mp4", "其六.mp4", "其七.mp4",
+    "其八.mp4", "其九.mp4", "其十.mp4", "其十一.mp4", "米米.mp4"
+]
```

## Comparing `nonebot_plugin_megumin-0.0.4.dist-info/METADATA` & `nonebot_plugin_megumin-0.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-megumin
-Version: 0.0.4
+Version: 0.0.5
 Summary: 让你的群友们释放爆裂魔法吧！
 Home-page: https://github.com/youlanan/nonebot_plugin_megumin
 License: MIT
 Keywords: NoneBot,Explosion
 Author: 悠岚岸
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-megumin Version: 0.0.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-megumin Version: 0.0.5 Summary:
 è®©ä½ çç¾¤åä»¬éæ¾çè£é­æ³å§ï¼ Home-page: https://github.com/
 youlanan/nonebot_plugin_megumin License: MIT Keywords: NoneBot,Explosion
 Author: æ å²å²¸ Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot-
```

