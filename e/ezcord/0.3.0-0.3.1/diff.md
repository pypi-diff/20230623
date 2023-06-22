# Comparing `tmp/ezcord-0.3.0.tar.gz` & `tmp/ezcord-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcord-0.3.0.tar", last modified: Sun Jun 18 19:32:45 2023, max compression
+gzip compressed data, was "ezcord-0.3.1.tar", last modified: Thu Jun 22 22:40:26 2023, max compression
```

## Comparing `ezcord-0.3.0.tar` & `ezcord-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 19:32:35.000000 ezcord-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-18 19:32:35.000000 ezcord-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-18 19:32:45.111140 ezcord-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-18 19:32:35.000000 ezcord-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 19:32:35.000000 ezcord-0.3.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-18 19:32:35.000000 ezcord-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-18 19:32:35.000000 ezcord-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 19:32:35.000000 ezcord-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 19:32:45.115140 ezcord-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.107140 ezcord-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/src/ezcord/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/src/ezcord/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/cogs/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/src/ezcord/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/embed_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/funcutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/src/ezcord/internal/language/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/language/de.json
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/language/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/language/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/ready_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/internal/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-18 19:32:35.000000 ezcord-0.3.0/src/ezcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 19:32:45.111140 ezcord-0.3.0/src/ezcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-18 19:32:45.000000 ezcord-0.3.0/src/ezcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-18 19:32:45.000000 ezcord-0.3.0/src/ezcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 19:32:45.000000 ezcord-0.3.0/src/ezcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-18 19:32:45.000000 ezcord-0.3.0/src/ezcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 19:32:45.000000 ezcord-0.3.0/src/ezcord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.718749 ezcord-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-22 22:40:14.000000 ezcord-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 22:40:14.000000 ezcord-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-22 22:40:26.718749 ezcord-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-22 22:40:14.000000 ezcord-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 22:40:14.000000 ezcord-0.3.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.710749 ezcord-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 22:40:14.000000 ezcord-0.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-22 22:40:14.000000 ezcord-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 22:40:14.000000 ezcord-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:40:26.718749 ezcord-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.710749 ezcord-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.714749 ezcord-0.3.1/src/ezcord/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18525 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.714749 ezcord-0.3.1/src/ezcord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/cogs/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.718749 ezcord-0.3.1/src/ezcord/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/embed_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/funcutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.718749 ezcord-0.3.1/src/ezcord/internal/language/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/language/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/language/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/language/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/ready_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/internal/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-22 22:40:14.000000 ezcord-0.3.1/src/ezcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:40:26.714749 ezcord-0.3.1/src/ezcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-22 22:40:26.000000 ezcord-0.3.1/src/ezcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-22 22:40:26.000000 ezcord-0.3.1/src/ezcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:40:26.000000 ezcord-0.3.1/src/ezcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-22 22:40:26.000000 ezcord-0.3.1/src/ezcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 22:40:26.000000 ezcord-0.3.1/src/ezcord.egg-info/top_level.txt
```

### Comparing `ezcord-0.3.0/LICENSE` & `ezcord-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.0/PKG-INFO` & `ezcord-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.3.0
+Version: 0.3.1
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.3.0/README.md` & `ezcord-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.0/pyproject.toml` & `ezcord-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.0/src/ezcord/bot.py` & `ezcord-0.3.1/src/ezcord/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,16 +305,15 @@
             Colors can only be used with :attr:`.ReadyEvent.box_colorful` and all table styles.
         """
         modifications = self.ready_event_adds, self.ready_event_removes
         print_custom_ready(self, title, modifications, style, default_info, new_info, colors)
 
     async def _ready_event(self):
         """Prints the bot's information when it's ready."""
-        if len(self.ready_event_adds) > 0 or len(self.ready_event_removes) > 0:
-            await asyncio.sleep(0.5)
+        await asyncio.sleep(0.1)
 
         modifications = self.ready_event_adds, self.ready_event_removes
         print_ready(self, self.ready_event, modifications=modifications)
 
     async def _check_cog_groups(self):
         """Checks if all cog groups are valid."""
         for cog in self.cogs.values():
@@ -408,44 +407,68 @@
                     "Please check if the URL is correct."
                 )
             else:
                 webhook_sent = True
 
         return webhook_sent
 
+    def get_cmd(self, name: str, bold: bool = True) -> str:
+        """Helper method to get a command mention. Returns a string if the command was not found.
+
+        Parameters
+        ----------
+        name:
+            The name of the command to get.
+        bold:
+            Whether to bold the command name. Defaults to ``True``.
+        """
+        cmd = self.get_application_command(name)
+        if cmd is None:
+            return f"**/{name}**" if bold else f"/{name}"
+        return cmd.mention
+
     def add_help_command(
         self,
         *,
         style: HelpStyle = HelpStyle.embed_description,
         embed: discord.Embed | None = None,
         show_categories: bool = True,
+        timeout: int = 500,
         ephemeral: bool = True,
+        author_only: bool = True,
     ):
         """Add a help command that uses a select menu to group commands by cogs.
 
         If you use :class:`Cog`, you can pass in emojis to use for the select menu.
 
         Parameters
         ----------
         style:
             The style to use for the help command. Defaults to :attr:`.HelpStyle.default`.
         embed:
             The embed to use for the help command. If this is ``None``, a default
             embed will be used.
         show_categories:
             Whether to display the categories of the help command front page. Defaults to ``True``.
+        timeout:
+            The timeout for the select menu. Defaults to ``500``.
         ephemeral:
-            Whether the help command should be ephemeral. Defaults to ``False``.
+            Whether the help command should be ephemeral. Defaults to ``True``.
+        author_only:
+            Whether the help command should only be visible to the author. Defaults to ``True``.
+            This only works if ``ephemeral`` is ``False``.
         """
-        self.load_extension(f".cogs.help", package="src.ezcord")
+        self.load_extension(f".cogs.help", package="ezcord")
         self.help = {
             "style": style,
             "embed": embed,
             "show_categories": show_categories,
+            "timeout": timeout,
             "ephemeral": ephemeral,
+            "author_only": author_only,
         }
 
 
 class PrefixBot(Bot, commands.Bot):
     """A subclass of :class:`discord.ext.commands.Bot` that implements the :class:`Bot` class.
 
     This class can be used if you want to use EzCord with prefix commands.
```

### Comparing `ezcord-0.3.0/src/ezcord/cogs/help.py` & `ezcord-0.3.1/src/ezcord/cogs/help.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import random
 
 import discord
 from discord.commands import slash_command
 
+from .. import emb
 from ..bot import Bot, Cog
-from ..components import EzView
 from ..enums import HelpStyle
-from ..internal import t
+from ..internal import replace_embed_values, t
 from ..logs import log
 
 
 def get_emoji(cog: Cog) -> str:
     if hasattr(cog, "emoji") and cog.emoji:
         emoji = cog.emoji
     else:
@@ -24,22 +24,24 @@
 def get_group(cog: Cog) -> str | None:
     if hasattr(cog, "group") and cog.group:
         return cog.group
     return None
 
 
 class Help(Cog, hidden=True):
-    @slash_command(name="help", description=t("cmd_description"))
-    async def help(self, ctx):
+    @slash_command(name=t("cmd_name"), description=t("cmd_description"))
+    async def help(self, ctx: discord.ApplicationContext):
         embed = self.bot.help["embed"]
         if embed is None:
             embed = discord.Embed(title=t("embed_title"), color=discord.Color.blue())
+        else:
+            embed = replace_embed_values(embed, ctx.interaction)
 
         options = []
-        commands = {}
+        commands: dict[str, dict] = {}
         for name, cog in self.bot.cogs.items():
             if hasattr(cog, "hidden") and cog.hidden:
                 continue
 
             group = get_group(cog)
             name = group if group else name
             name = name.title()
@@ -101,27 +103,29 @@
     ):
         super().__init__(min_values=1, max_values=1, placeholder=t("placeholder"), options=options)
         self.bot = bot
         self.member = member
         self.commands = commands
 
     async def callback(self, interaction: discord.Interaction):
-        if interaction.user != self.member:
-            return await interaction.response.send_message(t("wrong_user"), ephemeral=True)
+        if self.bot.help["author_only"] and interaction.user != self.member:
+            return await emb.error(interaction, t("wrong_user"))
 
         cmds = self.commands[self.values[0]]
         title = self.values[0].title()
         emoji = cmds["emoji"]
 
         embed = self.bot.help["embed"]
         if embed is None:
             embed = discord.Embed(
-                title=f"`{emoji}` - {title}",
                 color=discord.Color.blue(),
             )
+        else:
+            embed = replace_embed_values(embed, interaction)
+        embed.title = f"`{emoji}` - {title}"
         embed.clear_fields()
 
         commands = cmds["cmds"]
         embed_field_styles = [
             HelpStyle.embed_fields,
             HelpStyle.codeblocks_inline,
             HelpStyle.codeblocks,
@@ -165,17 +169,17 @@
                     break
 
         await interaction.response.edit_message(
             embed=embed, view=CategoryView(self.options, self.bot, self.member, self.commands)
         )
 
 
-class CategoryView(EzView):
+class CategoryView(discord.ui.View):
     def __init__(
         self,
         options: list[discord.SelectOption],
         bot: Bot,
         member: discord.Member | discord.User,
         commands: dict[str, dict],
     ):
-        super().__init__(timeout=500, disable_on_timeout=True)
+        super().__init__(timeout=bot.help["timeout"], disable_on_timeout=True)
         self.add_item(CategorySelect(options, bot, member, commands))
```

### Comparing `ezcord-0.3.0/src/ezcord/components.py` & `ezcord-0.3.1/src/ezcord/components.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.0/src/ezcord/emb.py` & `ezcord-0.3.1/src/ezcord/emb.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from __future__ import annotations
 
 import copy
 
 import discord
 
-from .internal import copy_kwargs, load_embed, save_embeds
+from .internal import copy_kwargs, load_embed, replace_dict, save_embeds
 
 
 def set_embed_templates(
     *,
     error_embed: discord.Embed | str | None = None,
     success_embed: discord.Embed | str | None = None,
     warn_embed: discord.Embed | str | None = None,
@@ -121,53 +121,14 @@
             )
         else:
             await target.followup.send(content=content, embed=embed, ephemeral=ephemeral, **kwargs)
     else:
         await target.send(content=content, embed=embed, **kwargs)
 
 
-def _replace_values(s: str, interaction: discord.Interaction) -> str:
-    user = interaction.user
-    s = s.replace("{user}", f"{user}")
-    s = s.replace("{username}", user.name)
-    s = s.replace("{user_mention}", user.mention)
-    s = s.replace("{user_id}", f"{user.id}")
-    s = s.replace("{user_avatar}", user.display_avatar.url)
-
-    if interaction.guild:
-        s = s.replace("{servername}", interaction.guild.name)
-    else:
-        s = s.replace("{servername}", interaction.client.user.name)
-
-    if interaction.guild and interaction.guild.icon:
-        s = s.replace("{server_icon}", interaction.guild.icon.url)
-    else:
-        s = s.replace("{server_icon}", interaction.client.user.display_avatar.url)
-
-    return s
-
-
-def _loop_object(content: dict | str, interaction: discord.Interaction) -> dict | str:
-    if isinstance(content, str):
-        return _replace_values(content, interaction)
-
-    for key, value in content.items():
-        if isinstance(value, str):
-            content[key] = _replace_values(value, interaction)
-        elif isinstance(value, list):
-            items = []
-            for element in value:
-                items.append(_loop_object(element, interaction))
-            content[key] = items
-        elif isinstance(value, dict):
-            content[key] = _loop_object(value, interaction)
-
-    return content
-
-
 def _insert_info(
     target: discord.ApplicationContext | discord.Interaction | discord.abc.Messageable,
     embed: discord.Embed | str,
 ):
     if not isinstance(target, discord.ApplicationContext) and not isinstance(
         target, discord.Interaction
     ):
@@ -175,15 +136,15 @@
 
     interaction = target
     if isinstance(target, discord.ApplicationContext):
         interaction = target.interaction
 
     if isinstance(embed, discord.Embed):
         embed = embed.to_dict()
-    embed_dic = _loop_object(embed, interaction)
+    embed_dic = replace_dict(embed, interaction)
 
     if isinstance(embed, dict):
         return discord.Embed.from_dict(embed_dic)
 
     return embed_dic
```

### Comparing `ezcord-0.3.0/src/ezcord/enums.py` & `ezcord-0.3.1/src/ezcord/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,19 +56,18 @@
     - ``{directory}`` is the directory where a cog was loaded from.
     - ``{path}`` is the path of a cog.
     - ``{sum}`` is the amount of cogs that were loaded.
 
     If ``{sum}`` is used, no other variables except ``{directory}`` can be used.
     """
 
-    default = "Loaded **{cog}**"
-    no_color = "Loaded {cog}"
     sum = "Loaded {sum} cogs"
     directory_sum = "Loaded {sum} cogs from {directory}"
     path = "Loaded {path}"
+    default = "Loaded {cog}"
 
     def __str__(self):
         return self.name
 
 
 class ReadyEvent(Enum):
     """Styles for the ready event. This can be used in :class:`.Bot`."""
```

### Comparing `ezcord-0.3.0/src/ezcord/internal/colors.py` & `ezcord-0.3.1/src/ezcord/internal/colors.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.0/src/ezcord/internal/language/de.json` & `ezcord-0.3.1/src/ezcord/internal/language/de.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'help'": "{'wrong_user': 'Dieser Help Command gehört dir nicht!', 'cmd_name': 'help'}"}*

```diff
@@ -5,19 +5,20 @@
         "error": "Der folgende Fehler ist aufgetreten: {}",
         "error_title": "Error",
         "no_perms": "Mir fehlen die folgenden Berechtigungen, um diesen Befehl auszuf\u00fchren.",
         "no_perms_title": "Fehlende Rechte"
     },
     "help": {
         "cmd_description": "Zeigt alle Befehle an.",
+        "cmd_name": "help",
         "default_description": "Alle Befehle der Kategorie **{}**.",
         "embed_title": "Meine Befehle",
         "no_commands": "Ups, ich konnte keine Befehle finden.",
         "placeholder": "\ud83d\udd30 \u203a W\u00e4hle eine Kategorie aus",
-        "wrong_user": "Dieser Help Command geh\u00f6rt dir nicht."
+        "wrong_user": "Dieser Help Command geh\u00f6rt dir nicht!"
     },
     "times": {
         "day": "Tag",
         "hour": "Stunde",
         "min": "Minute",
         "sec": "Sekunde"
     }
```

### Comparing `ezcord-0.3.0/src/ezcord/internal/language/en.json` & `ezcord-0.3.1/src/ezcord/internal/language/en.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904763%*

 * *Differences: {"'help'": "{'cmd_name': 'help'}"}*

```diff
@@ -5,14 +5,15 @@
         "error": "The following error occurred: {}",
         "error_title": "Error",
         "no_perms": "I'm missing the following permissions to execute this command.",
         "no_perms_title": "Missing permissions"
     },
     "help": {
         "cmd_description": "Show all commands",
+        "cmd_name": "help",
         "default_description": "All commands of category **{}**.",
         "embed_title": "My commands",
         "no_commands": "Oops, I didn't find any commands.",
         "placeholder": "\ud83d\udd30 \u203a Choose a category",
         "wrong_user": "This help command does not belong to you!"
     },
     "times": {
```

### Comparing `ezcord-0.3.0/src/ezcord/internal/language/languages.py` & `ezcord-0.3.1/src/ezcord/internal/language/languages.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.0/src/ezcord/internal/ready_style.py` & `ezcord-0.3.1/src/ezcord/internal/ready_style.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.0/src/ezcord/internal/translation.py` & `ezcord-0.3.1/src/ezcord/internal/translation.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.0/src/ezcord/logs.py` & `ezcord-0.3.1/src/ezcord/logs.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.0/src/ezcord/sql.py` & `ezcord-0.3.1/src/ezcord/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
     @staticmethod
     def _process_args(args) -> tuple:
         """If SQL query parameters are passed as a tuple instead of single values,
         the tuple will be unpacked.
         """
         if len(args) == 1 and isinstance(args, tuple):
-            return args[0]
+            if isinstance(args[0], tuple):
+                return args[0]
         return args
 
     def start(self):
         """Returns an instance of :class:`.DBHandler` with the current settings
         and ``transaction=True``.
         """
         cls = deepcopy(self)
@@ -65,14 +66,15 @@
 
         db = await aiosqlite.connect(self.DB, **con_args)
         return db
 
     async def close(self):
         """Close the current connection to the database."""
         if self.connection is not None:
+            await self.connection.commit()
             await self.connection.close()
 
     async def one(self, sql: str, *args, **kwargs):
         """Returns one result row. If no row is found, ``None`` is returned.
 
         If the query returns only one column, the value of that column is returned.
```

### Comparing `ezcord-0.3.0/src/ezcord/times.py` & `ezcord-0.3.1/src/ezcord/times.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.0/src/ezcord/utils.py` & `ezcord-0.3.1/src/ezcord/utils.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.3.0/src/ezcord.egg-info/PKG-INFO` & `ezcord-0.3.1/src/ezcord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.3.0
+Version: 0.3.1
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.3.0/src/ezcord.egg-info/SOURCES.txt` & `ezcord-0.3.1/src/ezcord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

