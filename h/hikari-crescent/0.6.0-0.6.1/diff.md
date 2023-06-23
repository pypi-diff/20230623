# Comparing `tmp/hikari_crescent-0.6.0.tar.gz` & `tmp/hikari_crescent-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_crescent-0.6.0.tar", max compression
+gzip compressed data, was "hikari_crescent-0.6.1.tar", max compression
```

## Comparing `hikari_crescent-0.6.0.tar` & `hikari_crescent-0.6.1.tar`

### file list

```diff
@@ -1,47 +1,46 @@
--rw-r--r--   0        0        0    16725 2023-02-19 08:03:34.318421 hikari_crescent-0.6.0/LICENSE
--rw-r--r--   0        0        0     5949 2023-02-19 08:03:34.318421 hikari_crescent-0.6.0/README.md
--rw-r--r--   0        0        0     1235 2023-02-19 08:03:34.318421 hikari_crescent-0.6.0/crescent/__init__.py
--rw-r--r--   0        0        0      207 2023-02-19 08:03:34.318421 hikari_crescent-0.6.0/crescent/_about.py
--rw-r--r--   0        0        0     1645 2023-02-19 08:03:34.318421 hikari_crescent-0.6.0/crescent/banner.txt
--rw-r--r--   0        0        0     8056 2023-02-19 08:03:34.318421 hikari_crescent-0.6.0/crescent/client.py
--rw-r--r--   0        0        0      531 2023-02-19 08:03:34.318421 hikari_crescent-0.6.0/crescent/commands/__init__.py
--rw-r--r--   0        0        0     2201 2023-02-19 08:03:34.318421 hikari_crescent-0.6.0/crescent/commands/args.py
--rw-r--r--   0        0        0     7627 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/commands/decorators.py
--rw-r--r--   0        0        0     2560 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/commands/groups.py
--rw-r--r--   0        0        0     1775 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/commands/hooks.py
--rw-r--r--   0        0        0    10666 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/commands/options.py
--rw-r--r--   0        0        0     3809 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/commands/signature.py
--rw-r--r--   0        0        0      374 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/context/__init__.py
--rw-r--r--   0        0        0     3229 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/context/autocomplete_context.py
--rw-r--r--   0        0        0     4242 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/context/base_context.py
--rw-r--r--   0        0        0     9782 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/context/context.py
--rw-r--r--   0        0        0     2109 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/context/utils.py
--rw-r--r--   0        0        0     3122 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/errors.py
--rw-r--r--   0        0        0     2654 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/event.py
--rw-r--r--   0        0        0      642 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/exceptions.py
--rw-r--r--   0        0        0     1964 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/ext/cooldowns/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/ext/cooldowns/py.typed
--rw-r--r--   0        0        0     2823 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/ext/locales/__init__.py
--rw-r--r--   0        0        0      277 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/ext/tasks/__init__.py
--rw-r--r--   0        0        0     1697 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/ext/tasks/cron.py
--rw-r--r--   0        0        0     1614 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/ext/tasks/loop.py
--rw-r--r--   0        0        0        0 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/ext/tasks/py.typed
--rw-r--r--   0        0        0     2402 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/ext/tasks/task.py
--rw-r--r--   0        0        0      281 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/internal/__init__.py
--rw-r--r--   0        0        0     6058 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/internal/app_command.py
--rw-r--r--   0        0        0     9298 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/internal/handle_resp.py
--rw-r--r--   0        0        0      980 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/internal/includable.py
--rw-r--r--   0        0        0    16830 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/internal/registry.py
--rw-r--r--   0        0        0      945 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/locale.py
--rw-r--r--   0        0        0     1315 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/mentionable.py
--rw-r--r--   0        0        0     8975 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/plugin.py
--rw-r--r--   0        0        0        0 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/py.typed
--rw-r--r--   0        0        0     2156 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/typedefs.py
--rw-r--r--   0        0        0      317 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/utils/__init__.py
--rw-r--r--   0        0        0      236 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/utils/any_issubclass.py
--rw-r--r--   0        0        0      256 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/utils/gather_iter.py
--rw-r--r--   0        0        0      629 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/utils/options.py
--rw-r--r--   0        0        0      513 2023-02-19 08:03:34.322422 hikari_crescent-0.6.0/crescent/utils/tasks.py
--rw-r--r--   0        0        0     2558 2023-02-19 08:03:45.650501 hikari_crescent-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7244 1970-01-01 00:00:00.000000 hikari_crescent-0.6.0/setup.py
--rw-r--r--   0        0        0     7334 1970-01-01 00:00:00.000000 hikari_crescent-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/LICENSE
+-rw-r--r--   0        0        0     6951 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/README.md
+-rw-r--r--   0        0        0     1235 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/_about.py
+-rw-r--r--   0        0        0     1645 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/banner.txt
+-rw-r--r--   0        0        0     8056 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/client.py
+-rw-r--r--   0        0        0      531 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/__init__.py
+-rw-r--r--   0        0        0     2328 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/args.py
+-rw-r--r--   0        0        0     7689 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/decorators.py
+-rw-r--r--   0        0        0     2560 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/groups.py
+-rw-r--r--   0        0        0     1775 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/hooks.py
+-rw-r--r--   0        0        0    11553 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/options.py
+-rw-r--r--   0        0        0     3814 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/commands/signature.py
+-rw-r--r--   0        0        0      374 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/context/__init__.py
+-rw-r--r--   0        0        0     3229 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/context/autocomplete_context.py
+-rw-r--r--   0        0        0     4242 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/context/base_context.py
+-rw-r--r--   0        0        0    10056 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/context/context.py
+-rw-r--r--   0        0        0     2109 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/context/utils.py
+-rw-r--r--   0        0        0     3122 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/errors.py
+-rw-r--r--   0        0        0     2673 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/event.py
+-rw-r--r--   0        0        0      642 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/exceptions.py
+-rw-r--r--   0        0        0     1964 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/cooldowns/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/cooldowns/py.typed
+-rw-r--r--   0        0        0     2823 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/locales/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/tasks/__init__.py
+-rw-r--r--   0        0        0     1697 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/tasks/cron.py
+-rw-r--r--   0        0        0     1614 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/tasks/loop.py
+-rw-r--r--   0        0        0        0 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/tasks/py.typed
+-rw-r--r--   0        0        0     2402 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/ext/tasks/task.py
+-rw-r--r--   0        0        0      281 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/internal/__init__.py
+-rw-r--r--   0        0        0     6063 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/internal/app_command.py
+-rw-r--r--   0        0        0     9438 2023-06-23 06:29:14.507058 hikari_crescent-0.6.1/crescent/internal/handle_resp.py
+-rw-r--r--   0        0        0      980 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/internal/includable.py
+-rw-r--r--   0        0        0    16835 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/internal/registry.py
+-rw-r--r--   0        0        0      945 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/locale.py
+-rw-r--r--   0        0        0     1315 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/mentionable.py
+-rw-r--r--   0        0        0     8975 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/py.typed
+-rw-r--r--   0        0        0     2270 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/typedefs.py
+-rw-r--r--   0        0        0      317 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/utils/__init__.py
+-rw-r--r--   0        0        0      236 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/utils/any_issubclass.py
+-rw-r--r--   0        0        0      256 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/utils/gather_iter.py
+-rw-r--r--   0        0        0      629 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/utils/options.py
+-rw-r--r--   0        0        0      513 2023-06-23 06:29:14.511058 hikari_crescent-0.6.1/crescent/utils/tasks.py
+-rw-r--r--   0        0        0     2570 2023-06-23 06:29:28.763278 hikari_crescent-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     8336 1970-01-01 00:00:00.000000 hikari_crescent-0.6.1/PKG-INFO
```

### Comparing `hikari_crescent-0.6.0/LICENSE` & `hikari_crescent-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/README.md` & `hikari_crescent-0.6.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -112,14 +112,42 @@
 | `crescent.Mentionable` | Role or User |
 | Any Hikari channel type. | Channel. The options will be the channel type and its subclasses. |
 | `List[Channel Types]` (classes only) | Channel. ^ |
 | `Union[Channel Types]` (functions only) | Channel. ^ |
 | `hikari.Attachment` | Attachment |
 
 
+### Autocomplete
+Autocomplete is supported by using a callback function. This function returns a list of tuples where the first
+value is the option name and the second value is the option value. `str`, `int`, and `float` value types
+can be used.
+
+```python
+async def autocomplete(
+    ctx: crescent.AutocompleteContext, option: hikari.AutocompleteInteractionOption
+) -> list[tuple[str, str]]:
+    return [("Option 1", "Option value 1"), ("Option 2", "Option value 2")]
+
+@client.include
+@crescent.command(name="class-command")
+class ClassCommand:
+    option = crescent.option(str, autocomplete=autocomplete)
+
+    async def callback(self) -> None:
+        await ctx.respond(self.option)
+
+@client.include
+@crescent.command
+async def function_command(
+    ctx: crescent.Context,
+    option: Annotated[str, crescent.Autocomplete(autocomplete)]
+) -> None:
+    await ctx.respond(option)
+```
+
 ### Error Handling
 Errors that are raised by a command can be handled by `crescent.catch_command`.
 
 ```python
 class MyError(Exception):
     ...
 
@@ -130,14 +158,17 @@
 
 @client.include
 @crescent.command
 async def my_command(ctx: crescent.Context):
     raise MyError()
 ```
 
+There is also a `crescent.catch_event` and `crescent.catch_autocomplete` function for
+events and autocomplete respectively.
+
 ### Events
 ```python
 import hikari
 
 @client.include
 @crescent.event
 async def on_message_create(event: hikari.MessageCreateEvent):
@@ -157,11 +188,11 @@
 
 These extensions can be installed with pip.
 
 - [crescent-ext-docstrings](https://github.com/hikari-crescent/crescent-ext-docstrings) - Lets you use docstrings to write descriptions for commands and options.
 - [crescent-ext-kebabify](https://github.com/hikari-crescent/crescent-ext-kebabify) - Turns your command names into kebabs!
 
 # Support
-You can ask questions in the `#crescent` channel in the [Hikari Discord server](https://discord.gg/Jx4cNGG). My Discord username is `Lunarmagpie❤#0001`.
+You can ask questions in the `#crescent` channel in the [Hikari Discord server](https://discord.gg/Jx4cNGG). My Discord username is `lunarmagpie`.
 
 # Contributing
 Create an issue for your feature. There aren't any guidelines right now so just don't be rude.
```

### Comparing `hikari_crescent-0.6.0/crescent/__init__.py` & `hikari_crescent-0.6.1/crescent/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/banner.txt` & `hikari_crescent-0.6.1/crescent/banner.txt`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/client.py` & `hikari_crescent-0.6.1/crescent/client.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/commands/__init__.py` & `hikari_crescent-0.6.1/crescent/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/commands/args.py` & `hikari_crescent-0.6.1/crescent/commands/args.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 from abc import ABC
 from dataclasses import dataclass
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Generic
 
 from hikari import ChannelType, CommandChoice
 
 from crescent.locale import LocaleBuilder
+from crescent.typedefs import AutocompleteValueT
 
 if TYPE_CHECKING:
     from typing import Any, Sequence
 
     from crescent.typedefs import AutocompleteCallbackT
 
 __all__: Sequence[str] = (
@@ -103,13 +104,13 @@
 
     @property
     def payload(self) -> int:
         return self.max_length
 
 
 @dataclass(frozen=True)
-class Autocomplete(Arg):
-    callback: AutocompleteCallbackT
+class Autocomplete(Arg, Generic[AutocompleteValueT]):
+    callback: AutocompleteCallbackT[AutocompleteValueT]
 
     @property
-    def payload(self) -> AutocompleteCallbackT:
+    def payload(self) -> AutocompleteCallbackT[AutocompleteValueT]:
         return self.callback
```

### Comparing `hikari_crescent-0.6.0/crescent/commands/decorators.py` & `hikari_crescent-0.6.1/crescent/commands/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,17 +85,17 @@
             command,
             guild=guild,
             name=name,
             description=description,
             default_member_permissions=default_member_permissions,
             dm_enabled=dm_enabled,
             nsfw=nsfw,
-        )
+        )  # pyright: ignore
 
-    autocomplete: dict[str, AutocompleteCallbackT] = {}
+    autocomplete: dict[str, AutocompleteCallbackT[Any]] = {}
     options: list[CommandOption] = []
 
     if isclass(callback):
         # If callback is a class it must be `type[ClassCommandProto]` because of the function
         # signature.
         callback = cast("type[ClassCommandProto]", callback)
 
@@ -191,15 +191,15 @@
         return partial(
             user_command,
             guild=guild,
             name=name,
             default_member_permissions=default_member_permissions,
             dm_enabled=dm_enabled,
             nsfw=nsfw,
-        )
+        )  # pyright: ignore
 
     return register_command(
         callback=_kwargs_to_args_callback(callback),
         owner=callback,
         command_type=CommandType.USER,
         name=name or callback.__name__,
         guild=guild,
@@ -240,15 +240,15 @@
         return partial(
             message_command,
             guild=guild,
             name=name,
             default_member_permissions=default_member_permissions,
             dm_enabled=dm_enabled,
             nsfw=nsfw,
-        )
+        )  # pyright: ignore
 
     return register_command(
         callback=_kwargs_to_args_callback(callback),
         owner=callback,
         command_type=CommandType.MESSAGE,
         name=name or callback.__name__,
         guild=guild,
```

### Comparing `hikari_crescent-0.6.0/crescent/commands/groups.py` & `hikari_crescent-0.6.1/crescent/commands/groups.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/commands/hooks.py` & `hikari_crescent-0.6.1/crescent/commands/hooks.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/commands/options.py` & `hikari_crescent-0.6.1/crescent/commands/options.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,19 @@
     Attachment,
     ChannelType,
     CommandChoice,
     CommandOption,
     DMChannel,
     GroupDMChannel,
     GuildCategory,
+    GuildForumChannel,
     GuildNewsChannel,
+    GuildNewsThread,
+    GuildPrivateThread,
+    GuildPublicThread,
     GuildStageChannel,
     GuildTextChannel,
     GuildVoiceChannel,
     InteractionChannel,
     OptionType,
     PartialChannel,
     Role,
@@ -55,27 +59,46 @@
 VALID_CHANNEL_TYPES = Union[
     GuildTextChannel,
     DMChannel,
     GroupDMChannel,
     GuildVoiceChannel,
     GuildCategory,
     GuildNewsChannel,
+    GuildNewsThread,
+    GuildPublicThread,
+    GuildPrivateThread,
     GuildStageChannel,
+    GuildForumChannel,
 ]
 CHANNEL_TYPE_MAP: dict[type[VALID_CHANNEL_TYPES], ChannelType] = {
     GuildTextChannel: ChannelType.GUILD_TEXT,
     DMChannel: ChannelType.DM,
     GuildVoiceChannel: ChannelType.GUILD_VOICE,
     GroupDMChannel: ChannelType.GROUP_DM,
     GuildCategory: ChannelType.GUILD_CATEGORY,
     GuildNewsChannel: ChannelType.GUILD_NEWS,
+    GuildNewsThread: ChannelType.GUILD_NEWS_THREAD,
+    GuildPublicThread: ChannelType.GUILD_PUBLIC_THREAD,
+    GuildPrivateThread: ChannelType.GUILD_PRIVATE_THREAD,
     GuildStageChannel: ChannelType.GUILD_STAGE,
+    GuildForumChannel: ChannelType.GUILD_FORUM,
 }
 
 
+def build_choices(
+    choices: Sequence[tuple[str | LocaleBuilder, str | int | float]]
+) -> list[CommandChoice]:
+    result: list[CommandChoice] = []
+    for name, value in choices:
+        name, name_localizations = str_or_build_locale(name)
+        result.append(CommandChoice(name=name, name_localizations=name_localizations, value=value))
+
+    return result
+
+
 def get_channel_types(*channels: type[PartialChannel]) -> set[ChannelType]:
     if len(channels) == 1 and channels[0] is PartialChannel:
         return set()
 
     types: set[ChannelType] = set()
     for k, v in CHANNEL_TYPE_MAP.items():
         if issubclass(k, channels):
@@ -96,15 +119,15 @@
     default: UndefinedNoneOr[Any]
     choices: Sequence[CommandChoice] | None
     channel_types: Sequence[ChannelType] | None
     min_value: int | float | None
     max_value: int | float | None
     min_length: int | None
     max_length: int | None
-    autocomplete: AutocompleteCallbackT | None
+    autocomplete: AutocompleteCallbackT[Any] | None
 
     def _gen_option(self, name: str) -> CommandOption:
         name, name_localizations = str_or_build_locale(self.name or name)
         description, description_localizations = str_or_build_locale(self.description)
 
         return CommandOption(
             type=self.type,
@@ -280,108 +303,108 @@
 
 
 @overload
 def option(
     option_type: type[int],
     description: str | LocaleBuilder = ...,
     *,
-    choices: Sequence[tuple[str, int]] | None = ...,
-    autocomplete: AutocompleteCallbackT | None = ...,
+    choices: Sequence[tuple[str | LocaleBuilder, int]] | None = ...,
+    autocomplete: AutocompleteCallbackT[int] | None = ...,
     min_value: int | None = ...,
     max_value: int | None = ...,
     name: str | LocaleBuilder | None = ...,
 ) -> ClassCommandOption[int]:
     ...
 
 
 @overload
 def option(
     option_type: type[int],
     description: str | LocaleBuilder = ...,
     *,
     default: DEFAULT,
-    choices: Sequence[tuple[str, int]] | None = ...,
-    autocomplete: AutocompleteCallbackT | None = ...,
+    choices: Sequence[tuple[str | LocaleBuilder, int]] | None = ...,
+    autocomplete: AutocompleteCallbackT[int] | None = ...,
     min_value: int | None = ...,
     max_value: int | None = ...,
     name: str | LocaleBuilder | None = ...,
 ) -> ClassCommandOption[int | DEFAULT]:
     ...
 
 
 @overload
 def option(
     option_type: type[float],
     description: str | LocaleBuilder = ...,
     *,
-    choices: Sequence[tuple[str, float]] | None = ...,
-    autocomplete: AutocompleteCallbackT | None = ...,
+    choices: Sequence[tuple[str | LocaleBuilder, float]] | None = ...,
+    autocomplete: AutocompleteCallbackT[float] | None = ...,
     min_value: float | None = ...,
     max_value: float | None = ...,
     name: str | LocaleBuilder | None = ...,
 ) -> ClassCommandOption[float]:
     ...
 
 
 @overload
 def option(
     option_type: type[float],
     description: str | LocaleBuilder = ...,
     *,
     default: DEFAULT,
-    choices: Sequence[tuple[str, float]] | None = ...,
-    autocomplete: AutocompleteCallbackT | None = ...,
+    choices: Sequence[tuple[str | LocaleBuilder, float]] | None = ...,
+    autocomplete: AutocompleteCallbackT[float] | None = ...,
     min_value: float | None = ...,
     max_value: float | None = ...,
     name: str | LocaleBuilder | None = ...,
 ) -> ClassCommandOption[float | DEFAULT]:
     ...
 
 
 @overload
 def option(
     option_type: type[str],
     description: str | LocaleBuilder = ...,
     *,
     min_length: int | None = ...,
     max_length: int | None = ...,
-    choices: Sequence[tuple[str, str]] | None = ...,
-    autocomplete: AutocompleteCallbackT | None = ...,
+    choices: Sequence[tuple[str | LocaleBuilder, str]] | None = ...,
+    autocomplete: AutocompleteCallbackT[str] | None = ...,
     name: str | LocaleBuilder | None = ...,
 ) -> ClassCommandOption[str]:
     ...
 
 
 @overload
 def option(
     option_type: type[str],
     description: str | LocaleBuilder = ...,
     *,
     default: DEFAULT,
     min_length: int | None = ...,
     max_length: int | None = ...,
-    choices: Sequence[tuple[str, str]] | None = ...,
-    autocomplete: AutocompleteCallbackT | None = ...,
+    choices: Sequence[tuple[str | LocaleBuilder, str]] | None = ...,
+    autocomplete: AutocompleteCallbackT[str] | None = ...,
     name: str | LocaleBuilder | None = ...,
 ) -> ClassCommandOption[str | DEFAULT]:
     ...
 
 
 def option(
     option_type: type[OptionTypesT] | Sequence[type[PartialChannel]],
     description: str | LocaleBuilder = "No Description",
     *,
     default: UndefinedOr[Any] = UNDEFINED,
-    choices: Sequence[tuple[str, str | int | float]] | None = None,
+    choices: Sequence[tuple[str | LocaleBuilder, str | int | float]] | None = None,
     min_value: int | float | None = None,
     max_value: int | float | None = None,
     min_length: int | None = None,
     max_length: int | None = None,
     name: str | LocaleBuilder | None = None,
-    autocomplete: AutocompleteCallbackT | None = None,
+    autocomplete: AutocompleteCallbackT[Any] | None = None,
 ) -> ClassCommandOption[Any]:
     _option_type: type[OptionTypesT]
     if (
         isinstance(option_type, type)
         and issubclass(option_type, PartialChannel)
         and option_type is not PartialChannel
     ):
@@ -395,15 +418,15 @@
         _option_type = option_type
         channel_types = None
 
     return ClassCommandOption(
         type=OPTIONS_TYPE_MAP[_option_type],
         description=description,
         default=default,
-        choices=[CommandChoice(name=n, value=v) for n, v in choices] if choices else None,
+        choices=build_choices(choices) if choices else None,
         channel_types=list(channel_types) if channel_types else None,
         min_value=min_value,
         max_value=max_value,
         min_length=min_length,
         max_length=max_length,
         name=name,
         autocomplete=autocomplete,
```

### Comparing `hikari_crescent-0.6.0/crescent/commands/signature.py` & `hikari_crescent-0.6.1/crescent/commands/signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,10 +126,10 @@
         max_value=max_value,
         min_length=min_length,
         max_length=max_length,
         is_required=required,
     )
 
 
-def get_autocomplete_func(param: Parameter) -> AutocompleteCallbackT | None:
+def get_autocomplete_func(param: Parameter) -> AutocompleteCallbackT[Any] | None:
     _, metadata = _get_origin_and_metadata(param)
     return _get_arg(Autocomplete, metadata)
```

### Comparing `hikari_crescent-0.6.0/crescent/context/autocomplete_context.py` & `hikari_crescent-0.6.1/crescent/context/autocomplete_context.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/context/base_context.py` & `hikari_crescent-0.6.1/crescent/context/base_context.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/context/context.py` & `hikari_crescent-0.6.1/crescent/context/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, overload
 
-from hikari import UNDEFINED, Guild, GuildChannel, MessageFlag, ResponseType
+from hikari import (
+    UNDEFINED,
+    GatewayGuild,
+    GuildThreadChannel,
+    MessageFlag,
+    PermissibleGuildChannel,
+    ResponseType,
+)
 from hikari.traits import CacheAware
 
 from crescent.context.base_context import BaseContext
-from crescent.utils import map_or
 
 if TYPE_CHECKING:
     from typing import Any, Literal, Sequence
 
     from hikari import (
         Attachment,
         CommandInteraction,
@@ -32,24 +38,29 @@
 
 class Context(BaseContext):
     """Represents the context for command interactions"""
 
     interaction: CommandInteraction
 
     @property
-    def channel(self) -> GuildChannel | None:
+    def channel(self) -> PermissibleGuildChannel | GuildThreadChannel | None:
+        """Get this context's guild channel or thread from the cache.
+
+        > 📝 This will always be `None` for interactions triggered in a DM channel.
+        """
         if isinstance(self.app, CacheAware):
-            return self.app.cache.get_guild_channel(self.channel_id)
+            return self.app.cache.get_guild_channel(self.channel_id) or self.app.cache.get_thread(
+                self.channel_id
+            )
         return None
 
     @property
-    def guild(self) -> Guild | None:
-        if isinstance(self.app, CacheAware):
-            return map_or(self.guild_id, self.app.cache.get_available_guild)
-        return None
+    def guild(self) -> GatewayGuild | None:
+        """Get this context's guild from the cache."""
+        return self.interaction.get_guild()
 
     async def defer(self, ephemeral: bool = False) -> None:
         """
         Defer this interaction response, allowing you to respond within the next 15
         minutes.
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hikari_crescent-0.6.0/crescent/context/utils.py` & `hikari_crescent-0.6.1/crescent/context/utils.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/errors.py` & `hikari_crescent-0.6.1/crescent/errors.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/event.py` & `hikari_crescent-0.6.1/crescent/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ...
 
 
 def event(
     callback: CallbackT[Any] | None = None, /, *, event_type: type[Any] | None = None
 ) -> Callable[[CallbackT[Any]], Includable[CallbackT[Any]]] | Includable[CallbackT[Any]]:
     if callback is None:
-        return partial(event, event_type=event_type)
+        return partial(event, event_type=event_type)  # pyright: ignore
 
     if not event_type:
         event_type = next(iter(get_type_hints(callback).values()))
 
     if not event_type:
         raise ValueError("`event_type` must be provided in the decorator or as a typehint")
```

### Comparing `hikari_crescent-0.6.0/crescent/exceptions.py` & `hikari_crescent-0.6.1/crescent/exceptions.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/ext/cooldowns/__init__.py` & `hikari_crescent-0.6.1/crescent/ext/cooldowns/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/ext/locales/__init__.py` & `hikari_crescent-0.6.1/crescent/ext/locales/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/ext/tasks/cron.py` & `hikari_crescent-0.6.1/crescent/ext/tasks/cron.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/ext/tasks/loop.py` & `hikari_crescent-0.6.1/crescent/ext/tasks/loop.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/ext/tasks/task.py` & `hikari_crescent-0.6.1/crescent/ext/tasks/task.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/internal/app_command.py` & `hikari_crescent-0.6.1/crescent/internal/app_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 @dataclass
 class AppCommandMeta:
     app_command: AppCommand
     owner: Any
     """The function or class that was used to create the command"""
     callback: CommandCallbackT
-    autocomplete: dict[str, TransformedAutocompleteCallbackT] = field(default_factory=dict)
+    autocomplete: dict[str, TransformedAutocompleteCallbackT[Any]] = field(default_factory=dict)
     group: Group | None = None
     sub_group: SubGroup | None = None
     hooks: list[TransformedHookCallbackT] = field(default_factory=list)
     after_hooks: list[TransformedHookCallbackT] = field(default_factory=list)
 
     def add_hooks(
         self, hooks: Sequence[HookCallbackT], prepend: bool = False, *, after: bool
```

### Comparing `hikari_crescent-0.6.0/crescent/internal/handle_resp.py` & `hikari_crescent-0.6.1/crescent/internal/handle_resp.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     CommandType,
     InteractionType,
     Locale,
     OptionType,
     Snowflake,
 )
 from hikari.api import InteractionResponseBuilder
+from hikari.impl import AutocompleteChoiceBuilder
 
 from crescent.context import AutocompleteContext, BaseContext, Context
 from crescent.internal.app_command import Unique
 from crescent.mentionable import Mentionable
 from crescent.utils import unwrap
 
 if TYPE_CHECKING:
@@ -103,18 +104,19 @@
     option = _get_option_recursive(interaction.options)
     if not option:
         return
     autocomplete = command.metadata.autocomplete[option.name]
 
     try:
         res, ctx = await autocomplete(ctx, option)
+        choices = [AutocompleteChoiceBuilder(name, value) for name, value in res]
         if future := ctx._unset_future:
-            future.set_result(interaction.build_response(res))
+            future.set_result(interaction.build_response(choices))
         else:
-            await interaction.create_response(res)
+            await interaction.create_response(choices)
     except Exception as exc:
         handled = await command.client._autocomplete_error_handler.try_handle(
             exc, [exc, ctx, option]
         )
         await command.client.on_crescent_autocomplete_error(
             exc, ctx.into(AutocompleteContext), option, handled
         )
```

### Comparing `hikari_crescent-0.6.0/crescent/internal/includable.py` & `hikari_crescent-0.6.1/crescent/internal/includable.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/internal/registry.py` & `hikari_crescent-0.6.1/crescent/internal/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     command_type: CommandType,
     name: str | LocaleBuilder,
     guild: Snowflakeish | None = None,
     description: str | LocaleBuilder | None = None,
     options: Sequence[CommandOption] | None = None,
     default_member_permissions: UndefinedType | int | Permissions = UNDEFINED,
     dm_enabled: bool = True,
-    autocomplete: dict[str, AutocompleteCallbackT] = {},
+    autocomplete: dict[str, AutocompleteCallbackT[Any]] = {},
     nsfw: bool | None = None,
 ) -> Includable[AppCommandMeta]:
     if not iscoroutinefunction(callback):
         raise ValueError(f"`{callback.__name__}` must be an async function.")
 
     includable: Includable[AppCommandMeta] = Includable(
         client_set_hooks=[_command_client_set_hook],
```

### Comparing `hikari_crescent-0.6.0/crescent/locale.py` & `hikari_crescent-0.6.1/crescent/locale.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/mentionable.py` & `hikari_crescent-0.6.1/crescent/mentionable.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/plugin.py` & `hikari_crescent-0.6.1/crescent/plugin.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/typedefs.py` & `hikari_crescent-0.6.1/crescent/typedefs.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     TypeVar,
     Union,
 )
 
 from hikari import (
     Attachment,
     AutocompleteInteractionOption,
-    CommandChoice,
     Event,
     Message,
     PartialChannel,
     Role,
     User,
 )
 from hikari.api import EntityFactory
@@ -37,29 +36,32 @@
     "UserCommandCallbackT",
     "MessageCommandCallbackT",
     "CommandOptionsT",
     "ClassCommandProto",
     "HookCallbackT",
     "CommandErrorHandlerCallbackT",
     "AutocompleteCallbackT",
+    "AutocompleteValueT",
 )
 
 CommandCallbackT = Callable[..., Awaitable[Any]]
 UserCommandCallbackT = Callable[[Any, User], Awaitable[None]]
 MessageCommandCallbackT = Callable[[Any, Message], Awaitable[None]]
 
 OptionTypesT = Union[str, bool, int, float, PartialChannel, Role, User, "Mentionable", Attachment]
 CommandOptionsT = Dict[str, Union[OptionTypesT, User, Message]]
 HookCallbackT = Callable[[Any], Awaitable[Optional["HookResult"]]]
 TransformedHookCallbackT = Callable[[Any], Awaitable[Tuple[Optional["HookResult"], "BaseContext"]]]
+AutocompleteValueT = TypeVar("AutocompleteValueT", str, int, float)
 AutocompleteCallbackT = Callable[
-    [Any, AutocompleteInteractionOption], Awaitable[Sequence[CommandChoice]]
+    [Any, AutocompleteInteractionOption], Awaitable[Sequence[Tuple[str, AutocompleteValueT]]]
 ]
 TransformedAutocompleteCallbackT = Callable[
-    [Any, AutocompleteInteractionOption], Awaitable[Tuple[Sequence[CommandChoice], "BaseContext"]]
+    [Any, AutocompleteInteractionOption],
+    Awaitable[Tuple[Sequence[Tuple[str, AutocompleteValueT]], "BaseContext"]],
 ]
 
 PluginCallbackT = Callable[[], None]
 
 
 class ClassCommandProto(Protocol):
     async def callback(self, ctx: Any) -> Any:
```

### Comparing `hikari_crescent-0.6.0/crescent/utils/options.py` & `hikari_crescent-0.6.1/crescent/utils/options.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/crescent/utils/tasks.py` & `hikari_crescent-0.6.1/crescent/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `hikari_crescent-0.6.0/pyproject.toml` & `hikari_crescent-0.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-crescent"
-version = "v0.6.0"
+version = "v0.6.1"
 description = "🌙 A command handler for Hikari that keeps your project neat and tidy."
 readme = "README.md"
 authors = ["Lunarmagpie <bambolambo0@gmail.com>"]
 maintainers = [
     "Lunarmagpie <bambolambo0@gmail.com>",
     "Circuit <circuitsacul@icloud.com>",
 ]
@@ -21,45 +21,45 @@
 ]
 classifiers = ["Development Status :: 5 - Production/Stable"]
 include = ["crescent/banner.txt"]
 packages = [{ include = "crescent" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-hikari = ">=2.0.0.dev115"
+hikari = "==2.0.0.dev120"
 sigparse = "^3.0.0"
 floodgate-rs = { version = "^0.1.1", optional = true }
 types-croniter = { version = "==1.0.11", optional = true }
 croniter = { version = "^1.3.5", optional = true }
 python-i18n = { version = ">=0.2", optional = true }
 
 [tool.poetry.extras]
 i18n = ["python-i18n"]
 cron = ["croniter", "types-croniter"]
 cooldowns = ["floodgate-rs"]
 
 [tool.poetry.group.typing.dependencies]
-mypy = "^0.982"
-pyright = "^1.1.269"
-nox = ">=2022.8.7"
+mypy = "^1.4.0"
+pyright = "^1.1.315"
+nox = "^2023.4.22"
 
 [tool.poetry.group.linting.dependencies]
-ruff = ">=0.0.244"
-isort = "^5.10.1"
-black = ">=23.1.0"
-codespell = "^2.1.0"
+ruff = ">=0.0.274,<0.0.276"
+isort = "^5.12.0"
+black = "^23.3.0"
+codespell = "^2.2.5"
 
 [tool.poetry.group.doc.dependencies]
-pdoc = "^12.1.0"
+pdoc = ">=12.1,<15.0"
 
 [tool.poetry.group.tests.dependencies]
-pytest = "^7.0.0"
-pytest-asyncio = "^0.20.1"
-pytest-cov = "^4.0.0"
-python-dotenv = "^0.21.0"
+pytest = "^7.3.2"
+pytest-asyncio = "^0.21.0"
+pytest-cov = "^4.1.0"
+python-dotenv = "^1.0.0"
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 skip-magic-trailing-comma = true
 
 [tool.mypy]
```

### Comparing `hikari_crescent-0.6.0/setup.py` & `hikari_crescent-0.6.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,231 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: hikari-crescent
+Version: 0.6.1
+Summary: 🌙 A command handler for Hikari that keeps your project neat and tidy.
+Home-page: https://github.com/hikari-crescent/hikari-crescent
+License: MPL-2.0
+Keywords: discord,hikari,command handler,slash commands,application commands
+Author: Lunarmagpie
+Author-email: bambolambo0@gmail.com
+Maintainer: Lunarmagpie
+Maintainer-email: bambolambo0@gmail.com
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: cooldowns
+Provides-Extra: cron
+Provides-Extra: i18n
+Requires-Dist: croniter (>=1.3.5,<2.0.0) ; extra == "cron"
+Requires-Dist: floodgate-rs (>=0.1.1,<0.2.0) ; extra == "cooldowns"
+Requires-Dist: hikari (==2.0.0.dev120)
+Requires-Dist: python-i18n (>=0.2) ; extra == "i18n"
+Requires-Dist: sigparse (>=3.0.0,<4.0.0)
+Requires-Dist: types-croniter (==1.0.11) ; extra == "cron"
+Project-URL: Documentation, https://hikari-crescent.github.io/hikari-crescent/crescent.html
+Project-URL: Repository, https://github.com/hikari-crescent/hikari-crescent
+Description-Content-Type: text/markdown
+
+# hikari-crescent
+
+<div align="center">
+
+![Pypi](https://img.shields.io/pypi/v/hikari-crescent)
+[![ci](https://github.com/hikari-crescent/hikari-crescent/actions/workflows/ci.yml/badge.svg)](https://github.com/hikari-crescent/hikari-crescent/actions/workflows/ci.yml)
+![mypy](https://badgen.net/badge/mypy/checked/2A6DB2)
+![pyright](https://badgen.net/badge/pyright/checked/2A6DB2)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+![code-style-black](https://img.shields.io/badge/code%20style-black-black)
+
+</div>
+
+🌙 A command handler for [Hikari](https://github.com/hikari-py/hikari) that keeps your project neat and tidy.
+
+## Features
+ - Simple and intuitive API.
+ - Slash, user, and message commands.
+ - Command localization.
+ - Error handling for commands, events, and autocomplete.
+ - Hooks to run function before or after a command (or any command from a group!)
+ - Plugin system to easily split bot into different modules.
+ - Easily use a custom context class.
+ - Makes typehinting easy.
+ - RESTBot and GatewayBot support.
+
+### Links
+> 📖 | [User Guide](https://hikari-crescent.github.io/book)<br>
+> 🗃️ | [Docs](https://hikari-crescent.github.io/hikari-crescent/crescent.html)<br>
+> 📦 | [Pypi](https://pypi.org/project/hikari-crescent/)
+
+## Installation
+Crescent is supported in python3.8+.
+```
+pip install hikari-crescent
+```
+
+## Bots using Crescent
+
+- [mCodingBot](https://github.com/mcb-dev/mCodingBot) - The bot for the mCoding Discord server.
+- [Starboard 3](https://github.com/circuitsacul/starboard-3) - A starbord bot by [@CircuitSacul](https://github.com/CircuitSacul)
+in over 17k servers.
+
+
+## Usage
+Crescent uses [class commands](https://github.com/hikari-crescent/hikari-crescent/blob/main/examples/basic/basic.py)
+to simplify creating commands. Class commands allow you to create a command similar to how you declare a
+dataclass. The option function takes a type followed by the description, then optional information.
+
+```python
+import crescent
+import hikari
+
+bot = hikari.GatewayBot("YOUR_TOKEN")
+client = crescent.Client(bot)
+
+# Include the command in your client - don't forget this
+@client.include
+# Create a slash command
+@crescent.command(name="say")
+class Say:
+    word = crescent.option(str, "The word to say")
+
+    async def callback(self, ctx: crescent.Context) -> None:
+        await ctx.respond(self.word)
+
+bot.run()
+```
+
+Simple commands can use functions instead of classes. It is recommended to use a function when your
+command does not have any options.
+
+```python
+@client.include
+@crescent.command
+async def ping(ctx: crescent.Context):
+    await ctx.respond("Pong!")
+```
+
+Adding arguments to the function adds more options. Information for arguments can be provided using the `Annotated` type hint.
+See [this example](https://github.com/hikari-crescent/hikari-crescent/blob/main/examples/basic/function_commands.py) for more information.
+
+```python
+# python 3.9 +
+from typing import Annotated as Atd
+
+# python 3.8
+from typing_extensions import Annotated as Atd
+
+@client.include
+@crescent.command
+async def say(ctx: crescent.Context, word: str):
+    await ctx.respond(word)
+
+# The same command but with a description for `word`
+@client.include
+@crescent.command
+async def say(ctx: crescent.Context, word: Atd[str, "The word to say"]) -> None:
+    await ctx.respond(word)
+```
+
+
+### Typing to Option Types Lookup Table 
+| Type | Option Type |
+|---|---|
+| `str` | Text |
+| `int` | Integer |
+| `bool` | Boolean |
+| `float` | Number |
+| `hikari.User` | User |
+| `hikari.Role` | Role |
+| `crescent.Mentionable` | Role or User |
+| Any Hikari channel type. | Channel. The options will be the channel type and its subclasses. |
+| `List[Channel Types]` (classes only) | Channel. ^ |
+| `Union[Channel Types]` (functions only) | Channel. ^ |
+| `hikari.Attachment` | Attachment |
+
+
+### Autocomplete
+Autocomplete is supported by using a callback function. This function returns a list of tuples where the first
+value is the option name and the second value is the option value. `str`, `int`, and `float` value types
+can be used.
+
+```python
+async def autocomplete(
+    ctx: crescent.AutocompleteContext, option: hikari.AutocompleteInteractionOption
+) -> list[tuple[str, str]]:
+    return [("Option 1", "Option value 1"), ("Option 2", "Option value 2")]
+
+@client.include
+@crescent.command(name="class-command")
+class ClassCommand:
+    option = crescent.option(str, autocomplete=autocomplete)
+
+    async def callback(self) -> None:
+        await ctx.respond(self.option)
+
+@client.include
+@crescent.command
+async def function_command(
+    ctx: crescent.Context,
+    option: Annotated[str, crescent.Autocomplete(autocomplete)]
+) -> None:
+    await ctx.respond(option)
+```
+
+### Error Handling
+Errors that are raised by a command can be handled by `crescent.catch_command`.
+
+```python
+class MyError(Exception):
+    ...
+
+@client.include
+@crescent.catch_command(MyError)
+async def on_err(exc: MyError, ctx: crescent.Context) -> None:
+    await ctx.respond("An error occurred while running the command.")
+
+@client.include
+@crescent.command
+async def my_command(ctx: crescent.Context):
+    raise MyError()
+```
+
+There is also a `crescent.catch_event` and `crescent.catch_autocomplete` function for
+events and autocomplete respectively.
+
+### Events
+```python
+import hikari
+
+@client.include
+@crescent.event
+async def on_message_create(event: hikari.MessageCreateEvent):
+    if event.message.author.is_bot:
+        return
+    await event.message.respond("Hello!")
+```
+Using crescent's event decorator lets you use
+crescent's [event error handling system](https://github.com/hikari-crescent/hikari-crescent/blob/main/examples/error_handling/basic.py#L27).
+
+# Extensions
+Crescent has 3 builtin extensions.
+
+- [crescent-ext-cooldowns](https://github.com/hikari-crescent/hikari-crescent/tree/main/examples/ext/cooldowns) - Allows you to add sliding window rate limits to your commands.
+- [crescent-ext-locales](https://github.com/hikari-crescent/hikari-crescent/tree/main/examples/ext/locales) - Contains classes that cover common use cases for localization.
+- [crescent-ext-tasks](https://github.com/hikari-crescent/hikari-crescent/tree/main/examples/ext/tasks) - Schedules background tasks using loops or cronjobs.
+
+These extensions can be installed with pip.
 
-packages = \
-['crescent',
- 'crescent.commands',
- 'crescent.context',
- 'crescent.ext.cooldowns',
- 'crescent.ext.locales',
- 'crescent.ext.tasks',
- 'crescent.internal',
- 'crescent.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['hikari>=2.0.0.dev115', 'sigparse>=3.0.0,<4.0.0']
-
-extras_require = \
-{'cooldowns': ['floodgate-rs>=0.1.1,<0.2.0'],
- 'cron': ['types-croniter==1.0.11', 'croniter>=1.3.5,<2.0.0'],
- 'i18n': ['python-i18n>=0.2']}
-
-setup_kwargs = {
-    'name': 'hikari-crescent',
-    'version': '0.6.0',
-    'description': '🌙 A command handler for Hikari that keeps your project neat and tidy.',
-    'long_description': '# hikari-crescent\n\n<div align="center">\n\n![Pypi](https://img.shields.io/pypi/v/hikari-crescent)\n[![ci](https://github.com/hikari-crescent/hikari-crescent/actions/workflows/ci.yml/badge.svg)](https://github.com/hikari-crescent/hikari-crescent/actions/workflows/ci.yml)\n![mypy](https://badgen.net/badge/mypy/checked/2A6DB2)\n![pyright](https://badgen.net/badge/pyright/checked/2A6DB2)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n![code-style-black](https://img.shields.io/badge/code%20style-black-black)\n\n</div>\n\n🌙 A command handler for [Hikari](https://github.com/hikari-py/hikari) that keeps your project neat and tidy.\n\n## Features\n - Simple and intuitive API.\n - Slash, user, and message commands.\n - Command localization.\n - Error handling for commands, events, and autocomplete.\n - Hooks to run function before or after a command (or any command from a group!)\n - Plugin system to easily split bot into different modules.\n - Easily use a custom context class.\n - Makes typehinting easy.\n - RESTBot and GatewayBot support.\n\n### Links\n> 📖 | [User Guide](https://hikari-crescent.github.io/book)<br>\n> 🗃️ | [Docs](https://hikari-crescent.github.io/hikari-crescent/crescent.html)<br>\n> 📦 | [Pypi](https://pypi.org/project/hikari-crescent/)\n\n## Installation\nCrescent is supported in python3.8+.\n```\npip install hikari-crescent\n```\n\n## Bots using Crescent\n\n- [mCodingBot](https://github.com/mcb-dev/mCodingBot) - The bot for the mCoding Discord server.\n- [Starboard 3](https://github.com/circuitsacul/starboard-3) - A starbord bot by [@CircuitSacul](https://github.com/CircuitSacul)\nin over 17k servers.\n\n\n## Usage\nCrescent uses [class commands](https://github.com/hikari-crescent/hikari-crescent/blob/main/examples/basic/basic.py)\nto simplify creating commands. Class commands allow you to create a command similar to how you declare a\ndataclass. The option function takes a type followed by the description, then optional information.\n\n```python\nimport crescent\nimport hikari\n\nbot = hikari.GatewayBot("YOUR_TOKEN")\nclient = crescent.Client(bot)\n\n# Include the command in your client - don\'t forget this\n@client.include\n# Create a slash command\n@crescent.command(name="say")\nclass Say:\n    word = crescent.option(str, "The word to say")\n\n    async def callback(self, ctx: crescent.Context) -> None:\n        await ctx.respond(self.word)\n\nbot.run()\n```\n\nSimple commands can use functions instead of classes. It is recommended to use a function when your\ncommand does not have any options.\n\n```python\n@client.include\n@crescent.command\nasync def ping(ctx: crescent.Context):\n    await ctx.respond("Pong!")\n```\n\nAdding arguments to the function adds more options. Information for arguments can be provided using the `Annotated` type hint.\nSee [this example](https://github.com/hikari-crescent/hikari-crescent/blob/main/examples/basic/function_commands.py) for more information.\n\n```python\n# python 3.9 +\nfrom typing import Annotated as Atd\n\n# python 3.8\nfrom typing_extensions import Annotated as Atd\n\n@client.include\n@crescent.command\nasync def say(ctx: crescent.Context, word: str):\n    await ctx.respond(word)\n\n# The same command but with a description for `word`\n@client.include\n@crescent.command\nasync def say(ctx: crescent.Context, word: Atd[str, "The word to say"]) -> None:\n    await ctx.respond(word)\n```\n\n\n### Typing to Option Types Lookup Table \n| Type | Option Type |\n|---|---|\n| `str` | Text |\n| `int` | Integer |\n| `bool` | Boolean |\n| `float` | Number |\n| `hikari.User` | User |\n| `hikari.Role` | Role |\n| `crescent.Mentionable` | Role or User |\n| Any Hikari channel type. | Channel. The options will be the channel type and its subclasses. |\n| `List[Channel Types]` (classes only) | Channel. ^ |\n| `Union[Channel Types]` (functions only) | Channel. ^ |\n| `hikari.Attachment` | Attachment |\n\n\n### Error Handling\nErrors that are raised by a command can be handled by `crescent.catch_command`.\n\n```python\nclass MyError(Exception):\n    ...\n\n@client.include\n@crescent.catch_command(MyError)\nasync def on_err(exc: MyError, ctx: crescent.Context) -> None:\n    await ctx.respond("An error occurred while running the command.")\n\n@client.include\n@crescent.command\nasync def my_command(ctx: crescent.Context):\n    raise MyError()\n```\n\n### Events\n```python\nimport hikari\n\n@client.include\n@crescent.event\nasync def on_message_create(event: hikari.MessageCreateEvent):\n    if event.message.author.is_bot:\n        return\n    await event.message.respond("Hello!")\n```\nUsing crescent\'s event decorator lets you use\ncrescent\'s [event error handling system](https://github.com/hikari-crescent/hikari-crescent/blob/main/examples/error_handling/basic.py#L27).\n\n# Extensions\nCrescent has 3 builtin extensions.\n\n- [crescent-ext-cooldowns](https://github.com/hikari-crescent/hikari-crescent/tree/main/examples/ext/cooldowns) - Allows you to add sliding window rate limits to your commands.\n- [crescent-ext-locales](https://github.com/hikari-crescent/hikari-crescent/tree/main/examples/ext/locales) - Contains classes that cover common use cases for localization.\n- [crescent-ext-tasks](https://github.com/hikari-crescent/hikari-crescent/tree/main/examples/ext/tasks) - Schedules background tasks using loops or cronjobs.\n\nThese extensions can be installed with pip.\n\n- [crescent-ext-docstrings](https://github.com/hikari-crescent/crescent-ext-docstrings) - Lets you use docstrings to write descriptions for commands and options.\n- [crescent-ext-kebabify](https://github.com/hikari-crescent/crescent-ext-kebabify) - Turns your command names into kebabs!\n\n# Support\nYou can ask questions in the `#crescent` channel in the [Hikari Discord server](https://discord.gg/Jx4cNGG). My Discord username is `Lunarmagpie❤#0001`.\n\n# Contributing\nCreate an issue for your feature. There aren\'t any guidelines right now so just don\'t be rude.\n',
-    'author': 'Lunarmagpie',
-    'author_email': 'bambolambo0@gmail.com',
-    'maintainer': 'Lunarmagpie',
-    'maintainer_email': 'bambolambo0@gmail.com',
-    'url': 'https://github.com/hikari-crescent/hikari-crescent',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<3.12',
-}
+- [crescent-ext-docstrings](https://github.com/hikari-crescent/crescent-ext-docstrings) - Lets you use docstrings to write descriptions for commands and options.
+- [crescent-ext-kebabify](https://github.com/hikari-crescent/crescent-ext-kebabify) - Turns your command names into kebabs!
 
+# Support
+You can ask questions in the `#crescent` channel in the [Hikari Discord server](https://discord.gg/Jx4cNGG). My Discord username is `lunarmagpie`.
+
+# Contributing
+Create an issue for your feature. There aren't any guidelines right now so just don't be rude.
 
-setup(**setup_kwargs)
```

