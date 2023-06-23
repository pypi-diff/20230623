# Comparing `tmp/aiogram3_form-0.4.1.tar.gz` & `tmp/aiogram3_form-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_form-0.4.1.tar", max compression
+gzip compressed data, was "aiogram3_form-0.5.1.tar", max compression
```

## Comparing `aiogram3_form-0.4.1.tar` & `aiogram3_form-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      294 2023-01-24 13:28:23.727234 aiogram3_form-0.4.1/aiogram3_form/__init__.py
--rw-r--r--   0        0        0     1383 2023-04-13 18:33:34.599104 aiogram3_form-0.4.1/aiogram3_form/field.py
--rw-r--r--   0        0        0      843 2023-01-24 00:46:35.276915 aiogram3_form-0.4.1/aiogram3_form/filters.py
--rw-r--r--   0        0        0     8589 2023-05-28 19:15:40.978378 aiogram3_form-0.4.1/aiogram3_form/form.py
--rw-r--r--   0        0        0      120 2023-01-24 00:23:37.244911 aiogram3_form-0.4.1/aiogram3_form/state.py
--rw-r--r--   0        0        0     1092 2023-01-24 00:20:12.265098 aiogram3_form-0.4.1/LICENSE
--rw-r--r--   0        0        0      520 2023-05-28 19:15:24.895556 aiogram3_form-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1479 2023-01-24 00:20:12.265098 aiogram3_form-0.4.1/README.md
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 aiogram3_form-0.4.1/setup.py
--rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 aiogram3_form-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      294 2023-05-28 20:07:11.098853 aiogram3_form-0.5.1/aiogram3_form/__init__.py
+-rw-r--r--   0        0        0     1383 2023-04-13 18:33:34.599104 aiogram3_form-0.5.1/aiogram3_form/field.py
+-rw-r--r--   0        0        0      843 2023-01-24 00:46:35.276915 aiogram3_form-0.5.1/aiogram3_form/filters.py
+-rw-r--r--   0        0        0     8500 2023-06-22 21:12:33.945649 aiogram3_form-0.5.1/aiogram3_form/form.py
+-rw-r--r--   0        0        0      120 2023-01-24 00:23:37.244911 aiogram3_form-0.5.1/aiogram3_form/state.py
+-rw-r--r--   0        0        0     1092 2023-01-24 00:20:12.265098 aiogram3_form-0.5.1/LICENSE
+-rw-r--r--   0        0        0      520 2023-06-23 00:19:42.272913 aiogram3_form-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1372 2023-06-22 20:59:34.559238 aiogram3_form-0.5.1/README.md
+-rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 aiogram3_form-0.5.1/setup.py
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 aiogram3_form-0.5.1/PKG-INFO
```

### Comparing `aiogram3_form-0.4.1/aiogram3_form/field.py` & `aiogram3_form-0.5.1/aiogram3_form/field.py`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.4.1/aiogram3_form/filters.py` & `aiogram3_form-0.5.1/aiogram3_form/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.4.1/aiogram3_form/form.py` & `aiogram3_form-0.5.1/aiogram3_form/form.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 from . import filters
 from .field import FormFieldData, FormFieldInfo
 from .state import FormState
 
 SubmitCallback = Callable[..., Any]
 Markup = Union[types.ReplyKeyboardMarkup, types.InlineKeyboardMarkup]
 
-REMOVE_MARKUP = types.ReplyKeyboardRemove(remove_keyboard=True)
-
 
 class FormMeta(ABCMeta):
     router: ClassVar[Router]
     clear_state_on_submit: ClassVar[bool] = True
 
     __form_cls_names: Set[str] = set()
 
@@ -41,26 +39,31 @@
         cls_dict["clear_state_on_submit"] = clear_state_on_submit
         cls_dict["router"] = router
 
         return super().__new__(cls, cls_name, parents, cls_dict)
 
 
 class Form(ABC, metaclass=FormMeta, router=None):  # type: ignore
-    __registered_forms: Set[str] = set()
     __submit_callback: Optional[SubmitCallback] = None
 
     def __init__(self, bot: Bot, chat_id: int):
         self.bot = bot
         self.chat_id = chat_id
 
     @classmethod
     def submit(cls):
         def decorator(submit_callback: SubmitCallback):
             cls.__submit_callback = submit_callback
 
+            cls.router.message.register(
+                cls.__resolve_callback,
+                FormState.waiting_field_value,
+                cls.__current_field_filter,
+            )
+
         return decorator
 
     @classmethod
     async def __create_object(
         cls, handler_data: dict[str, Any], state_data: Dict[str, Any]
     ):
         form_object = cls(handler_data["bot"], handler_data["event_chat"].id)
@@ -125,43 +128,31 @@
     async def start(cls, bot: Bot, state_ctx: FSMContext):
         first_field = cls.__get_next_field(None)
 
         if first_field is None:
             raise TypeError("First field couldn't be None")
 
         await state_ctx.set_state(FormState.waiting_field_value)
-
         await state_ctx.update_data(
-            __current_field_name=first_field.name,  # type: ignore
+            __current_field_name=first_field.name,
             __form_values={},
             __form_name=cls.__name__,
         )
 
         if first_field.info.enter_callback:
-            await first_field.info.enter_callback(
+            return await first_field.info.enter_callback(
                 state_ctx.key.chat_id, state_ctx.key.user_id, {}
             )
-        else:
-            await bot.send_message(
-                state_ctx.key.chat_id,
-                first_field.info.enter_message_text,  # type: ignore
-                reply_markup=first_field.info.reply_markup or REMOVE_MARKUP,  # type: ignore
-            )
 
-        if cls in Form.__registered_forms:
-            return
-
-        cls.router.message.register(
-            cls.__resolve_callback,
-            FormState.waiting_field_value,
-            cls.__current_field_filter,
+        return await bot.send_message(
+            state_ctx.key.chat_id,
+            first_field.info.enter_message_text,  # type: ignore
+            reply_markup=first_field.info.reply_markup,
         )
 
-        Form.__registered_forms.add(cls.__name__)
-
     @classmethod
     async def __resolve_callback(
         cls, message: types.Message, state: FSMContext, value: Any, **data
     ):
         state_data = await state.get_data()
         current_field_name: str = state_data["__current_field_name"]
         state_data["__form_values"][current_field_name] = value
@@ -176,15 +167,15 @@
             if next_field.info.enter_callback:
                 return await next_field.info.enter_callback(
                     state.key.chat_id, state.key.user_id, state_data
                 )
 
             return await message.answer(
                 next_field.info.enter_message_text,  # type: ignore
-                reply_markup=next_field.info.reply_markup or REMOVE_MARKUP,
+                reply_markup=next_field.info.reply_markup,
             )
 
         if not cls.__submit_callback:
             raise TypeError(
                 f"{cls.__name__} submit callback is {cls.__submit_callback}"
             )
 
@@ -211,42 +202,45 @@
         current_field_name: str = state_data["__current_field_name"]
         current_field = cls.__get_field_data_by_name(current_field_name)
 
         field_filter = current_field.info.filter or cls.__get_filter_from_type(
             current_field.type
         )
 
+        async def send_error_message():
+            if current_field.info.error_message_text:
+                return await message.answer(
+                    current_field.info.error_message_text,
+                    reply_markup=current_field.info.reply_markup,
+                )
+
         # TODO: allow using sync filters
         if inspect.iscoroutinefunction(field_filter):
             prepared_field_filter = cls.__prepare_function(
                 field_filter, message, **data
             )
 
             filter_result = await prepared_field_filter()
 
-            if filter_result is False:
-                return False
+            if filter_result is not False:
+                return dict(value=filter_result)
 
-            return dict(value=filter_result)
+            await send_error_message()
+            return False
 
         if isinstance(field_filter, MagicFilter):
             filter_result = field_filter.resolve(message)
 
-            if not filter_result:
-                return False
+            if filter_result is not None:
+                return dict(value=filter_result)
 
-            return dict(value=filter_result)
-
-        if current_field.info.error_message_text:
-            await message.answer(
-                current_field.info.error_message_text,
-                reply_markup=current_field.info.reply_markup or REMOVE_MARKUP,
-            )
+            await send_error_message()
+            return False
 
-        return False
+        raise TypeError(f"Invalid filter specified for field {current_field_name}")
 
     async def answer(
         self,
         text: str,
         reply_markup: Union[
             types.InlineKeyboardMarkup,
             types.ReplyKeyboardMarkup,
```

### Comparing `aiogram3_form-0.4.1/LICENSE` & `aiogram3_form-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.4.1/pyproject.toml` & `aiogram3_form-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiogram3-form"
-version = "0.4.1"
+version = "0.5.1"
 description = "A library to create forms in aiogram3"
 authors = ["TrixiS <oficialmorozov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aiogram3_form"}]
 
 [tool.poetry.dependencies]
```

### Comparing `aiogram3_form-0.4.1/README.md` & `aiogram3_form-0.5.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 # aiogram3-form
 A library to create forms in aiogram3
 
+```shell
+pip install aiogram3-form
+```
+
 # Example
 ```Python
-# suppose you import here your router and bot objects
-from aiogram import F, types
+import asyncio
 
+from aiogram import Bot, Dispatcher, F, Router, types
 from aiogram3_form import Form, FormField
+from aiogram.fsm.context import FSMContext
+
+bot = Bot(token=YOUR_TOKEN)
+dispatcher = Dispatcher()
+router = Router()
+dispatcher.include_router(router)
 
 
-class NameForm(Form, router=your_router):
+class NameForm(Form, router=router):
     first_name: str = FormField(enter_message_text="Enter your first name please")
-    second_name: str = FormField(enter_message_text="Enter your second name please", filter=F.text.len() > 10)
-    age: int = FormField(enter_message_text="Enter age as integer", error_message_text="Age should be numeric!")
+    second_name: str = FormField(
+        enter_message_text="Enter your second name please",
+        filter=F.text.len() > 10 & F.text,
+    )
+    age: int = FormField(
+        enter_message_text="Enter age as integer",
+        error_message_text="Age should be numeric!",
+    )
 
 
 @NameForm.submit()
 async def name_form_submit_handler(form: NameForm, event_chat: types.Chat):
     # handle form data
     # also supports aiogram standart DI (e. g. middlewares, filters, etc)
-    await bot.send_message(
-        event_chat.id, f"Your full name is {form.first_name} {form.second_name}!"
+    await form.answer(
+        f"{form.first_name} {form.second_name} of age {form.age} in chat {event_chat.title}"
     )
-    
-    
-@router.message(F.text == "/form")
-async def form_handler(message: types.Message, state: FSMContext):
-    await NameForm.start(state)  # start your form
-```
-
-After submit callback call the state would be automatically cleared.
 
-You can control this state using the following metaclass kwarg
 
-```Python
-...
+@router.message(F.text == "/form")
+async def form_handler(_, state: FSMContext):
+    await NameForm.start(bot, state)  # start your form
 
 
-class NameForm(Form, clear_state_on_submit=False):  # True by default
-    ...
+async def main():
+    await dispatcher.start_polling(bot)
 
 
-@NameForm.submit()
-async def name_form_submit_handler(form: NameForm, state: FSMContext):
-    # so you can set your exit state manually
-    await state.set_state(...)
+asyncio.run(main())
 ```
```

### Comparing `aiogram3_form-0.4.1/setup.py` & `aiogram3_form-0.5.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['aiogram3_form']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'aiogram3-form',
-    'version': '0.4.1',
+    'version': '0.5.1',
     'description': 'A library to create forms in aiogram3',
-    'long_description': '# aiogram3-form\nA library to create forms in aiogram3\n\n# Example\n```Python\n# suppose you import here your router and bot objects\nfrom aiogram import F, types\n\nfrom aiogram3_form import Form, FormField\n\n\nclass NameForm(Form, router=your_router):\n    first_name: str = FormField(enter_message_text="Enter your first name please")\n    second_name: str = FormField(enter_message_text="Enter your second name please", filter=F.text.len() > 10)\n    age: int = FormField(enter_message_text="Enter age as integer", error_message_text="Age should be numeric!")\n\n\n@NameForm.submit()\nasync def name_form_submit_handler(form: NameForm, event_chat: types.Chat):\n    # handle form data\n    # also supports aiogram standart DI (e. g. middlewares, filters, etc)\n    await bot.send_message(\n        event_chat.id, f"Your full name is {form.first_name} {form.second_name}!"\n    )\n    \n    \n@router.message(F.text == "/form")\nasync def form_handler(message: types.Message, state: FSMContext):\n    await NameForm.start(state)  # start your form\n```\n\nAfter submit callback call the state would be automatically cleared.\n\nYou can control this state using the following metaclass kwarg\n\n```Python\n...\n\n\nclass NameForm(Form, clear_state_on_submit=False):  # True by default\n    ...\n\n\n@NameForm.submit()\nasync def name_form_submit_handler(form: NameForm, state: FSMContext):\n    # so you can set your exit state manually\n    await state.set_state(...)\n```\n',
+    'long_description': '# aiogram3-form\nA library to create forms in aiogram3\n\n```shell\npip install aiogram3-form\n```\n\n# Example\n```Python\nimport asyncio\n\nfrom aiogram import Bot, Dispatcher, F, Router, types\nfrom aiogram3_form import Form, FormField\nfrom aiogram.fsm.context import FSMContext\n\nbot = Bot(token=YOUR_TOKEN)\ndispatcher = Dispatcher()\nrouter = Router()\ndispatcher.include_router(router)\n\n\nclass NameForm(Form, router=router):\n    first_name: str = FormField(enter_message_text="Enter your first name please")\n    second_name: str = FormField(\n        enter_message_text="Enter your second name please",\n        filter=F.text.len() > 10 & F.text,\n    )\n    age: int = FormField(\n        enter_message_text="Enter age as integer",\n        error_message_text="Age should be numeric!",\n    )\n\n\n@NameForm.submit()\nasync def name_form_submit_handler(form: NameForm, event_chat: types.Chat):\n    # handle form data\n    # also supports aiogram standart DI (e. g. middlewares, filters, etc)\n    await form.answer(\n        f"{form.first_name} {form.second_name} of age {form.age} in chat {event_chat.title}"\n    )\n\n\n@router.message(F.text == "/form")\nasync def form_handler(_, state: FSMContext):\n    await NameForm.start(bot, state)  # start your form\n\n\nasync def main():\n    await dispatcher.start_polling(bot)\n\n\nasyncio.run(main())\n```\n',
     'author': 'TrixiS',
     'author_email': 'oficialmorozov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `aiogram3_form-0.4.1/PKG-INFO` & `aiogram3_form-0.5.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-form
-Version: 0.4.1
+Version: 0.5.1
 Summary: A library to create forms in aiogram3
 License: MIT
 Author: TrixiS
 Author-email: oficialmorozov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,53 +13,58 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # aiogram3-form
 A library to create forms in aiogram3
 
+```shell
+pip install aiogram3-form
+```
+
 # Example
 ```Python
-# suppose you import here your router and bot objects
-from aiogram import F, types
+import asyncio
 
+from aiogram import Bot, Dispatcher, F, Router, types
 from aiogram3_form import Form, FormField
+from aiogram.fsm.context import FSMContext
+
+bot = Bot(token=YOUR_TOKEN)
+dispatcher = Dispatcher()
+router = Router()
+dispatcher.include_router(router)
 
 
-class NameForm(Form, router=your_router):
+class NameForm(Form, router=router):
     first_name: str = FormField(enter_message_text="Enter your first name please")
-    second_name: str = FormField(enter_message_text="Enter your second name please", filter=F.text.len() > 10)
-    age: int = FormField(enter_message_text="Enter age as integer", error_message_text="Age should be numeric!")
+    second_name: str = FormField(
+        enter_message_text="Enter your second name please",
+        filter=F.text.len() > 10 & F.text,
+    )
+    age: int = FormField(
+        enter_message_text="Enter age as integer",
+        error_message_text="Age should be numeric!",
+    )
 
 
 @NameForm.submit()
 async def name_form_submit_handler(form: NameForm, event_chat: types.Chat):
     # handle form data
     # also supports aiogram standart DI (e. g. middlewares, filters, etc)
-    await bot.send_message(
-        event_chat.id, f"Your full name is {form.first_name} {form.second_name}!"
+    await form.answer(
+        f"{form.first_name} {form.second_name} of age {form.age} in chat {event_chat.title}"
     )
-    
-    
-@router.message(F.text == "/form")
-async def form_handler(message: types.Message, state: FSMContext):
-    await NameForm.start(state)  # start your form
-```
-
-After submit callback call the state would be automatically cleared.
 
-You can control this state using the following metaclass kwarg
 
-```Python
-...
+@router.message(F.text == "/form")
+async def form_handler(_, state: FSMContext):
+    await NameForm.start(bot, state)  # start your form
 
 
-class NameForm(Form, clear_state_on_submit=False):  # True by default
-    ...
+async def main():
+    await dispatcher.start_polling(bot)
 
 
-@NameForm.submit()
-async def name_form_submit_handler(form: NameForm, state: FSMContext):
-    # so you can set your exit state manually
-    await state.set_state(...)
+asyncio.run(main())
 ```
```

