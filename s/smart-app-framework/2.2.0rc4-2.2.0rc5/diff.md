# Comparing `tmp/smart_app_framework-2.2.0rc4-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.2.0rc5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 305894 bytes, number of entries: 333
+Zip file size: 305932 bytes, number of entries: 333
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/actions/__init__.py
 -rw-r--r--  2.0 unx    10756 b- defN 80-Jan-01 00:00 core/basic_models/actions/basic_actions.py
 -rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
 -rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 core/basic_models/actions/command.py
 -rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 core/basic_models/actions/counter_actions.py
@@ -247,15 +247,15 @@
 -rw-r--r--  2.0 unx    24642 b- defN 80-Jan-01 00:00 smart_kit/resources/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/start_points/__init__.py
 -rw-r--r--  2.0 unx     1198 b- defN 80-Jan-01 00:00 smart_kit/start_points/app.py
 -rw-r--r--  2.0 unx     6735 b- defN 80-Jan-01 00:00 smart_kit/start_points/base_main_loop.py
 -rw-r--r--  2.0 unx       56 b- defN 80-Jan-01 00:00 smart_kit/start_points/constants.py
 -rw-r--r--  2.0 unx     7976 b- defN 80-Jan-01 00:00 smart_kit/start_points/main_loop_async_http.py
 -rw-r--r--  2.0 unx     7147 b- defN 80-Jan-01 00:00 smart_kit/start_points/main_loop_http.py
--rw-r--r--  2.0 unx    36715 b- defN 80-Jan-01 00:00 smart_kit/start_points/main_loop_kafka.py
+-rw-r--r--  2.0 unx    36783 b- defN 80-Jan-01 00:00 smart_kit/start_points/main_loop_kafka.py
 -rw-r--r--  2.0 unx      612 b- defN 80-Jan-01 00:00 smart_kit/start_points/postprocess.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/system_answers/__init__.py
 -rw-r--r--  2.0 unx     1005 b- defN 80-Jan-01 00:00 smart_kit/system_answers/nothing_found_action.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/template/app/__init__.py-tpl
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/template/app/adapters/__init__.py-tpl
 -rw-r--r--  2.0 unx      969 b- defN 80-Jan-01 00:00 smart_kit/template/app/adapters/db_adapters.py-tpl
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/template/app/basic_entities/__init__.py-tpl
@@ -325,11 +325,11 @@
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     3946 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
 -rw-r--r--  2.0 unx     3322 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 smart_kit/utils/object_location.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc4.dist-info/WHEEL
-?rw-r--r--  2.0 unx    32268 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc4.dist-info/RECORD
-333 files, 985048 bytes uncompressed, 253288 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc5.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32268 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc5.dist-info/RECORD
+333 files, 985116 bytes uncompressed, 253326 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -984,17 +984,17 @@
 
 Filename: smart_kit/utils/object_location.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc4.dist-info/METADATA
+Filename: smart_app_framework-2.2.0rc5.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc4.dist-info/WHEEL
+Filename: smart_app_framework-2.2.0rc5.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.2.0rc4.dist-info/RECORD
+Filename: smart_app_framework-2.2.0rc5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smart_kit/start_points/main_loop_kafka.py

```diff
@@ -636,41 +636,44 @@
     async def do_behavior_timeout(self, kwargs, worker_kwargs):
         self.concurrent_messages += 1
         mq_message, kafka_key = kwargs.get("mq_message"), kwargs.get("kafka_key")
         callback_id, db_uid = kwargs.get("callback_id"), kwargs.get("db_uid")
 
         try:
             save_tries = 0
-            user_save_no_collisions = False
+            user_save_ok = False
             answers = []
             user = None
             timeout_from_message = None
-            while save_tries < self.user_save_collisions_tries and not user_save_no_collisions:
+            callback_found = True
+            while save_tries < self.user_save_collisions_tries and not user_save_ok:
+                callback_found = False
                 save_tries += 1
                 orig_message_raw = json.loads(mq_message.value())
                 orig_message_raw[SmartAppFromMessage.MESSAGE_NAME] = message_names.LOCAL_TIMEOUT
                 timeout_from_message = self._get_timeout_from_message(orig_message_raw, callback_id,
                                                                       headers=mq_message.headers())
 
                 log(f"MainLoop.do_behavior_timeout: handling callback {callback_id}. "
                     f"for db_uid {db_uid}. try {save_tries}.",
                     params={log_const.KEY_NAME: "MainLoop",
                             MESSAGE_ID_STR: timeout_from_message.incremental_id})
                 user = await self.load_user(db_uid, timeout_from_message)
 
                 if user.behaviors.has_callback(callback_id):
+                    callback_found = True
                     commands = await self.model.answer(timeout_from_message, user)
                     topic_key = self._get_topic_key(mq_message, kafka_key)
                     answers = self._generate_answers(user=user, commands=commands, message=timeout_from_message,
                                                      topic_key=topic_key,
                                                      kafka_key=kafka_key)
 
-                    user_save_no_collisions = await self.save_user(db_uid, user, mq_message)
+                    user_save_ok = await self.save_user(db_uid, user, mq_message)
 
-                    if not user_save_no_collisions:
+                    if not user_save_ok:
                         log("MainLoop.do_behavior_timeout: save user got collision on uid %(uid)s db_version "
                             "%(db_version)s.",
                             user=user,
                             params={log_const.KEY_NAME: "ignite_collision",
                                     "db_uid": db_uid,
                                     "message_key": (mq_message.key() or b"").decode('utf-8', 'backslashreplace'),
                                     "kafka_key": kafka_key,
@@ -678,29 +681,29 @@
                                     "db_version": str(user.private_vars.get(user.USER_DB_VERSION))},
                             level="WARNING")
                 else:
                     break
 
             self.remove_timer(timeout_from_message)
 
-            if not user_save_no_collisions:
+            if not user_save_ok and callback_found:
                 log("MainLoop.do_behavior_timeout: db_save collision all tries left on uid %(uid)s db_version "
                     "%(db_version)s.",
                     user=user,
                     params={log_const.KEY_NAME: "ignite_collision",
                             "db_uid": db_uid,
                             "message_key": (mq_message.key() or b"").decode('utf-8', 'backslashreplace'),
                             "message_partition": mq_message.partition(),
                             "kafka_key": kafka_key,
                             "uid": user.id,
                             "db_version": str(user.private_vars.get(user.USER_DB_VERSION))},
                     level="WARNING")
                 monitoring.counter_save_collision_tries_left(self.app_name)
 
-            if user_save_no_collisions:
+            if user_save_ok:
                 self.save_behavior_timeouts(user, mq_message, kafka_key)
                 for answer in answers:
                     self._send_request(user, answer, mq_message)
         except Exception:
             log("%(class_name)s error.", params={log_const.KEY_NAME: "error_handling_timeout",
                                                  "class_name": self.__class__.__name__,
                                                  log_const.REQUEST_VALUE: str(mq_message.value())},
```

## Comparing `smart_app_framework-2.2.0rc4.dist-info/METADATA` & `smart_app_framework-2.2.0rc5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.2.0rc4
+Version: 2.2.0rc5
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
 Requires-Python: >=3.8.1,<3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

## Comparing `smart_app_framework-2.2.0rc4.dist-info/RECORD` & `smart_app_framework-2.2.0rc5.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -246,15 +246,15 @@
 smart_kit/resources/__init__.py,sha256=wn2ybqp9FpcZB__W4XTDdbyuRoYRFihO_Lp-WQEPhJc,24642
 smart_kit/start_points/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/start_points/app.py,sha256=8lcZV7SiEBzFdcF7oe-54w7hmyHfK9PQ_IDa64_kVjM,1198
 smart_kit/start_points/base_main_loop.py,sha256=Kcedoy-rAhjk2HChcxb-sWY-XlE3ptMcB4VZT6HO6WY,6735
 smart_kit/start_points/constants.py,sha256=d_XQfL3YxYswZd5AFIwugqv8EimD18ZFfPRcPJpAgK0,56
 smart_kit/start_points/main_loop_async_http.py,sha256=o2tOOpkt-J0T3fJzS-cKVBqAEwEsmshWeACbudzzBfg,7976
 smart_kit/start_points/main_loop_http.py,sha256=TNNHuwrqbrg7fpLY1pY_J43dA2hbsNs-_MePOyqo_s8,7147
-smart_kit/start_points/main_loop_kafka.py,sha256=KNVMRXimJ4FY2cDMA06Y0Q6Prlba096S-Op9gU9dN4c,36715
+smart_kit/start_points/main_loop_kafka.py,sha256=kUn-UYM0Nr-4DvNCshbTODK1UhNSBSZLjG3VO8CUZWE,36783
 smart_kit/start_points/postprocess.py,sha256=rUfh8Wl3rJ0Tbaoce5EtckG87_nCg5KYo8y_O2UpclQ,612
 smart_kit/system_answers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/system_answers/nothing_found_action.py,sha256=yW0_X34v4UEuPFlR2jTdBk7wJ9elSu-MezLVcNS-jJY,1005
 smart_kit/template/app/__init__.py-tpl,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/template/app/adapters/__init__.py-tpl,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/template/app/adapters/db_adapters.py-tpl,sha256=yocQSahj8Kgw2Odi9XUlO7E7Y2DXCxe1Tq6bgP2tJnQ,969
 smart_kit/template/app/basic_entities/__init__.py-tpl,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -324,10 +324,10 @@
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=UP2Zmp0VW4YZpDPe_lGQ-5L_wF5wd7J4B33kXyUINmQ,3946
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/logger_writer/logger_formatter.py,sha256=n5N4FHjXyeZAASjVB2zhoOMsbnWiixI0OQsk4KkcDFg,3322
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/object_location.py,sha256=uJmTxBBeeyvwahiA1TMKr2rzDW9R1bh-FwK663zoBe4,332
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.2.0rc4.dist-info/METADATA,sha256=SS1JEdW8cryo47JC1VmRYDc9J10OASyIstICHX-wXdg,10823
-smart_app_framework-2.2.0rc4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-smart_app_framework-2.2.0rc4.dist-info/RECORD,,
+smart_app_framework-2.2.0rc5.dist-info/METADATA,sha256=chmnKcJzs9OXmUM3oV3_SsRfu_IB2Fh5tdKYKBrEid0,10823
+smart_app_framework-2.2.0rc5.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+smart_app_framework-2.2.0rc5.dist-info/RECORD,,
```

