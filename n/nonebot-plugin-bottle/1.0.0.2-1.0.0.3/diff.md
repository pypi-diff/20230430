# Comparing `tmp/nonebot_plugin_bottle-1.0.0.2-py3-none-any.whl.zip` & `tmp/nonebot_plugin_bottle-1.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 27729 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat    17114 b- defN 23-Apr-29 10:07 nonebot_plugin_bottle/__init__.py
--rw-rw-rw-  2.0 fat      636 b- defN 23-Apr-29 05:06 nonebot_plugin_bottle/config.py
--rw-rw-rw-  2.0 fat    17498 b- defN 23-Apr-29 05:06 nonebot_plugin_bottle/data_source.py
--rw-rw-rw-  2.0 fat     1426 b- defN 23-Apr-29 10:05 nonebot_plugin_bottle/model.py
--rw-rw-rw-  2.0 fat     2647 b- defN 23-Apr-29 05:06 nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
--rw-rw-rw-  2.0 fat    35821 b- defN 23-Apr-29 14:44 nonebot_plugin_bottle-1.0.0.2.dist-info/LICENCE
--rw-rw-rw-  2.0 fat     8240 b- defN 23-Apr-29 14:44 nonebot_plugin_bottle-1.0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 14:44 nonebot_plugin_bottle-1.0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-29 14:44 nonebot_plugin_bottle-1.0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      939 b- defN 23-Apr-29 14:44 nonebot_plugin_bottle-1.0.0.2.dist-info/RECORD
-10 files, 84435 bytes uncompressed, 26097 bytes compressed:  69.1%
+Zip file size: 27765 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat    17112 b- defN 23-Apr-30 04:37 nonebot_plugin_bottle/__init__.py
+-rw-rw-rw-  2.0 fat      636 b- defN 23-Apr-30 04:37 nonebot_plugin_bottle/config.py
+-rw-rw-rw-  2.0 fat    17632 b- defN 23-Apr-30 04:37 nonebot_plugin_bottle/data_source.py
+-rw-rw-rw-  2.0 fat     1426 b- defN 23-Apr-30 04:37 nonebot_plugin_bottle/model.py
+-rw-rw-rw-  2.0 fat     2647 b- defN 23-Apr-30 04:37 nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
+-rw-rw-rw-  2.0 fat    35821 b- defN 23-Apr-30 05:00 nonebot_plugin_bottle-1.0.0.3.dist-info/LICENCE
+-rw-rw-rw-  2.0 fat     8240 b- defN 23-Apr-30 05:00 nonebot_plugin_bottle-1.0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-30 05:00 nonebot_plugin_bottle-1.0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-30 05:00 nonebot_plugin_bottle-1.0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      939 b- defN 23-Apr-30 05:00 nonebot_plugin_bottle-1.0.0.3.dist-info/RECORD
+10 files, 84567 bytes uncompressed, 26133 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: nonebot_plugin_bottle/model.py
 Comment: 
 
 Filename: nonebot_plugin_bottle/migrations/449e066410fd_init_db.py
 Comment: 
 
-Filename: nonebot_plugin_bottle-1.0.0.2.dist-info/LICENCE
+Filename: nonebot_plugin_bottle-1.0.0.3.dist-info/LICENCE
 Comment: 
 
-Filename: nonebot_plugin_bottle-1.0.0.2.dist-info/METADATA
+Filename: nonebot_plugin_bottle-1.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: nonebot_plugin_bottle-1.0.0.2.dist-info/WHEEL
+Filename: nonebot_plugin_bottle-1.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: nonebot_plugin_bottle-1.0.0.2.dist-info/top_level.txt
+Filename: nonebot_plugin_bottle-1.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: nonebot_plugin_bottle-1.0.0.2.dist-info/RECORD
+Filename: nonebot_plugin_bottle-1.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nonebot_plugin_bottle/__init__.py

```diff
@@ -51,15 +51,15 @@
     漂流瓶黑名单 [QQ / 群聊] [QQ号 / 群号]
     漂流瓶详情 [漂流瓶编号]
 """.strip(),
     extra={
         "unique_name": "nonebot_plugin_bottle",
         "example": "扔漂流瓶\n寄漂流瓶\n捡漂流瓶\n评论漂流瓶\n举报漂流瓶\n查看漂流瓶\n删除漂流瓶",
         "author": "Todysheep",
-        "version": "1.0.0.1",
+        "version": "1.0.0",
     },
 )
 
 throw = on_command(
     "扔漂流瓶", aliases=set(["寄漂流瓶", "丢漂流瓶"]), permission=GROUP, priority=100, block=True
 )
 get = on_command("捡漂流瓶", priority=100, block=True)
```

## nonebot_plugin_bottle/data_source.py

```diff
@@ -215,14 +215,16 @@
         for table in [
             "nonebot_plugin_bottle_bottle",
             "nonebot_plugin_bottle_comment",
             "nonebot_plugin_bottle_report",
         ]:
             if engine.name == "sqlite":
                 await session.execute(text(f"DELETE FROM {table}"))
+            elif engine.name == "postgresql":
+                await session.execute(text(f"TRUNCATE TABLE {table} RESTART IDENTITY"))
             else:
                 await session.execute(text(f"TRUNCATE TABLE {table}"))
 
     async def report(
         self, bottle: Bottle, user_id: int, session: AsyncSession, times_max: int = 5
     ) -> int:
         """
@@ -540,8 +542,8 @@
         request_url = request_url + "?access_token=" + access_token
         headers = {"content-type": "application/x-www-form-urlencoded"}
         response = await client.post(request_url, data=params, headers=headers)
         if response:
             return response.json()
         else:
             # 调用审核API失败
-            return "Error"
+            return "Error"
```

## Comparing `nonebot_plugin_bottle-1.0.0.2.dist-info/LICENCE` & `nonebot_plugin_bottle-1.0.0.3.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `nonebot_plugin_bottle-1.0.0.2.dist-info/METADATA` & `nonebot_plugin_bottle-1.0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bottle
-Version: 1.0.0.2
+Version: 1.0.0.3
 Summary: Bottle post plugin in Nonebot
 Home-page: https://github.com/Todysheep/nonebot_plugin_bottle
 Author: Todysheep
 Author-email: todysheep@163.com
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

## Comparing `nonebot_plugin_bottle-1.0.0.2.dist-info/RECORD` & `nonebot_plugin_bottle-1.0.0.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-nonebot_plugin_bottle/__init__.py,sha256=4jnBmzpBZSs6uCnAXcLjc0WFh1hQW6rUxwKQwMA9UMk,17114
+nonebot_plugin_bottle/__init__.py,sha256=4D5SLLR6sPPuEpe8OeD7I6aYqrvouF5Bt5Ogp1YeXok,17112
 nonebot_plugin_bottle/config.py,sha256=ZR5r0jPivngaixOdWe8Zq51GdVNH2eGMB2mY6g8BJb4,636
-nonebot_plugin_bottle/data_source.py,sha256=abz1ePDi3wvAKfDAv6L4kF2Wrf4UPNyddKLU5vxVRZQ,17498
+nonebot_plugin_bottle/data_source.py,sha256=xBIfCFvK0AXxLedqRHZQBjQx1hY50TxAEE_nVSn3HyE,17632
 nonebot_plugin_bottle/model.py,sha256=KOSnuuBvJJJtWPKnrvo8hvZACX1l1K4ahYLuyrXQb6A,1426
 nonebot_plugin_bottle/migrations/449e066410fd_init_db.py,sha256=GiRcKkExGH8egMyiKBLVhF1xwe8kKiZwo36fPdjPntk,2647
-nonebot_plugin_bottle-1.0.0.2.dist-info/LICENCE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
-nonebot_plugin_bottle-1.0.0.2.dist-info/METADATA,sha256=sD7Oi-Q4n-i7y_gDOoAm9VKV3090pMue-xDC2m3yR4k,8240
-nonebot_plugin_bottle-1.0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-nonebot_plugin_bottle-1.0.0.2.dist-info/top_level.txt,sha256=Q9vMfveUHJFO9CzFuJmg1yJ0jzwBs0034WbzsgQrcfw,22
-nonebot_plugin_bottle-1.0.0.2.dist-info/RECORD,,
+nonebot_plugin_bottle-1.0.0.3.dist-info/LICENCE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
+nonebot_plugin_bottle-1.0.0.3.dist-info/METADATA,sha256=hIbdPAJY6ofjthdrzBT_r-7EzR5ZKu1Xq-gu9mMUnBM,8240
+nonebot_plugin_bottle-1.0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+nonebot_plugin_bottle-1.0.0.3.dist-info/top_level.txt,sha256=Q9vMfveUHJFO9CzFuJmg1yJ0jzwBs0034WbzsgQrcfw,22
+nonebot_plugin_bottle-1.0.0.3.dist-info/RECORD,,
```

