# Comparing `tmp/ikomia_cli-0.1.0-py3-none-any.whl.zip` & `tmp/ikomia_cli-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,42 +1,53 @@
-Zip file size: 33265 bytes, number of entries: 40
+Zip file size: 50438 bytes, number of entries: 51
 -rw-r--r--  2.0 unx       82 b- defN 22-Oct-27 15:07 ikcli/__init__.py
--rw-r--r--  2.0 unx     2759 b- defN 22-Dec-16 13:40 ikcli/cli.py
--rw-r--r--  2.0 unx       86 b- defN 22-Dec-16 13:40 ikcli/algo/__init__.py
--rw-r--r--  2.0 unx     2274 b- defN 22-Dec-16 13:40 ikcli/algo/cli.py
--rw-r--r--  2.0 unx    13807 b- defN 22-Dec-16 13:40 ikcli/algo/core.py
--rw-r--r--  2.0 unx      792 b- defN 22-Dec-16 13:40 ikcli/algo/templates/entry_point.pyt
--rw-r--r--  2.0 unx     3804 b- defN 22-Dec-16 13:40 ikcli/algo/templates/process.pyt
--rw-r--r--  2.0 unx      173 b- defN 22-Dec-16 13:40 ikcli/algo/templates/pyqt_layout.pyt
--rw-r--r--  2.0 unx      189 b- defN 22-Dec-16 13:40 ikcli/algo/templates/pyside_layout.pyt
--rw-r--r--  2.0 unx      584 b- defN 22-Dec-16 13:40 ikcli/algo/templates/test.pyt
--rw-r--r--  2.0 unx     1548 b- defN 22-Dec-16 13:40 ikcli/algo/templates/widget.pyt
+-rw-r--r--  2.0 unx     4155 b- defN 23-Jun-23 08:19 ikcli/cli.py
+-rw-r--r--  2.0 unx       81 b- defN 23-Jun-23 08:19 ikcli/algos/__init__.py
+-rw-r--r--  2.0 unx    11392 b- defN 23-Jun-23 08:19 ikcli/algos/cli.py
+-rw-r--r--  2.0 unx     6904 b- defN 23-Jun-23 08:19 ikcli/algos/core.py
+-rw-r--r--  2.0 unx    10538 b- defN 23-Jun-23 08:19 ikcli/algos/local.py
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-23 08:19 ikcli/algos/templates/cookiecutter.json
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 08:19 ikcli/algos/templates/{{cookiecutter.plugin_dir}}/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 08:19 ikcli/algos/templates/{{cookiecutter.plugin_dir}}/requirements.txt
+-rw-r--r--  2.0 unx      918 b- defN 23-Jun-23 08:19 ikcli/algos/templates/{{cookiecutter.plugin_dir}}/{{cookiecutter.algo_name}}.py
+-rw-r--r--  2.0 unx     4104 b- defN 23-Jun-23 08:19 ikcli/algos/templates/{{cookiecutter.plugin_dir}}/{{cookiecutter.algo_name}}_process.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Jun-23 08:19 ikcli/algos/templates/{{cookiecutter.plugin_dir}}/{{cookiecutter.algo_name}}_test.py
+-rw-r--r--  2.0 unx     2421 b- defN 23-Jun-23 08:19 ikcli/algos/templates/{{cookiecutter.plugin_dir}}/{{cookiecutter.algo_name}}_widget.py
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-23 08:19 ikcli/common/__init__.py
+-rw-r--r--  2.0 unx      291 b- defN 23-Jun-23 08:19 ikcli/common/cli.py
+-rw-r--r--  2.0 unx     1089 b- defN 23-Jun-23 08:19 ikcli/common/core.py
+-rw-r--r--  2.0 unx       80 b- defN 23-Jun-23 08:19 ikcli/hub/__init__.py
+-rw-r--r--  2.0 unx     2989 b- defN 23-Jun-23 08:19 ikcli/hub/cli.py
+-rw-r--r--  2.0 unx     1398 b- defN 23-Jun-23 08:19 ikcli/hub/core.py
 -rw-r--r--  2.0 unx       86 b- defN 22-Oct-27 15:07 ikcli/namespaces/__init__.py
--rw-r--r--  2.0 unx     1638 b- defN 22-Dec-16 13:40 ikcli/namespaces/cli.py
--rw-r--r--  2.0 unx     1099 b- defN 22-Dec-16 13:24 ikcli/namespaces/core.py
+-rw-r--r--  2.0 unx     4329 b- defN 23-Jun-23 08:19 ikcli/namespaces/cli.py
+-rw-r--r--  2.0 unx     1816 b- defN 23-Jun-23 08:19 ikcli/namespaces/core.py
 -rw-r--r--  2.0 unx       89 b- defN 22-Oct-27 15:07 ikcli/net/__init__.py
 -rw-r--r--  2.0 unx      109 b- defN 22-Oct-27 15:07 ikcli/net/api/__init__.py
--rw-r--r--  2.0 unx     4369 b- defN 22-Dec-16 13:24 ikcli/net/api/core.py
--rw-r--r--  2.0 unx     1074 b- defN 22-Dec-16 13:24 ikcli/net/api/exceptions.py
--rw-r--r--  2.0 unx     3598 b- defN 22-Dec-16 13:24 ikcli/net/api/pagination.py
--rw-r--r--  2.0 unx      714 b- defN 22-Dec-16 13:40 ikcli/net/http/__init__.py
--rw-r--r--  2.0 unx     1037 b- defN 22-Dec-16 13:24 ikcli/net/http/auth.py
--rw-r--r--  2.0 unx     6897 b- defN 22-Dec-16 13:40 ikcli/net/http/core.py
--rw-r--r--  2.0 unx      872 b- defN 22-Dec-16 13:24 ikcli/net/http/exceptions.py
--rw-r--r--  2.0 unx     5227 b- defN 22-Dec-16 13:40 ikcli/net/http/serializer.py
+-rw-r--r--  2.0 unx     5279 b- defN 23-Jun-23 08:19 ikcli/net/api/core.py
+-rw-r--r--  2.0 unx     1357 b- defN 23-Jun-23 08:19 ikcli/net/api/exceptions.py
+-rw-r--r--  2.0 unx     4460 b- defN 23-Jun-23 08:19 ikcli/net/api/pagination.py
+-rw-r--r--  2.0 unx      638 b- defN 23-Jun-23 08:19 ikcli/net/http/__init__.py
+-rw-r--r--  2.0 unx     3016 b- defN 23-Jun-23 08:19 ikcli/net/http/auth.py
+-rw-r--r--  2.0 unx    10190 b- defN 23-Jun-23 08:19 ikcli/net/http/core.py
+-rw-r--r--  2.0 unx      886 b- defN 23-Jun-23 08:19 ikcli/net/http/exceptions.py
+-rw-r--r--  2.0 unx     1171 b- defN 23-Jun-23 08:19 ikcli/net/http/progress.py
+-rw-r--r--  2.0 unx     5427 b- defN 23-Jun-23 08:19 ikcli/net/http/serializer.py
 -rw-r--r--  2.0 unx       88 b- defN 22-Oct-27 15:07 ikcli/organizations/__init__.py
--rw-r--r--  2.0 unx     3867 b- defN 22-Dec-16 13:40 ikcli/organizations/cli.py
--rw-r--r--  2.0 unx     1370 b- defN 22-Dec-16 13:24 ikcli/organizations/core.py
+-rw-r--r--  2.0 unx     4353 b- defN 23-Jun-23 08:19 ikcli/organizations/cli.py
+-rw-r--r--  2.0 unx     1108 b- defN 23-Jun-23 08:19 ikcli/organizations/core.py
 -rw-r--r--  2.0 unx       83 b- defN 22-Oct-27 15:07 ikcli/projects/__init__.py
--rw-r--r--  2.0 unx     3862 b- defN 22-Dec-16 13:24 ikcli/projects/archive.py
--rw-r--r--  2.0 unx     9227 b- defN 22-Dec-16 13:40 ikcli/projects/cli.py
--rw-r--r--  2.0 unx     3707 b- defN 22-Dec-16 13:40 ikcli/projects/core.py
+-rw-r--r--  2.0 unx     3839 b- defN 23-Jun-23 08:19 ikcli/projects/archive.py
+-rw-r--r--  2.0 unx    14091 b- defN 23-Jun-23 08:19 ikcli/projects/cli.py
+-rw-r--r--  2.0 unx     4199 b- defN 23-Jun-23 08:19 ikcli/projects/core.py
+-rw-r--r--  2.0 unx     4690 b- defN 23-Jun-23 08:19 ikcli/projects/http.py
 -rw-r--r--  2.0 unx       80 b- defN 22-Oct-27 15:07 ikcli/users/__init__.py
--rw-r--r--  2.0 unx     1896 b- defN 22-Dec-16 13:24 ikcli/users/core.py
+-rw-r--r--  2.0 unx     2490 b- defN 23-Jun-23 08:19 ikcli/users/core.py
 -rw-r--r--  2.0 unx       79 b- defN 22-Oct-27 15:07 ikcli/utils/__init__.py
--rw-r--r--  2.0 unx     7729 b- defN 22-Dec-16 13:40 ikcli/utils/rich.py
--rw-r--r--  2.0 unx     1025 b- defN 22-Dec-16 14:11 ikomia_cli-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-16 14:11 ikomia_cli-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 22-Dec-16 14:11 ikomia_cli-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 22-Dec-16 14:11 ikomia_cli-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3252 b- defN 22-Dec-16 14:11 ikomia_cli-0.1.0.dist-info/RECORD
-40 files, 89310 bytes uncompressed, 28093 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx    12263 b- defN 23-Jun-23 08:19 ikcli/utils/rich.py
+-rw-r--r--  2.0 unx     5174 b- defN 23-Jun-23 08:19 ikcli/utils/version.py
+-rw-r--r--  2.0 unx     1186 b- defN 23-Jun-23 08:21 ikomia_cli-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 08:21 ikomia_cli-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-23 08:21 ikomia_cli-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-23 08:21 ikomia_cli-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4383 b- defN 23-Jun-23 08:21 ikomia_cli-0.2.0.dist-info/RECORD
+51 files, 144346 bytes uncompressed, 43410 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -1,38 +1,62 @@
 Filename: ikcli/__init__.py
 Comment: 
 
 Filename: ikcli/cli.py
 Comment: 
 
-Filename: ikcli/algo/__init__.py
+Filename: ikcli/algos/__init__.py
 Comment: 
 
-Filename: ikcli/algo/cli.py
+Filename: ikcli/algos/cli.py
 Comment: 
 
-Filename: ikcli/algo/core.py
+Filename: ikcli/algos/core.py
 Comment: 
 
-Filename: ikcli/algo/templates/entry_point.pyt
+Filename: ikcli/algos/local.py
 Comment: 
 
-Filename: ikcli/algo/templates/process.pyt
+Filename: ikcli/algos/templates/cookiecutter.json
 Comment: 
 
-Filename: ikcli/algo/templates/pyqt_layout.pyt
+Filename: ikcli/algos/templates/{{cookiecutter.plugin_dir}}/__init__.py
 Comment: 
 
-Filename: ikcli/algo/templates/pyside_layout.pyt
+Filename: ikcli/algos/templates/{{cookiecutter.plugin_dir}}/requirements.txt
 Comment: 
 
-Filename: ikcli/algo/templates/test.pyt
+Filename: ikcli/algos/templates/{{cookiecutter.plugin_dir}}/{{cookiecutter.algo_name}}.py
 Comment: 
 
-Filename: ikcli/algo/templates/widget.pyt
+Filename: ikcli/algos/templates/{{cookiecutter.plugin_dir}}/{{cookiecutter.algo_name}}_process.py
+Comment: 
+
+Filename: ikcli/algos/templates/{{cookiecutter.plugin_dir}}/{{cookiecutter.algo_name}}_test.py
+Comment: 
+
+Filename: ikcli/algos/templates/{{cookiecutter.plugin_dir}}/{{cookiecutter.algo_name}}_widget.py
+Comment: 
+
+Filename: ikcli/common/__init__.py
+Comment: 
+
+Filename: ikcli/common/cli.py
+Comment: 
+
+Filename: ikcli/common/core.py
+Comment: 
+
+Filename: ikcli/hub/__init__.py
+Comment: 
+
+Filename: ikcli/hub/cli.py
+Comment: 
+
+Filename: ikcli/hub/core.py
 Comment: 
 
 Filename: ikcli/namespaces/__init__.py
 Comment: 
 
 Filename: ikcli/namespaces/cli.py
 Comment: 
@@ -63,14 +87,17 @@
 
 Filename: ikcli/net/http/core.py
 Comment: 
 
 Filename: ikcli/net/http/exceptions.py
 Comment: 
 
+Filename: ikcli/net/http/progress.py
+Comment: 
+
 Filename: ikcli/net/http/serializer.py
 Comment: 
 
 Filename: ikcli/organizations/__init__.py
 Comment: 
 
 Filename: ikcli/organizations/cli.py
@@ -87,35 +114,41 @@
 
 Filename: ikcli/projects/cli.py
 Comment: 
 
 Filename: ikcli/projects/core.py
 Comment: 
 
+Filename: ikcli/projects/http.py
+Comment: 
+
 Filename: ikcli/users/__init__.py
 Comment: 
 
 Filename: ikcli/users/core.py
 Comment: 
 
 Filename: ikcli/utils/__init__.py
 Comment: 
 
 Filename: ikcli/utils/rich.py
 Comment: 
 
-Filename: ikomia_cli-0.1.0.dist-info/METADATA
+Filename: ikcli/utils/version.py
+Comment: 
+
+Filename: ikomia_cli-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: ikomia_cli-0.1.0.dist-info/WHEEL
+Filename: ikomia_cli-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: ikomia_cli-0.1.0.dist-info/entry_points.txt
+Filename: ikomia_cli-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ikomia_cli-0.1.0.dist-info/top_level.txt
+Filename: ikomia_cli-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ikomia_cli-0.1.0.dist-info/RECORD
+Filename: ikomia_cli-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ikcli/cli.py

```diff
@@ -7,103 +7,142 @@
 import rich.padding
 import rich.panel
 import rich.traceback
 from rich.logging import RichHandler
 
 import ikcli.utils.rich
 
-from .algo.cli import cli_algo
-from .namespaces.cli import cli_namespace
+from .algos.cli import cli_algo
+from .hub.cli import cli_hub
+
+# from .namespaces.cli import cli_namespace
 from .net.http import http
-from .organizations.cli import cli_organization
-from .projects.cli import cli_project
+
+# from .organizations.cli import cli_organization
+# from .projects.cli import cli_project
 from .users.core import Account
 
 # Click context settings
-CONTEXT_SETTINGS = dict(help_option_names=["--help", "-h"])
+CONTEXT_SETTINGS = {"help_option_names": ["--help", "-h"]}
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 @click.version_option()
 @click.option(
     "--url",
     envvar="IKOMIA_URL",
-    default="",
+    default="https://scale.ikomia.ai",
     help="Ikomia HUB url.",
 )
-@click.option(
-    "--username",
-    envvar="IKOMIA_USER",
-    help="Ikomia API user name.",
-)
-@click.option(
-    "--password",
-    envvar="IKOMIA_PWD",
-    help="Ikomia API password.",
-)
+# @click.option(
+#    "--token",
+#    envvar="IKOMIA_TOKEN",
+#    help="Ikomia API Token.",
+# )
 @click.option("--debug/--no-debug", default=False)
 @click.pass_context
-def cli_cli(ctx, url, username, password, debug=False):
+# def cli_cli(ctx, url, token, debug=False):
+def cli_cli(ctx, url, debug=False):
     """Ikomia command line interface."""
     # Configure logger
     level = logging.INFO
     if debug:
         level = logging.DEBUG
         rich.traceback.install(show_locals=True, suppress=[click])
     logging.basicConfig(level=level, datefmt="[%X]", handlers=[RichHandler()])
 
     # Setup HTTP request
-    ctx.obj = http(url, username=username, password=password)
+    # ctx.obj = http(url, token=token)
+    ctx.obj = http(url)
+
+
+# @cli_cli.command(name="signup")
+@click.option("--username", prompt="Username")
+@click.option("--email", prompt="Email")
+@click.password_option()
+@click.pass_context
+def cli_signup(ctx, username, email, password):
+    """Signup a new user."""
+    rich.print(f"Signup user {username}")
+    user = Account(ctx.obj).signup(username, email, password)
+    rich.print(f"[green] {user}")
 
 
-# @cli_cli.command(name="register")
-# @click.option("--username", prompt="Username")
-# @click.option("--email", prompt="Email")
-# @click.password_option()
-# @click.pass_context
-# def cli_register(ctx, username, email, password):
-#     """Register a new user."""
-#     rich.print(f"Register user {username}")
-#     account = Account(ctx.obj)
-#     user = account.register(username, email, password)
-#     rich.print(f"[green] {user}")
-#
-#
 # @cli_cli.command(name="login")
-# @click.option("--username", prompt="Username")
-# @click.option(
-#    "--password",
-#    prompt=True,
-#    hide_input=True,
-# )
-# @click.pass_context
-# def cli_login(ctx, username, password):
-#    """Log in user."""
-#    Account(ctx.obj).login(username, password)
+@click.option("--username", prompt="Username")
+@click.option(
+    "--password",
+    prompt=True,
+    hide_input=True,
+)
+@click.option("--token-name", default="Short live token from ikcli", help="Name for token")
+@click.option("--token-ttl", type=int, default=3600, help="Token time to live")
+@click.pass_context
+def cli_login(ctx, username, password, token_name, token_ttl):
+    """Create a new API Token and display it."""
+    try:
+        token = Account(ctx.obj).create_token(username, password, name=token_name, ttl=token_ttl)
+        print(
+            f"# This token will be only visible once and will be valid for next {token_ttl} seconds.\n"
+            f"export IKOMIA_TOKEN={token}"
+        )
+    except ikcli.net.http.exceptions.HTTPBadCodeError as e:
+        if e.code != 401:
+            raise
+        rich.print("[red]Invalid credentials")
+
+
+# @cli_cli.command(name="whoami")
+@click.pass_context
+def cli_whoami(ctx):
+    """Get information about current user."""
+    try:
+        # Get user info
+        me = Account(ctx.obj).me()
+
+        # Get user profile fields
+        profile = list(
+            ikcli.utils.rich.show_api_object_format(me["profile"], ["job", "company", "location", "url", "biography"])
+        )
+
+        # Render
+        ikcli.utils.rich.show(
+            me,
+            f"Logged in as '{me['username']}' on '{ctx.obj.url}'",
+            ["username", "email", "first_name", "last_name"],
+            extra=profile,
+        )
+
+    except ikcli.net.http.exceptions.HTTPBadCodeError as e:
+        if e.code != 401:
+            raise
+        rich.print(f"[orange3]Not logged in on '{ctx.obj.url}'")
 
 
 def cli():
     """
     Call click and catch all Exceptions to display them properly.
 
-    :raises Exception: If debug is enabled and something wrong happen
+    Raises:
+        Exception: If debug is enabled and something wrong happen
     """
     try:
         # Call click
-        cli_cli()
-    except Exception as e:
+        cli_cli()  # pylint: disable=E1120
+    except Exception as e:  # pylint: disable=W0703
         # If debug enable, let exception raise (and rich display traceback)
         if logging.root.level == logging.DEBUG:
             raise
 
         # Otherwise try to display it properly
         ikcli.utils.rich.exception(e)
         sys.exit(1)
 
 
 cli_cli.add_command(cli_algo)
+cli_cli.add_command(cli_hub)
 # cli_cli.add_command(cli_namespace)
 # cli_cli.add_command(cli_organization)
 # cli_cli.add_command(cli_project)
 
 if __name__ == "__main__":
     cli()
```

## ikcli/namespaces/cli.py

```diff
@@ -1,20 +1,19 @@
 """Namespace subcommand cli."""
+import sys
+
 import click
 import rich
 
 import ikcli.utils.rich
+from ikcli.common.cli import role_choice, visibility_choice
+from ikcli.users.core import Users
 
 from .core import Namespaces
 
-# Click choice on organization visibility
-# TODO: move this on core file
-visibility_choice = click.Choice(["PRIVATE", "TEAM"], case_sensitive=False)
-
-
 # A decorator to give Namespaces object to commands
 pass_namespaces = click.make_pass_decorator(Namespaces)
 
 
 @click.group(name="namespace")
 @click.pass_context
 def cli_namespace(ctx):
@@ -31,14 +30,41 @@
     ikcli.utils.rich.table(
         namespaces.list(name=name).limit(limit),
         "Namespaces",
         ["name", "path", "visibility"],
     )
 
 
+@cli_namespace.command(name="show")
+@click.argument("name")
+@pass_namespaces
+def cli_namespace_show(namespaces, name):
+    """Show namespace NAME."""
+    try:
+        namespace = namespaces.get(name=name)
+    except ikcli.net.api.exceptions.ObjectNotFoundException:
+        rich.print(f"[orange3]Unable to find namespace {name}.")
+        sys.exit(1)
+
+    # Get member list
+    extra = None
+    try:
+        members = namespace.members.list()
+        extra = [ikcli.utils.rich.table(members, "Members", ["username", "role", "source"], display=False)]
+    except ikcli.net.http.exceptions.HTTPBadCodeError as e:
+        # Member list doesn't works with organization (due to conflict with 'organization member' command, for now)
+        #  or personal namespaces (because no membership supported)
+        # So if 404, don't bother, display nothing
+        if e.code != 404:
+            raise
+
+    # Display namespace
+    ikcli.utils.rich.show(namespace, "Namespace", ["name", "path", "visibility"], extra=extra)
+
+
 @cli_namespace.command(name="add")
 @click.argument("namespace")
 @click.argument("name")
 @click.option("--visibility", type=visibility_choice, help="Filter organizations by visibility")
 @pass_namespaces
 def cli_namespace_add(namespaces, namespace, name, visibility):
     """Add namespaces NAME to NAMESPACE."""
@@ -52,7 +78,61 @@
 
 @cli_namespace.command(name="delete")
 @click.argument("name")
 @pass_namespaces
 def cli_namespace_delete(namespaces, name):
     """Delete namespace NAME."""
     ikcli.utils.rich.delete(namespaces.get(name=name))
+
+
+#
+#   Members
+#
+@cli_namespace.group(name="member")
+def cli_namespace_member():
+    """Manage namespace members."""
+    pass
+
+
+@cli_namespace_member.command(name="ls")
+@click.argument("namespace_name")
+@click.option("--username", help="Filter namespace members by name")
+@click.option("--role", type=role_choice, help="Filter namespace members by role")
+@pass_namespaces
+def cli_namespace_member_list(namespaces, namespace_name, username, role):
+    """List namespace members."""
+    # Get namespace and members
+    namespace = namespaces.get(name=namespace_name)
+    members = namespace.members.list(username=username, role=role)
+
+    # Display on table
+    ikcli.utils.rich.table(members, "Members", ["username", "role", "source"])
+
+
+@cli_namespace_member.command(name="add")
+@click.argument("namespace_name")
+@click.argument("username")
+@click.argument("role", type=role_choice)
+@pass_namespaces
+def cli_namespace_member_add(namespaces, namespace_name, username, role):
+    """Add namespace members."""
+    # Get namespace and user
+    namespace = namespaces.get(name=namespace_name)
+    user = Users(namespaces.get_http_request()).get(username=username)
+    ikcli.utils.rich.create(
+        f"Add '{username}' as {namespace_name}'s {role}",
+        namespace.members,
+        user=user,
+        role=role,
+    )
+
+
+@cli_namespace_member.command(name="delete")
+@click.argument("namespace_name")
+@click.argument("username")
+@pass_namespaces
+def cli_namespace_member_delete(namespaces, namespace_name, username):
+    """Remove namespace member."""
+    # Get namespace and member
+    namespace = namespaces.get(name=namespace_name)
+    member = namespace.members.get(username=username)
+    ikcli.utils.rich.delete(member)
```

## ikcli/namespaces/core.py

```diff
@@ -1,45 +1,77 @@
 """Namespace API Object."""
 from yarl import URL
 
+from ikcli.algos.core import Algos
+from ikcli.common.core import Members
 from ikcli.net.api import List, Object
 from ikcli.net.http.core import HTTPRequest
 from ikcli.projects.core import Projects
 
 
 class Namespace(Object):
     """Namespace API Object."""
 
     def __repr__(self) -> str:
         """
         Return a representation of Namespace object.
 
-        :return: Namespace object representation
+        Returns:
+            Namespace object representation
         """
         return f"Namespace {self['path']}"
 
     @property
+    def members(self) -> Members:
+        """
+        Return member list.
+
+        Returns:
+            Member list
+        """
+        return Members(self._http, self._url / "members/")
+
+    @property
     def projects(self) -> Projects:
         """
         Return a namespace project list.
 
-        :return: Namespace project list
+        Returns:
+            Namespace project list
         """
         return Projects(self._http, self._url / "projects/")
 
     @property
+    def algos(self) -> Algos:
+        """
+        Return namespace algo list.
+
+        Returns:
+            Namespace algo list
+        """
+        return Algos(self._http, self._url / "algos/")
+
+    @property
     def namespaces(self) -> "Namespace":
         """
         Return sub namespace list.
 
-        :return: Sub namespace list
+        Returns:
+            Sub namespace list
         """
         return Namespaces(self._http, self._url / "namespaces/")
 
 
 class Namespaces(List):
     """Namespace API List."""
 
     def __init__(self, http: HTTPRequest, url: URL = None):
+        """
+        Initialize a new Namespaces object.
+
+        Args:
+            http: A HTTPRequest object to talk with api
+            url: Absolute or relative path to Namespaces
+        """
         if url is None:
             url = URL("/v1/namespaces/")
         super().__init__(http, url, Namespace)
```

## ikcli/net/api/core.py

```diff
@@ -16,78 +16,114 @@
     This can be use as python dict.
     """
 
     def __init__(self, http: HTTPRequest, url: URL, data: dict = None):
         """
         Initialize a new api object.
 
-        :param http: A HTTPRequest object to talk with api
-        :param url: Relative or absolute URL to object
-        :param data: Object data
+        Args:
+            http: A HTTPRequest object to talk with api
+            url: Relative or absolute URL to object
+            data: Object data
         """
         self._http = http
         self._url = url
         if data is None:
             self._data = {}
         else:
             self._data = data
 
+    def get_http_request(self) -> HTTPRequest:
+        """
+        Return internal HTTP request object.
+
+        Returns:
+            Internal HTTPRequest
+        """
+        return self._http
+
     def get(self, key: Any, default: Any = None) -> Optional[Any]:
         """
         Get object item.
 
-        :param key: Item key
-        :param default: Default value if key not found
-        :return: Object item value
+        Args:
+            key: Item key
+            default: Default value if key not found
+
+        Returns:
+            Object item value
         """
         return self._data.get(key, default=default)
 
     def __getitem__(self, key: str):
         """
         Get object item.
 
-        :param key: Item key
-        :return: Object item value
+        Args:
+            key: Item key
+
+        Returns:
+            Object item value
 
         Example:
             name = organisation['name']
         """
         return self._data.get(key)
 
     # TODO: def __missing__(self, key)
     # as in dict, if key is missing, try to load / reload data
     # https://docs.python.org/3/reference/datamodel.html#object.__missing__
 
     def __setitem__(self, key: str, value):
         """
         Set object item value.
 
-        :param key: Object item key
-        :param value: Object item value
+        Args:
+            key: Object item key
+            value: Object item value
         """
         self._data[key] = value
 
     def __contains__(self, key: str) -> bool:
         """
         Return if object contains item.
 
-        :param key: Object item key
-        :return: True if item exists, False otherwise
+        Args:
+            key: Object item key
+
+        Returns:
+            True if item exists, False otherwise
         """
         return key in self._data
 
     def clear(self):
         """Clear object data."""
         self._data.clear()
 
+    def reload(self) -> object:
+        """
+        Reload object data.
+
+        Returns:
+            Self object
+        """
+        self.clear()
+        self._data = self._http.get(self._url)
+        return self
+
+    def update(self):
+        """Update object on remote server."""
+        self._data = self._http.put(self._url, self._data)
+
     def delete(self):
         """
         Delete object on remote server.
 
-        :return: Raw server response
+        Returns:
+            Raw server response
         """
         return self._http.delete(self._url)
 
 
 class List:
     """A list of API objects."""
 
@@ -97,57 +133,78 @@
         url: URL,
         object_class: Type[Object],
         pagination: Type[Pagination] = PageNumberPagination,
     ):
         """
         Initialize a new api object list.
 
-        :param http: A HTTPRequest object to talk with api
-        :param url: Absolute or relative path to list
-        :param object_class: A class to map api object in list
-        :param pagination: A pagination class
+        Args:
+            http: A HTTPRequest object to talk with api
+            url: Absolute or relative path to list
+            object_class: A class to map api object in list
+            pagination: A pagination class
         """
         self._http = http
         self._url = url
         # TODO: remove when code will be clean
         assert isinstance(url, URL)
         self._object_class = object_class
         self._pagination = pagination
 
+    def get_http_request(self) -> HTTPRequest:
+        """
+        Return internal HTTP request object.
+
+        Returns:
+            Internal HTTPRequest
+        """
+        return self._http
+
     def list(self, **kwargs) -> Pagination:
         """
         Return a generator to object list.
 
-        :param kwargs: lookup param
-        :return: A pagination generator
+        Args:
+            kwargs: lookup param
+
+        Returns:
+            A pagination generator
         """
         # Remove 'None' values from kwargs (not supported by yarl as query)
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         return self._pagination(self._http, self._url % kwargs, self._object_class)
 
     def get(self, **kwargs) -> Object:
         """
         Return an object.
 
-        :param kwargs: lookup param
-        :return: An API object
-        :raises ObjectNotFoundException: If no object found
-        :raises NotUniqueObjectException: If more than one object found
+        Args:
+            kwargs: lookup param
+
+        Returns:
+            An API object
+
+        Raises:
+            ObjectNotFoundException: If no object found
+            NotUniqueObjectException: If more than one object found
         """
         pagination = iter(self.list(**kwargs))
         if len(pagination) == 0:
             raise ObjectNotFoundException(self._object_class, **kwargs)
         if len(pagination) > 1:
             raise NotUniqueObjectException(self._object_class, pagination, **kwargs)
         return pagination.get(0)
 
     def create(self, **kwargs) -> Object:
         """
         Create a new object in list.
 
-        :param kwargs: Object data
-        :return: New API Object
+        Args:
+            **kwargs: Object data
+
+        Returns:
+            New API Object
         """
         # Remove 'None' values from kwargs
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         data = self._http.post(self._url, data=kwargs)
         return self._object_class(self._http, URL(data["url"]), data=data)
```

## ikcli/net/api/exceptions.py

```diff
@@ -4,30 +4,36 @@
 class ObjectNotFoundException(Exception):
     """Raised when no api object found."""
 
     def __init__(self, object_class, **kwargs):
         """
         Initialize a new ObjectNotFoundException.
 
-        :param object_class: API Objet class.
-        :param kwargs: lookup param
+        Args:
+            object_class: API Objet class.
+            kwargs: lookup param
         """
+        # Remove kwargs with None value to avoid get user confused
+        kwargs = {k: v for k, v in kwargs.items() if v is not None}
         super().__init__(f"{object_class.__name__} that match '{kwargs}' not found.")
         self.object_class = object_class
         self.kwargs = kwargs
 
 
 class NotUniqueObjectException(Exception):
     """Raised when more than one object found."""
 
     def __init__(self, object_class, pagination, **kwargs):
         """
         Initialize a new NotUniqueObjectException.
 
-        :param object_class: API Objet class.
-        :param pagination: A pagination object that contains all items found
-        :param kwargs: lookup param
+        Args:
+            object_class: API Objet class.
+            pagination: A pagination object that contains all items found
+            kwargs: lookup param
         """
+        # Remove kwargs with None value to avoid get user confused
+        kwargs = {k: v for k, v in kwargs.items() if v is not None}
         super().__init__(f"{len(pagination)} {object_class.__name__} that match '{kwargs}' were found.")
         self.object_class = object_class
         self.pagination = pagination
         self.kwargs = kwargs
```

## ikcli/net/api/pagination.py

```diff
@@ -9,127 +9,187 @@
 class Pagination(ABC):
     """Abstract class to manage pagination."""
 
     def __init__(self, http: HTTPRequest, url: URL, object_class):
         """
         Initialize a new pagination class.
 
-        :param http: HTTP Request object
-        :param url: Absolute or relative URL
-        :param object_class: Object API class
+        Args:
+            http: HTTP Request object
+            url: Absolute or relative URL
+            object_class: Object API class
         """
         self._http = http
         self._url = url
         self._object_class = object_class
         self._data = None
         self._index = 0
 
     def __iter__(self):
-        """Initialize iterator."""
+        """
+        Initialize iterator.
+
+        Returns:
+            Itself as iterator
+        """
         self._data = self._http.get(self._url)
         self._index = 0
         return self
 
     @abstractmethod
     def __next__(self):
         """
         Return next item.
 
-        :raises StopIteration: When loop is over
+        Returns:
+            Next item
+
+        Raises:
+            StopIteration: When loop is over
         """
 
     @abstractmethod
-    def __len__(self):
-        """Return paginator total length."""
+    def __len__(self) -> int:
+        """
+        Return paginator total length.
+
+        Returns:
+            Paginator length
+        """
 
     @abstractmethod
     def get(self, index: int):
         """
         Get object at index, for internal purpose only.
 
-        :param index: Index
-        :return: API Object instance
+        Args:
+            index: Index
+
+        Returns:
+            API Object instance
         """
 
     def limit(self, limit: int):
         """
         Limit pagination results.
 
-        :param limit: How many objects return at max
-        :return: A LimitPagination generator.
+        Args:
+            limit: How many objects return at max
+
+        Returns:
+            A LimitPagination generator.
         """
         # First check if iterator was started
         assert self._data is None, "Can't set limit if paginator was already started"
         return LimitedPagination(self, limit)
 
 
 class PageNumberPagination(Pagination):
     """Manage django PageNumberPagination."""
 
-    def __len__(self):
+    def __len__(self) -> int:
+        """
+        Return paginator total length.
+
+        Returns:
+            Paginator length
+        """
         return self._data["count"]
 
     def __next__(self):
+        """
+        Return next item.
+
+        Returns:
+            Next item
+
+        Raises:
+            StopIteration: When loop is over
+        """
         # If reach end of page, load next one
         if self._index >= len(self._data["results"]):
             if self._data["next"] is None:
                 raise StopIteration()
             self._data = self._http.get(URL(self._data["next"]))
             self._index = 0
 
         # Get object, increment index and return
         next_object = self.get(self._index)
         self._index += 1
         return next_object
 
     def get(self, index):
+        """
+        Get object at index, for internal purpose only.
+
+        Args:
+            index: Index
+
+        Returns:
+            API Object instance
+        """
         data = self._data["results"][index]
         return self._object_class(self._http, URL(data["url"]), data=data)
 
 
 class LimitedPagination:
     """Limited pagination returned results."""
 
     def __init__(self, pagination: Pagination, limit: int):
         """
         Initialize a new limited pagination.
 
-        :param pagination: A pagination object to limit
-        :param limit: How many results to return
+        Args:
+            pagination: A pagination object to limit
+            limit: How many results to return
         """
         self._pagination = pagination
         self._limit = limit
         self._index = 0
 
     def __len__(self):
-        """Return pagination total length."""
+        """
+        Return pagination total length.
+
+        Returns:
+            Pagination length
+        """
         return len(self._pagination)
 
     def __iter__(self):
-        """Initialize iterator."""
+        """
+        Initialize iterator.
+
+        Returns:
+            Itself as iterator
+        """
         iter(self._pagination)
         self._index = 0
         return self
 
     def __next__(self):
         """
         Return next api object.
 
-        :return: Next api object
-        :raises StopIterator: If reach limit of reach end of pagination
+        Returns:
+            Next api object
+
+        Raises:
+            StopIteration: If reach limit of reach end of pagination
         """
         # Check if reach limit
         if self._index >= self._limit:
             raise StopIteration()
 
         # Get next object, increment index and return
         next_object = next(self._pagination)
         self._index += 1
         return next_object
 
     def remaining(self) -> int:
         """
         Return how many object remain on pagination.
 
-        :return: How many objects remaining.
+        Returns:
+            How many objects remaining.
         """
         return len(self._pagination) - self._index
```

## ikcli/net/http/__init__.py

```diff
@@ -1,27 +1,29 @@
 """Make HTTP interactions easier."""
 import functools
 
 from yarl import URL
 
-from .auth import HTTPBasicAuth
+from .auth import HTTPTokenAuth
 from .core import HTTPRequest
 
 
 @functools.lru_cache(maxsize=None)
-def http(url: str, username: str = None, password: str = None) -> HTTPRequest:
+def http(url: str, token: str = None) -> HTTPRequest:
     """
     Return driver to talk with ikscale API.
 
-    :param url: Ikomia scale api url
-    :param username: Username for authentication
-    :param password: Password for authentication
-    :return: A fully loaded HTTPRequest object.
+    Args:
+        url: Ikomia scale api url
+        token: API token for authentication
+
+    Returns:
+        A fully loaded HTTPRequest object.
     """
     # Parse url from str as yarl URL
     parsed_url = URL(url)
 
     # Get auth
-    auth = HTTPBasicAuth(parsed_url, username, password)
+    auth = HTTPTokenAuth(parsed_url, token)
 
     # Return HTTPRequest object
     return HTTPRequest(parsed_url, auth=auth)
```

## ikcli/net/http/auth.py

```diff
@@ -8,29 +8,103 @@
 class HTTPBasicAuth(requests.auth.AuthBase):
     """Basic HTTP authentication."""
 
     def __init__(self, url: URL, username: Optional[str], password: Optional[str]):
         """
         Initialize authentication.
 
-        :param url: URL to authenticate
-        :param username: A user name
-        :param password: A password
+        Args:
+            url: URL to authenticate
+            username: A username
+            password: A password
         """
         super().__init__()
         self.url = url
         self.username = username
         self.password = password
 
     def __call__(self, r: requests.PreparedRequest) -> requests.PreparedRequest:
         """
         Modify a request to set authentication headers.
 
-        :param r: a Prepared Request
-        :return: An authenticated and prepared request
+        Args:
+            r: a Prepared Request
+
+        Returns:
+            An authenticated and prepared request
         """
         if self.username is None or self.password is None:
             return r
 
         # Add header
         r.headers["Authorization"] = requests.auth._basic_auth_str(self.username, self.password)
         return r
+
+
+class HTTPTokenAuth(requests.auth.AuthBase):
+    """Token in HTTP Header authentication."""
+
+    def __init__(self, url: URL, token: str, schema: str = "Token"):
+        """
+        Initialize authentication.
+
+        Args:
+            url: URL to authenticate
+            token: Token to authenticate
+            schema: Authentication schema
+        """
+        super().__init__()
+        self.url = url
+        if token is None:
+            self.token = None
+        else:
+            self.token = f"{schema} {token}"
+
+    def __call__(self, r: requests.PreparedRequest) -> requests.PreparedRequest:
+        """
+        Modify a request to set authentication headers.
+
+        Args:
+            r: a Prepared Request
+
+        Returns:
+            An authenticated and prepared request
+        """
+        if self.token is None:
+            return r
+
+        # Add header
+        r.headers["Authorization"] = self.token
+        return r
+
+
+class HTTPAuthContextManager:
+    """Switch authentication in a context."""
+
+    def __init__(self, http_request, auth: requests.auth.AuthBase):
+        """
+        Initialize a new http auth context manager.
+
+        Args:
+            http_request: An HTTPRequest object
+            auth: A new auth to using within context
+        """
+        self.http_request = http_request
+        self.auth = auth
+        self.actual_auth = None
+
+    def __enter__(self):
+        """Enter to the context by replacing current authentication method with new one."""
+        assert self.actual_auth is None, f"{self.__class__.__name__} was already initialized"
+
+        self.actual_auth = self.http_request.auth
+        self.http_request.auth = self.auth
+
+    def __exit__(self, *exc):
+        """
+        Exit from context by restoring actual authentication.
+
+        Args:
+            *exc: Information related to stack trace
+        """
+        self.http_request.auth = self.actual_auth
+        self.actual_auth = None
```

## ikcli/net/http/core.py

```diff
@@ -1,12 +1,15 @@
 """Core HTTP object."""
+import io
 import logging
+from pathlib import Path
 
 import requests
 import requests.auth
+import requests_toolbelt.multipart
 from yarl import URL
 
 from .exceptions import HTTPBadCodeError
 from .serializer import JsonSerializer, Serializer, load
 
 logger = logging.getLogger(__name__)
 
@@ -18,180 +21,281 @@
 class HTTPRequest:
     """An object to make requests usage easier."""
 
     def __init__(self, url: URL, auth=None, timeout: int = DEFAULT_TIMEOUT, serializer: Serializer = None):
         """
         Initialize HTTPRequest object.
 
-        :param url: IKScale service url
-        :param auth: Authentication class
-        :param timeout: HTTP request timeout
-        :param serializer: A Serializer to format data before request. If None, use JsonSerializer
+        Args:
+            url: IKScale service url
+            auth: Authentication class
+            timeout: HTTP request timeout
+            serializer: A Serializer to format data before request. If None, use JsonSerializer
         """
-        # TODO: remove when code will be clean
-        assert isinstance(url, URL)
         self.url = url
         self.timeout = timeout
         self.connect_timeout = 5
         self.auth = auth
         self.session = requests.Session()
         self.headers = {"User-Agent": "IkomiaCli"}
         if serializer is None:
             self.serializer = JsonSerializer()
         else:
             self.serializer = serializer
+        self._observers = []
+
+    def append_observer(self, observer: object):
+        """
+        Append observer to observer list.
+
+        Args:
+            observer: Observer to append
+        """
+        self._observers.append(observer)
+
+    def remove_observer(self, observer: object):
+        """
+        Remove observer from observer list.
+
+        Args:
+            observer: Observer to remove
+        """
+        self._observers.remove(observer)
+
+    def _download_monitor(self, total: int, completed: int):
+        """
+        Call observers to notify download progress.
+
+        Args:
+            total: Total bytes to read
+            completed: Bytes already read
+        """
+        for observer in self._observers:
+            observer.downloading(total, completed)
+
+    def _upload_monitor(self, monitor: requests_toolbelt.multipart.encoder.MultipartEncoderMonitor):
+        """
+        Call observers to notify upload progress.
+
+        Args:
+            monitor: A MultipartEncoderMonitor
+        """
+        for observer in self._observers:
+            observer.uploading(monitor.len, monitor.bytes_read)
 
     def request(self, method: str, path: URL, query: dict = None, data=None, files: dict = None):
         """
         Send an HTTP request.
 
-        :param method: HTTP method
-        :param path: Query path as URL
-        :param query: URL query params
-        :param data: Data to send
-        :param files: A dict that contains (filename, fh) pair
-        :return: A tuple with raw content and headers
-        :raises HTTPBadCodeError: If server return a code <200 or >299
-        :raises requests.exceptions.ReadTimeout: If request timeout
+        Args:
+            method: HTTP method
+            path: Query path as URL
+            query: URL query params
+            data: Data to send
+            files: A dict that contains (filename, fh) pair
+
+        Returns:
+            A tuple with raw content and headers
+
+        Raises:
+            HTTPBadCodeError: If server return a code <200 or >299
+            requests.exceptions.ReadTimeout: If request timeout
         """
         # Prepare headers
         headers = self.headers.copy()
 
-        # TODO: remove when code will be clean
-        assert isinstance(path, URL)
-
         # Check if url is absolute
         if path.is_absolute():
             # Assert then address same origin
             assert path.origin() == self.url, f"Given URL '{path}' is not relative with '{self.url}'"
             url = path
         else:
             url = self.url.join(path)
 
-        if data is not None:
+        # If files are given, use requests_toolbelt.multipart.encoder to monitor upload
+        if files is not None:
+            # As requests_toolbelt.multipart.encoder doesn't support list or dict as value,
+            #   convert data and set content-type
+            # https://github.com/requests/toolbelt/issues/205
+            fields = []
+            if data is not None:
+                for k, v in data.items():
+                    if isinstance(v, (list, dict)):
+                        fields.append((k, (None, self.serializer.dump(v), format(self.serializer.mime))))
+                    else:
+                        fields.append((k, v))
+
+            # Append files
+            for key in files:
+                filename = files[key] if isinstance(files[key], Path) else Path(files[key])
+                fields.append(
+                    (
+                        key,
+                        (filename.name, filename.open("rb"), "application/octet-stream"),
+                    )
+                )
+
+            # Create MultipartEncoderMonitor as request data
+            m_encoder = requests_toolbelt.multipart.encoder.MultipartEncoder(fields=fields)
+            data = requests_toolbelt.multipart.encoder.MultipartEncoderMonitor(m_encoder, callback=self._upload_monitor)
+            headers["Content-Type"] = data.content_type
+
+        elif data is not None:
+            # Otherwise dump data on right format
             data = self.serializer.dump(data)
             headers["Content-Type"] = format(self.serializer.mime)
 
         # Create request object
         request = requests.Request(
             method=method,
             url=url,
             headers=headers,
             params=query,
             data=data,
-            files=files,
             auth=self.auth,
         )
         prepared_request = self.session.prepare_request(request)
 
         # Produce some debug logs
         logger.debug("Will %s '%s'", prepared_request.method, prepared_request.url)
         if prepared_request.headers:
             logger.debug(" with headers : %s", prepared_request.headers)
         if prepared_request.body:
-            if len(prepared_request.body) > 2048:
-                logger.debug(" with body    : .... too long to be dumped ! ...")
+            if isinstance(prepared_request.body, requests_toolbelt.multipart.encoder.MultipartEncoderMonitor):
+                logger.debug(" with body    : %s", prepared_request.body.encoder)
             else:
-                logger.debug(" with body    : %s", prepared_request.body)
+                if len(prepared_request.body) > 2048:
+                    logger.debug(" with body    : .... too long to be dumped ! ...")
+                else:
+                    logger.debug(" with body    : %s", prepared_request.body)
 
         # Get response
         try:
             response = self.session.send(
-                prepared_request, timeout=(self.connect_timeout, self.timeout), allow_redirects=False
+                prepared_request, stream=True, timeout=(self.connect_timeout, self.timeout), allow_redirects=False
             )
         except requests.exceptions.ReadTimeout:
             logger.warning(
                 "'%s' '%s' timeout after %d seconds", prepared_request.method, prepared_request.url, self.timeout
             )
             # TODO: raise custom exception ?
             raise
 
+        # Read stream and make observable progress
+        content_bytes = io.BytesIO()
+        content_bytes_total = int(response.headers["Content-Length"]) if "Content-Length" in response.headers else None
+        content_bytes_done = 0
+        for chunk in response.iter_content(chunk_size=requests.models.CONTENT_CHUNK_SIZE):
+            content_bytes.write(chunk)
+            content_bytes_done += len(chunk)
+            self._download_monitor(content_bytes_total, content_bytes_done)
+
+        # Get content
+        content = content_bytes.getvalue()
+
+        # Log response
         logger.debug("Response code : %d", response.status_code)
         logger.debug(" with headers : %s", response.headers)
         if ("Content-Length" in response.headers and int(response.headers["Content-Length"]) > 10240) or len(
-            response.content
+            content
         ) > 2048:
             logger.debug(" with content    : .... too long to be dumped ! ...")
         else:
-            logger.debug(" with content    : %s", response.content)
+            logger.debug(" with content    : %s", content)
 
         # 200 = return response and meta
         # TODO = response.raise_for_status()
         if response.status_code >= 200 and response.status_code <= 299:
-            return (response.content, response.headers)
+            return (content, response.headers)
 
         # Otherwise raise error
-        raise HTTPBadCodeError(
-            prepared_request.url, response.status_code, headers=response.headers, content=response.content
-        )
+        raise HTTPBadCodeError(prepared_request.url, response.status_code, headers=response.headers, content=content)
 
     def head(self, path: URL, query: dict = None):
         """
         HEAD HTTP Request.
 
-        :param path: request path
-        :param query: Query param as dict
-        :return: Python data
+        Args:
+            path: request path
+            query: Query param as dict
+
+        Returns:
+            Python data
         """
         (content, metadata) = self.request("HEAD", path, query=query)
         return load(content, metadata=metadata)
 
     def get(self, path: URL, query: dict = None):
         """
         GET HTTP Request.
 
-        :param path: request path
-        :param query: Query param as dict
-        :return: Python data
+        Args:
+            path: request path
+            query: Query param as dict
+
+        Returns:
+            Python data
         """
         (content, metadata) = self.request("GET", path, query=query)
         return load(content, metadata=metadata)
 
     def post(self, path: URL, data, files: dict = None, query: dict = None):
         """
         POST HTTP Request.
 
-        :param path: request path
-        :param data: Payload data
-        :param files: A dict that contains info about files to send
-        :param query: Query param as dict
-        :return: Python data
+        Args:
+            path: request path
+            data: Payload data
+            files: A dict that contains info about files to send
+            query: Query param as dict
+
+        Returns:
+            Python data
         """
         (content, metadata) = self.request("POST", path, query=query, data=data, files=files)
         return load(content, metadata=metadata)
 
     def put(self, path: URL, data, files: dict = None, query: dict = None):
         """
         PUT HTTP Request.
 
-        :param path: request path
-        :param data: Payload data
-        :param files: A dict that contains info about files to send
-        :param query: Query param as dict
-        :return: Python data
+        Args:
+            path: request path
+            data: Payload data
+            files: A dict that contains info about files to send
+            query: Query param as dict
+
+        Returns:
+            Python data
         """
         (content, metadata) = self.request("PUT", path, query=query, data=data, files=files)
         return load(content, metadata=metadata)
 
     def patch(self, path: URL, data, files: dict = None, query: dict = None):
         """
         PATCH HTTP Request.
 
-        :param path: request path
-        :param data: Payload data
-        :param files: A dict that contains info about files to send
-        :param query: Query param as dict
-        :return: Python data
+        Args:
+            path: request path
+            data: Payload data
+            files: A dict that contains info about files to send
+            query: Query param as dict
+
+        Returns:
+            Python data
         """
         (content, metadata) = self.request("PATCH", path, query=query, data=data, files=files)
         return load(content, metadata=metadata)
 
     def delete(self, path: URL, query: dict = None):
         """
         DELETE HTTP Request.
 
-        :param path: request path
-        :param query: Query param as dict
-        :return: Python data
+        Args:
+            path: request path
+            query: Query param as dict
+
+        Returns:
+            Python data
         """
         (content, metadata) = self.request("DELETE", path, query=query)
         return load(content, metadata=metadata)
```

## ikcli/net/http/exceptions.py

```diff
@@ -9,25 +9,27 @@
 class HTTPBadCodeError(Exception):
     """Raised when request status code <200 or >299."""
 
     def __init__(self, url: yarl.URL, code: int, headers: requests.structures.CaseInsensitiveDict = None, content=None):
         """
         Init a new HTTP error.
 
-        :param url: URL
-        :param code: HTTP code
-        :param headers: Response header
-        :param content: Response content
+        Args:
+            url: URL
+            code: HTTP code
+            headers: Response header
+            content: Response content
         """
         super().__init__(f"Bad return code {code} on '{url}'")
         self.url = url
         self.code = code
         self.headers = headers
         self.content = content
 
     def data(self):
         """
         Return parsed content as valid python data.
 
-        :return: Parsed content as python data
+        Returns:
+            Parsed content as python data
         """
         return load(self.content, self.headers)
```

## ikcli/net/http/serializer.py

```diff
@@ -8,45 +8,52 @@
 class Mime:
     """A mime type : https://en.wikipedia.org/wiki/Media_type."""
 
     def __init__(self, mime_type: str, subtype: str, suffix: str = None, parameters: dict = None):
         """
         Initialize a new mime type.
 
-        :param mime_type: A mime type
-        :param subtype: Mime sub type
-        :param suffix: Mime suffix
-        :param parameters: Mime parameters
+        Args:
+            mime_type: A mime type
+            subtype: Mime sub type
+            suffix: Mime suffix
+            parameters: Mime parameters
         """
         self.type = mime_type
         self.subtype = subtype
         self.suffix = suffix
         self.parameters = parameters
 
     def __repr__(self) -> str:
         """
         Mime type representation.
 
-        :return: Mime type representation
+        Returns:
+            Mime type representation
         """
         message = f"{self.type}/{self.subtype}"
         if self.suffix is not None:
             message += f"+{self.suffix}"
         if self.parameters is not None:
             message += "; ".join([f"{k}={v}" for k, v in sorted(self.parameters.items())])
         return message
 
     @classmethod
     def parse(cls, mime: str) -> "Mime":
         """
         Parse textual mime and return Mime object.
 
-        :param mime: A textual mime type
-        :return: A Mime object
-        :raises ValueError: If can't parse mime
+        Args:
+            mime: A textual mime type
+
+        Returns:
+            A Mime object
+
+        Raises:
+            ValueError: If can't parse mime
         """
         # Parse mime
         m = re.match(r"^(?P<type>[a-z]+)\/(?P<subtype>[a-z-\.]+)(?P<suffix>\+[a-z\.]+)?(; (?P<parameters>.+))?", mime)
         if m is None:
             raise ValueError(f"Can't parse mime type '{mime}'")
 
         # Split parameter to dict
@@ -64,35 +71,42 @@
     """Convert data from or to python data."""
 
     @abstractmethod
     def __init__(self, mime: Mime):
         """
         Initialize a new Serializer.
 
-        :param mime: Supported Mime
+        Args:
+            mime: Supported Mime
         """
         self.mime = mime
 
     @abstractmethod
     def load(self, data):
         """
         Convert to python data.
 
-        :param data: Native data
-        :return: Python data
+        Args:
+            data: Native data
+
+        Returns:
+            Python data
         """
         pass
 
     @abstractmethod
     def dump(self, data):
         """
         Convert from python data.
 
-        :param data: Python data
-        :return: Native data
+        Args:
+            data: Python data
+
+        Returns:
+            Native data
         """
         pass
 
 
 class JsonSerializer(Serializer):
     """Serialize json data."""
 
@@ -133,14 +147,16 @@
         return data
 
     def dump(self, data):
         return data
 
 
 class FormURLEncoded(Serializer):
+    """Serialize Form urlencoded data."""
+
     def __init__(self):
         super().__init__(Mime("application", "x-www-form-urlencoded"))
 
     def load(self, data):
         if isinstance(data, bytes):
             return data.decode("UTF-8")
         return data
@@ -150,17 +166,22 @@
 
 
 @functools.lru_cache(maxsize=None)
 def get(name: str) -> Serializer:
     """
     Get a serializer from mime type or subtype.
 
-    :param name: A mime type or subtype name
-    :return: Serializer
-    :raises TypeError: If data type not supported.
+    Args:
+        name: A mime type or subtype name
+
+    Returns:
+        Serializer
+
+    Raises:
+        TypeError: If data type not supported.
     """
     if name == "json":
         return JsonSerializer()
     if name == "text":
         return TextSerializer()
     if name == "x-python":
         return PythonSerializer()
@@ -168,18 +189,23 @@
     raise TypeError(f"Can't find a serializer to process '{name}' type")
 
 
 def load(data, metadata=None):
     """
     Convert heterogeneous data to python.
 
-    :param data: HTTPRequest data
-    :param metadata: HTTPRequest metadata
-    :return: Python data
-    :raises TypeError: If raw data can't be converted to python
+    Args:
+        data: HTTPRequest data
+        metadata: HTTPRequest metadata
+
+    Returns:
+        Python data
+
+    Raises:
+        TypeError: If raw data can't be converted to python
     """
     # If no data, return python serializer
     if data is None:
         return get("x-python").load(data)
 
     # Extract mime type if available
     if metadata is not None and "Content-Type" in metadata:
```

## ikcli/organizations/cli.py

```diff
@@ -1,22 +1,22 @@
 """Organization subcommand cli."""
+import sys
+
 import click
 import rich
 
 import ikcli.utils.rich
+from ikcli.common.cli import role_choice
 from ikcli.users.core import Users
 
 from .core import Organizations
 
 # Click choice on organization visibility
 visibility_choice = click.Choice(["PUBLIC", "TEAM"], case_sensitive=False)
 
-# Click choice on member roles
-role_choice = click.Choice(["OWNER", "MANAGER", "MEMBER", "PARTNER"], case_sensitive=False)
-
 # A decorator to give Organizations object to commands
 pass_organizations = click.make_pass_decorator(Organizations)
 
 
 @click.group(name="organization")
 @click.pass_context
 def cli_organization(ctx):
@@ -30,15 +30,15 @@
 @click.option("--limit", type=int, default=20, help="Specify how many rows to display")
 @pass_organizations
 def cli_organization_list(organizations, name, visibility, limit):
     """List organizations."""
     ikcli.utils.rich.table(
         organizations.list(name=name, visibility=visibility).limit(limit),
         "Organizations",
-        ["name", "visibility"],
+        ["name", "description", "visibility", "location", "homepage"],
     )
 
 
 @cli_organization.command(name="add")
 @click.option("--visibility", type=visibility_choice, help="Organization visibility")
 @click.argument("name")
 @pass_organizations
@@ -48,15 +48,28 @@
 
 
 @cli_organization.command(name="show")
 @click.argument("name")
 @pass_organizations
 def cli_organization_show(organizations, name):
     """Show organization NAME."""
-    rich.print_json(data=organizations.get(name=name)._data)
+    try:
+        organization = organizations.get(name=name)
+    except ikcli.net.api.exceptions.ObjectNotFoundException:
+        rich.print(f"[orange3]Unable to find organization {name}.")
+        sys.exit(1)
+
+    # Get member list
+    members = organization.members.list()
+    extra = [ikcli.utils.rich.table(members, "Members", ["username", "role"], display=False)]
+
+    # Display organization
+    ikcli.utils.rich.show(
+        organization, "Organization", ["name", "description", "visibility", "location", "homepage"], extra=extra
+    )
 
 
 @cli_organization.command(name="delete")
 @click.argument("name")
 @pass_organizations
 def cli_organization_delete(organizations, name):
     """Delete organization NAME."""
@@ -74,43 +87,44 @@
 
 @cli_organization_member.command(name="ls")
 @click.argument("organization_name")
 @click.option("--username", help="Filter organization members by name")
 @click.option("--role", type=role_choice, help="Filter organization members by role")
 @pass_organizations
 def cli_organization_member_list(organizations, organization_name, username, role):
-    """List organizaton members."""
+    """List organization members."""
     # Get organization and members
     organization = organizations.get(name=organization_name)
     members = organization.members.list(username=username, role=role)
 
     # Display on table
     ikcli.utils.rich.table(members, "Members", ["username", "role"])
 
 
 @cli_organization_member.command(name="add")
 @click.argument("organization_name")
 @click.argument("username")
 @click.argument("role", type=role_choice)
 @pass_organizations
 def cli_organization_member_add(organizations, organization_name, username, role):
-    """Add organizaton members."""
+    """Add organization members."""
     # Get organization and user
     organization = organizations.get(name=organization_name)
-    user = Users(organizations._http).get(username=username)
+    user = Users(organizations.get_http_request()).get(username=username)
     ikcli.utils.rich.create(
         f"Add '{username}' as {organization_name}'s {role}",
         organization.members,
         user=user,
         role=role,
     )
 
 
 @cli_organization_member.command(name="delete")
 @click.argument("organization_name")
 @click.argument("username")
 @pass_organizations
 def cli_organization_member_delete(organizations, organization_name, username):
-    """Remove organizaton member."""
+    """Remove organization member."""
     # Get organization and member
     organization = organizations.get(name=organization_name)
-    ikcli.utils.rich.delete(organization.members.get(username=username))
+    member = organization.members.get(username=username)
+    ikcli.utils.rich.delete(member)
```

## ikcli/organizations/core.py

```diff
@@ -1,56 +1,45 @@
 """Organization API Objects."""
 from yarl import URL
 
+from ikcli.common.core import Members
 from ikcli.net.api import List, Object
 from ikcli.net.http.core import HTTPRequest
-from ikcli.users.core import User
-
-
-class Member(Object):
-    """Organization Member API Object."""
-
-    def __repr__(self) -> str:
-        """
-        Return a representation of Member object.
-
-        :return: Member object representation
-        """
-        return f"{self['username']} as {self['role']}"
-
-
-class Members(List):
-    """Member API List."""
-
-    def __init__(self, http: HTTPRequest, url: URL):
-        super().__init__(http, url, Member)
-
-    def create(self, user: User = None, **kwargs) -> Member:
-        return super().create(user=user["url"], **kwargs)
 
 
 class Organization(Object):
     """Organization API Object."""
 
     def __repr__(self) -> str:
         """
         Return a representation of Organization object.
 
-        :return: Organization object representation
+        Returns:
+            Organization object representation
         """
         return f"Organization {self['name']}"
 
     @property
     def members(self) -> Members:
         """
-        Return organization member list.
+        Return member list.
 
-        :return: Member list
+        Returns:
+            Member list
         """
         return Members(self._http, self._url / "members/")
 
 
 class Organizations(List):
     """Organization API List."""
 
-    def __init__(self, http: HTTPRequest):
-        super().__init__(http, URL("/v1/organizations/"), Organization)
+    def __init__(self, http: HTTPRequest, url: URL = None):
+        """
+        Initialize a new Organizations object.
+
+        Args:
+            http: A HTTPRequest object to talk with api
+            url: Absolute or relative path to Organizations
+        """
+        if url is None:
+            url = URL("/v1/organizations/")
+        super().__init__(http, url, Organization)
```

## ikcli/projects/archive.py

```diff
@@ -16,33 +16,33 @@
 class Archive:
     """Manager archive to send to ikomia service to deploy a workflow."""
 
     def __init__(self, filename: Path):
         """
         Initialize a new Archive.
 
-        :param filename: workflow filename to process
+        Args:
+            filename: workflow filename to process
         """
         with open(filename, "rt", encoding="utf-8") as fh:
             self.workflow = json.load(fh)
         self.temporary_directory = None
-        self.zipfh = None
 
     def prepare(self) -> BinaryIO:
         """
         Prepare zip archive to send to service.
 
-        :return: A zip file handler
+        Returns:
+            A zip file name
         """
         # Sanity check
         assert self.temporary_directory is None
-        assert self.zipfh is None
 
         # Create temporary directory
-        self.temporary_directory = tempfile.TemporaryDirectory(prefix="ikcli-workflow-")
+        self.temporary_directory = tempfile.TemporaryDirectory(prefix="ikcli-workflow-")  # pylint: disable=R1732
 
         # Create temporary working directory
         directory = Path(self.temporary_directory.name)
         working_directory = directory / "workdir"
         working_directory.mkdir()
 
         # Create workflow file
@@ -56,65 +56,69 @@
         zip_filename = directory / "archive.zip"
         with zipfile.ZipFile(zip_filename, "w", zipfile.ZIP_DEFLATED) as zipf:
             for root, _, files in os.walk(working_directory):
                 for filename in files:
                     filepath = Path(root, filename)
                     zipf.write(filepath, filepath.relative_to(working_directory))
 
-        # Return zip file handler
-        self.zipfh = open(zip_filename, "rb")
-        return self.zipfh
+        # Return zip file name
+        return zip_filename
 
     def __enter__(self):
         """
         When used with ContextManager, prepare zip to send to service.
 
-        :return: A zip file handler
+        Returns:
+            A zip file handler
         """
         return self.prepare()
 
     def cleanup(self):
         """Clean temporary working files and directories."""
         # Sanity check
         assert self.temporary_directory is not None
 
-        # Close zip file handler
-        if self.zipfh is not None:
-            self.zipfh.close()
-            self.zipfh = None
-
         # Clean temporary directory
         self.temporary_directory.cleanup()
         self.temporary_directory = None
 
-    def __exit__(self, exc_type, exc_value, traceback):
-        """Cleanup when exit to ContextManager."""
+    def __exit__(self, *exc):
+        """
+        Cleanup when exit to ContextManager.
+
+        Args:
+            *exc: Information related to stack trace
+        """
         self.cleanup()
 
     def _add_plugins(self, directory: Path):
         """
         Parse task list and embed plugins if needed.
 
-        :param directory: Directory to copy plugins
+        Args:
+            directory: Directory to copy plugins
+
+        Raises:
+            ValueError: when plugin URL is not supported
         """
-        logger.debug("Check to embeded plugins")
+        logger.debug("Check to embedded plugins")
 
         # For each task, check if we have to embed plugin
         for task in self.workflow["tasks"]:
             data = task["task_data"]
 
             # Extract URL
             if "url" not in data:
-                logger.debug("Task {data['name']} plugin is internal")
+                logger.debug("Task %s plugin is internal", data["name"])
             else:
                 url = URL(task["task_data"]["url"])
-                logger.debug("Task {data['name']} plugin is located at {url}")
+                logger.debug("Task %s plugin is located at %s", data["name"], url)
 
                 if url.scheme == "file":
                     # If URL is file scheme, copy
                     dst = directory / data["name"]
-                    logger.debug("Copy plugin from '{url.path}' to '{dst}'")
+                    logger.debug("Copy plugin from '%s' to '%s'", url.path, dst)
                     shutil.copytree(url.path, dst, ignore=shutil.ignore_patterns(".git"))
                     # Update url
                     data["url"] = "file://" + data["name"]
                 else:
-                    raise ValueError("Plugin url scheme '{url}' is not supported yet")
+                    raise ValueError(f"Plugin url scheme '{url}' is not supported yet")
```

## ikcli/projects/cli.py

```diff
@@ -1,35 +1,39 @@
 """Project sub command cli."""
 import io
 import os
+import sys
 import tempfile
+import time
 from pathlib import Path
 
 import click
 import rich
 import rich.console
 import rich.json
 from PIL import Image
 
 import ikcli.utils.rich
+from ikcli.common.cli import role_choice, visibility_choice
 from ikcli.namespaces.core import Namespaces
+from ikcli.users.core import Users
 
 from .core import Projects
 
-# Click choice on project visibilities
-visibility_choice = click.Choice(["PUBLIC", "TEAM", "PRIVATE"], case_sensitive=False)
-
 # Click choice on cloud providers
-provider_choice = click.Choice(["AWS"], case_sensitive=False)
+provider_choice = click.Choice(["AWS", "SCALEWAY_VIA_SCALEDYNAMICS"], case_sensitive=False)
 
 # Click choice on cloud provider region
-provider_region_choice = click.Choice(["FRANCE"], case_sensitive=False)
+provider_region_choice = click.Choice(["FRANCE", "GERMANY", "IRELAND"], case_sensitive=False)
 
 # Click choice on deployment flavour
-provider_flavour_choice = click.Choice(["SERVERLESS"], case_sensitive=False)
+provider_flavour_choice = click.Choice(["SERVERLESS", "CLUSTER", "GPU"], case_sensitive=False)
+
+# Click choice on deployment size
+provider_size_choice = click.Choice(["S", "M", "L", "XL"], case_sensitive=False)
 
 # A decorator to give Projects object to commands
 pass_projects = click.make_pass_decorator(Projects)
 
 
 @click.group(name="project")
 @click.pass_context
@@ -56,26 +60,45 @@
 @click.option("--visibility", type=visibility_choice, help="Project visibility")
 @click.argument("namespace")
 @click.argument("name")
 @pass_projects
 def cli_project_add(projects, namespace, name, description, visibility):
     """Add project NAME on NAMESPACE."""
     # Get namespace
-    namespace = Namespaces(projects._http).get(name=namespace)
+    namespace = Namespaces(projects.get_http_request()).get(name=namespace)
 
     # Add project
     ikcli.utils.rich.create(
         f"Add Project '{name}' to {namespace}",
         namespace.projects,
         name=name,
         description=description,
         visibility=visibility,
     )
 
 
+@cli_project.command(name="show")
+@click.argument("name")
+@pass_projects
+def cli_project_show(projects, name):
+    """Show project NAME."""
+    try:
+        project = projects.get(name=name)
+    except ikcli.net.api.exceptions.ObjectNotFoundException:
+        rich.print(f"[orange3]Unable to find project {name}.")
+        sys.exit(1)
+
+    # Get member list
+    members = project.members.list()
+    extra = [ikcli.utils.rich.table(members, "Members", ["username", "role", "source"], display=False)]
+
+    # Display project
+    ikcli.utils.rich.show(project, "Project", ["name", "description", "visibility"], extra=extra)
+
+
 @cli_project.command(name="delete")
 @click.argument("name")
 @pass_projects
 def cli_project_delete(projects, name):
     """Delete project NAME."""
     ikcli.utils.rich.delete(projects.get(name=name))
 
@@ -94,17 +117,77 @@
     NAME                Project name.
     WORKFLOW_FILENAME   Path to workflow json file.
     """
     # Get project
     project = projects.get(name=name)
 
     # Push workflow
-    ikcli.utils.rich.create(f"Push workflow to {project['name']}", project.workflows, workflow_filename)
+    console = rich.console.Console()
+    with ikcli.utils.rich.HTTPTransferProgress("Workflow", project.get_http_request(), download=False, upload=True):
+        workflow = project.workflows.create(workflow_filename)
+    console.print(f"[green] {workflow}")
+
+
+#
+#   Members
+#
+@cli_project.group(name="member")
+def cli_project_member():
+    """Manage project members."""
+    pass
 
 
+@cli_project_member.command(name="ls")
+@click.argument("project_name")
+@click.option("--username", help="Filter project members by name")
+@click.option("--role", type=role_choice, help="Filter project members by role")
+@pass_projects
+def cli_project_member_list(projects, project_name, username, role):
+    """List project members."""
+    # Get project and members
+    project = projects.get(name=project_name)
+    members = project.members.list(username=username, role=role)
+
+    # Display on table
+    ikcli.utils.rich.table(members, "Members", ["username", "role", "source"])
+
+
+@cli_project_member.command(name="add")
+@click.argument("project_name")
+@click.argument("username")
+@click.argument("role", type=role_choice)
+@pass_projects
+def cli_project_member_add(projects, project_name, username, role):
+    """Add project members."""
+    # Get project and user
+    project = projects.get(name=project_name)
+    user = Users(projects.get_http_request()).get(username=username)
+    ikcli.utils.rich.create(
+        f"Add '{username}' as {project_name}'s {role}",
+        project.members,
+        user=user,
+        role=role,
+    )
+
+
+@cli_project_member.command(name="delete")
+@click.argument("project_name")
+@click.argument("username")
+@pass_projects
+def cli_project_member_delete(projects, project_name, username):
+    """Remove project member."""
+    # Get project and member
+    project = projects.get(name=project_name)
+    member = project.members.get(username=username)
+    ikcli.utils.rich.delete(member)
+
+
+#
+#   Workflow
+#
 @cli_project.group(name="workflow")
 def cli_workflow():
     """Manage workflows."""
     pass
 
 
 @cli_workflow.command(name="ls")
@@ -117,15 +200,15 @@
     # Get project
     project = projects.get(name=project_name)
 
     # Display workflow
     ikcli.utils.rich.table(
         project.workflows.list(name=name).limit(limit),
         "Workflows",
-        ["name", "description"],
+        ["name", "description", "tag"],
     )
 
 
 @cli_workflow.command(name="show")
 @click.argument("project_name")
 @click.argument("workflow_name")
 @pass_projects
@@ -141,25 +224,26 @@
 
 @cli_workflow.command(name="deploy")
 @click.argument("project_name")
 @click.argument("workflow_name")
 @click.argument("provider", type=provider_choice)
 @click.argument("region", type=provider_region_choice)
 @click.argument("flavour", type=provider_flavour_choice)
+@click.option("--size", type=provider_size_choice, default="M")
 @pass_projects
-def cli_workflow_deploy(projects, project_name, workflow_name, provider, region, flavour):
+def cli_workflow_deploy(projects, project_name, workflow_name, provider, region, flavour, size):
     """Deploy workflow."""
     # Get project and workflow
     project = projects.get(name=project_name)
     workflow = project.workflows.get(name=workflow_name)
 
     # Create deployment
     console = rich.console.Console()
     with console.status(f"[cyan]Deploying {workflow} to {provider} {flavour} {region} ...", spinner="earth"):
-        deployment = workflow.deployments.create(provider=provider, flavour=flavour, region=region)
+        deployment = workflow.deployments.create(provider=provider, flavour=flavour, region=region, size=size)
     console.print(f"\U0001F30D  [bold green]{deployment}")
 
 
 @cli_workflow.command(name="delete")
 @click.argument("project_name")
 @click.argument("workflow_name")
 @pass_projects
@@ -168,14 +252,17 @@
     # Get project
     project = projects.get(name=project_name)
 
     # Delete workflow
     ikcli.utils.rich.delete(project.workflows.get(name=workflow_name))
 
 
+#
+#   Deployment
+#
 @cli_project.group(name="deployment")
 def cli_deployment():
     """Manage deployments."""
     pass
 
 
 @cli_deployment.command(name="ls")
@@ -188,32 +275,83 @@
     project = projects.get(name=project_name)
     workflow = project.workflows.get(name=workflow_name)
 
     # List deployments
     ikcli.utils.rich.table(
         workflow.deployments.list(),
         "Deployments",
-        ["provider", "region", "flavour", "status", "endpoint"],
+        ["provider", "region", "flavour", "size", "tag", "status", "endpoint"],
+    )
+
+
+@cli_deployment.command(name="update")
+@click.argument("project_name")
+@click.argument("workflow_name")
+@click.option("--provider", type=provider_choice, help="Cloud provider")
+@click.option("--region", type=provider_region_choice, help="Cloud provider region")
+@click.option("--flavour", type=provider_flavour_choice, help="Deployment flavour")
+@click.option("--size", type=provider_size_choice, default=None)
+@pass_projects
+def cli_deployment_update(projects, project_name, workflow_name, provider, region, flavour, size):
+    """Update deployment against workflow or size."""
+    console = rich.console.Console()
+
+    # Get project and workflow
+    project = projects.get(name=project_name)
+    workflow = project.workflows.get(name=workflow_name)
+
+    # Get deployments to update
+    deployments = [
+        deployment
+        for deployment in workflow.deployments.list(provider=provider, region=region, flavour=flavour)
+        if (deployment["tag"] != workflow["tag"])
+        or (size is not None and deployment["size"] != size)
+        or deployment["status"] == "ERROR"
+    ]
+    if len(deployments) == 0:
+        console.print("[orange3]Nothing to update")
+        return
+
+    # Display and confirm
+    ikcli.utils.rich.table(
+        deployments,
+        "Will update these deployments",
+        ["provider", "region", "flavour", "size", "tag", "status", "endpoint"],
     )
 
+    if not rich.prompt.Confirm.ask("Continue to update ?"):
+        console.print("[orange3]Aborted by user")
+        return
+
+    # Update each one
+    for deployment in deployments:
+        with console.status(f"[cyan]Updating {deployment} ..."):
+            if size is not None:
+                deployment["size"] = size
+            deployment.update()
+        console.print("[green]Done")
+
 
 @cli_deployment.command(name="run")
 @click.argument("project_name")
 @click.argument("workflow_name")
 @click.argument(
     "image",
     type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True, path_type=Path),
 )
 @click.option("--provider", type=provider_choice, help="Cloud provider")
 @click.option("--region", type=provider_region_choice, help="Cloud provider region")
 @click.option("--flavour", type=provider_flavour_choice, help="Deployment flavour")
 @click.option("--task", help="Workflow task to query. Will prompt user if not given")
 @click.option("--output-index", type=click.INT, multiple=True, help="Output index to display (default = all)")
+@click.option("--polling", type=click.INT, help="time in seconds between 2 poll when wait for response", default=5)
 @pass_projects
-def cli_deployment_run(projects, project_name, workflow_name, image, provider, region, flavour, task, output_index):
+def cli_deployment_run(
+    projects, project_name, workflow_name, image, provider, region, flavour, task, output_index, polling
+):
     """Call deployment endpoint on image."""
     # Get project, workflow and deployment
     project = projects.get(name=project_name)
     workflow = project.workflows.get(name=workflow_name)
     deployment = workflow.deployments.get(provider=provider, region=region, flavour=flavour)
 
     # If task wasn't specified, ask to user to choose one
@@ -223,24 +361,28 @@
             task = next(iter(task_options))
         else:
             task = ikcli.utils.rich.menu("Choose a task", task_options)
 
     # Query endpoint
     console = rich.console.Console()
     with console.status(f"[cyan]Querying {deployment} ..."):
-        outputs = deployment.run(task, image, output_indexes=output_index)
-    console.print("[green] Done")
+        # Get endpoint HTTPRequest object and query
+        start = time.time()
+        outputs = list(
+            deployment.get_endpoint_http_request().run(task, image, output_indexes=output_index, polling=polling)
+        )
+        duration = int(time.time() - start)
 
     # Display outputs
     for counter, output in enumerate(outputs):
-        title = f"{output['type']} ({counter})" if len(output_index) == 0 else output["type"]
-        data = output["data"]
+        (typ, data) = next(iter(output.items()))
+        title = f"{typ} ({counter})" if len(output_index) == 0 else typ
 
         # If type is image, save it and display
-        if output["type"] == "IMAGE" or output["type"] == "IMAGE_BINARY":
+        if typ in ("image", "image_binary"):
             image = Image.open(io.BytesIO(data))
             fd, path = tempfile.mkstemp(
                 prefix=f"ikcli - {project_name} - {workflow_name} (", suffix=f") {title}.{image.format}"
             )
             with os.fdopen(fd, "w") as fh:
                 image.save(fh, image.format)
             ikcli.utils.rich.show_image(path, title=title)
@@ -252,14 +394,17 @@
                 rich.padding.Padding(rich.json.JSON.from_data(data=data), (1, 1)),
                 title=title,
                 width=80,
                 border_style="bold green",
             )
         )
 
+    # Print duration
+    console.print(f"[green] Done in {duration} seconds")
+
 
 @cli_deployment.command(name="delete")
 @click.argument("project_name")
 @click.argument("workflow_name")
 @click.option("--provider", type=provider_choice, help="Cloud provider")
 @click.option("--region", type=provider_region_choice, help="Cloud provider region")
 @click.option("--flavour", type=provider_flavour_choice, help="Deployment flavour")
```

## ikcli/projects/core.py

```diff
@@ -1,132 +1,161 @@
 """Project API Object."""
-import base64
+import re
 from pathlib import Path
 
 from yarl import URL
 
+from ikcli.common.core import Members
 from ikcli.net.api import List, Object
 from ikcli.net.http.core import HTTPRequest
 
 from .archive import Archive
+from .http import DeploymentHTTPJWTAuth, DeploymentHTTPRequest
 
 
 class Deployment(Object):
     """Deployment API Object."""
 
     def __repr__(self) -> str:
         """
         Return a representation of Deployment object.
 
-        :return: Deployment object representation
+        Returns:
+            Deployment object representation
         """
         return f"Deployment {self['provider']} {self['region']} {self['flavour']} {self['endpoint']}"
 
-    def run(self, task: str, image: str, output_indexes: list = None) -> list:
+    def get_endpoint_http_request(self) -> DeploymentHTTPRequest:
         """
-        Call deployment endpoint.
+        Return a HTTPRequest object configured to easily call deployment endpoint.
 
-        :param task: Task name to call
-        :param image: Image filename to give
-        :param output_indexes: List of output index to retreive. None = All
-        :return: A list of output. Each one is a dict that contains 'type' and 'data'.
-        """
-        # Load image and encode to b64
-        with open(image, "rb") as fh:
-            b64_image = base64.b64encode(fh.read()).decode("UTF-8")
-
-        # Craft data
-        if output_indexes is None or len(output_indexes) == 0:
-            outputs = [{"task_name": task, "task_index": 0}]
-        else:
-            outputs = [{"task_name": task, "task_index": 0, "output_index": index} for index in output_indexes]
-        data = {
-            "inputs": [{"image": b64_image}],
-            "outputs": outputs,
-            "parameters": [],
-        }
-
-        # Query endpoint
-        outputs = HTTPRequest(URL(self["endpoint"]), timeout=180).put(URL("/run"), data)
-        for output in outputs:
-            # Convert b64 to binary if needed
-            if output["type"] == "IMAGE" or output["type"] == "IMAGE_BINARY":
-                output["data"] = base64.b64decode(output["data"]["image"])
+        Returns:
+            A fully configured HTTPRequest object
 
-        # Return outputs
-        return outputs
+        Raises:
+            ValueError: when can't extract project url from this deployment url
+        """
+        # Extract project url from deployment url
+        m = re.match(r"^(?P<project_url>.*projects\/[0-9a-f-]+\/)", format(self._url))
+        if m is None:
+            raise ValueError(f"Can't extract project URL from '{self._url}'")
+        project_url = URL(m.group("project_url"))
+
+        # Get endpoint authenticator
+        auth = DeploymentHTTPJWTAuth(self._http, project_url)
+
+        # Get deployment endpoint HTTP request
+        return DeploymentHTTPRequest(URL(self["endpoint"]), auth=auth, timeout=180)
 
 
 class Deployments(List):
     """Deployment API List."""
 
     def __init__(self, http: HTTPRequest, url: URL):
+        """
+        Initialize a new Deployments object.
+
+        Args:
+            http: A HTTPRequest object to talk with api
+            url: Absolute or relative path to Deployments
+        """
         super().__init__(http, url, Deployment)
 
 
 class Workflow(Object):
     """Workflow API Object."""
 
     def __repr__(self) -> str:
         """
         Return a representation of Workflow object.
 
-        :return: Workflow object representation
+        Returns:
+            Workflow object representation
         """
         return f"Workflow {self['name']}"
 
     @property
     def deployments(self) -> Deployments:
         """
         Return workflow deployment list.
 
-        :return: workflow deployment list
+        Returns:
+            workflow deployment list
         """
         return Deployments(self._http, self._url / "deployments/")
 
 
 class Workflows(List):
     """Workflow API List."""
 
     def __init__(self, http: HTTPRequest, url: URL):
+        """
+        Initialize a new Workflows object.
+
+        Args:
+            http: A HTTPRequest object to talk with api
+            url: Absolute or relative path to Workflows
+        """
         super().__init__(http, url, Workflow)
 
     def create(self, filename: Path) -> Workflow:
         """
         Create a new workflow from filename.
 
-        :param filename: Workflow json file name
-        :return: A new workflow
+        Args:
+            filename: Workflow json file name
+
+        Returns:
+            A new workflow
         """
         with Archive(filename) as zfh:
             data = self._http.post(self._url, None, files={"archive": zfh})
             return Workflow(self._http, URL(data["url"]), data=data)
 
 
 class Project(Object):
     """Project API Object."""
 
     def __repr__(self) -> str:
         """
         Return a representation of object.
 
-        :return:  object representation
+        Returns:
+            Object representation
         """
         return f"Project {self['name']}"
 
     @property
+    def members(self) -> Members:
+        """
+        Return member list.
+
+        Returns:
+            Member list
+        """
+        return Members(self._http, self._url / "members/")
+
+    @property
     def workflows(self) -> Workflows:
         """
         Return project workflow list.
 
-        :return: Project workflow list
+        Returns:
+            Project workflow list
         """
         return Workflows(self._http, self._url / "workflows/")
 
 
 class Projects(List):
     """Project API List."""
 
     def __init__(self, http, url: URL = None):
+        """
+        Initialize a new Projects object.
+
+        Args:
+            http: A HTTPRequest object to talk with api
+            url: Absolute or relative path to Projects
+        """
         if url is None:
             url = URL("/v1/projects/")
         super().__init__(http, url, Project)
```

## ikcli/users/core.py

```diff
@@ -1,71 +1,95 @@
 """User API object."""
-import random
-import string
-
 from yarl import URL
 
 from ikcli.net.api import List, Object
+from ikcli.net.http.auth import HTTPAuthContextManager, HTTPBasicAuth
 from ikcli.net.http.core import HTTPRequest
 
 
 class User(Object):
     """User API Object."""
 
     def __repr__(self) -> str:
         """
         Return a representation of User object.
 
-        :return: User object representation
+        Returns:
+            User object representation
         """
         return f"User {self['username']}"
 
 
 class Users(List):
     """User API List."""
 
-    def __init__(self, http: HTTPRequest):
-        super().__init__(http, URL("/v1/users/"), User)
+    def __init__(self, http: HTTPRequest, url: URL = None):
+        """
+        Initialize a new Users object.
+
+        Args:
+            http: A HTTPRequest object to talk with api
+            url: Absolute or relative path to Users
+        """
+        if url is None:
+            url = URL("/v1/users/")
+        super().__init__(http, url, User)
 
 
 class Account(Object):
     """Manage personal account."""
 
     def __init__(self, http: HTTPRequest):
-        super().__init__(http, URL("/v1/accounts/"))
+        """
+        Initialize a new Account object.
+
+        Args:
+            http: A HTTPRequest object to talk with api
+        """
+        super().__init__(http, URL("/v1/users/"))
 
-    def login(self, username: str, password: str):
+    def create_token(self, username: str, password: str, name: str = "Token from ikcli", ttl: int = 3600) -> str:
         """
         Log user to platform.
 
-        :param username: User name
-        :param password: User password
+        Args:
+            username: Username
+            password: User password
+            name: Token name
+            ttl: Token time to live
+
+        Returns:
+            A clear and valid token
         """
-        # Fake endpoint until authentication works for real
-        letters = string.ascii_uppercase + string.digits
-        token = "".join(random.choice(letters) for i in range(29))
-        print(f"export IKCLI_TOKEN='IKT{token}'")
-
-    def logout(self):
-        """Log out user."""
-        self._http.post(self._url / "logout/")
-
-    def register(self, username, email, password, password2=None) -> User:
-        """
-        Register a new user.
-
-        :param username: User name
-        :param email: User email
-        :param password: User password
-        :param password2: User password verification
-        :return: Newly created user
+        with HTTPAuthContextManager(self._http, HTTPBasicAuth(self._http.url, username, password)):
+            response = self._http.post(self._url / "me/tokens/", data={"name": name, "ttl": ttl})
+        return response["clear_token"]
+
+    def me(self) -> User:
+        """
+        Return logged user.
+
+        Returns:
+            Logged user
+        """
+        url = self._url / "me/"
+        return User(self._http, url, data=self._http.get(url))
+
+    def signup(self, username, email, password) -> User:
+        """
+        Signup a new user.
+
+        Args:
+            username: Username
+            email: User email
+            password: User password
+
+        Returns:
+            Newly created user
         """
-        if password2 is None:
-            password2 = password
         data = {
             "username": username,
             "email": email,
             "password": password,
-            "password2": password2,
         }
-        response = self._http.post(self._url / "register/", data)
+        response = self._http.post(URL("/v1/accounts/signup/"), data)
         return User(self._http, URL(response["url"]), data=response)
```

## ikcli/utils/rich.py

```diff
@@ -1,62 +1,103 @@
 """Some shortcuts to display rich interface on ikcli."""
 from typing import List
 
 import rich
 import rich.align
 import rich.console
+import rich.progress
 import rich.prompt
 import rich.table
 from PIL import ImageShow
 
 import ikcli.net.api
+import ikcli.net.http.core
 import ikcli.net.http.exceptions
+import ikcli.net.http.progress
 from ikcli.net.api.pagination import LimitedPagination, Pagination
 
 
-def table(pagination: Pagination, title: str, columns: List[str]):
+def table_cell_format(value) -> str:
     """
-    Display API object in a table.
+    Pretty format for table cell.
 
-    :param pagination: Pagination object
-    :param title: Table title
-    :param columns: Column name to display
+    Args:
+        value: A celle value
+
+    Returns:
+        Pretty formatted value
+    """
+    if value is None:
+        return "-"
+
+    if isinstance(value, list):
+        return ",".join(value)
+
+    if isinstance(value, str):
+        return value
+
+    if isinstance(value, dict):
+        if "name" in value:
+            return value["name"]
+
+    return format(value)
+
+
+def table(pagination: Pagination, title: str, columns: List[str], display: bool = True) -> rich.table.Table:
+    """
+    Craft (and display) API object in a table.
+
+    Args:
+        pagination: Pagination object
+        title: Table title
+        columns: Column name to display
+        display: True if must be display, False otherwise
+
+    Returns:
+        Table
     """
     # Define table
     rtable = rich.table.Table()
     for column in columns:
-        rtable.add_column(column.title(), justify="right")
+        rtable.add_column(column.replace("_", " ").title(), justify="right")
 
-    # Add row per organization
+    # Add row per object
     for row in pagination:
-        args = [row[column] for column in columns]
+        args = [table_cell_format(row[column]) for column in columns]
         rtable.add_row(*args)
 
     # If it remains object in pagination, display it
     if isinstance(pagination, LimitedPagination) and pagination.remaining() > 0:
         rtable.add_section()
         rtable.add_row(f"[bold] ... and {pagination.remaining()} remaining")
 
     # Craft title
     rtable.title = f"{title.title()} ({len(pagination)})"
 
-    # Print table
-    rich.print(rtable)
+    # Display if needed
+    if display:
+        rich.print(rtable)
+
+    # Return table
+    return rtable
 
 
 def menu(title: str, options: dict, prompt: str = "Please choose an option", default=None, none: bool = False):
     """
     Display a menu and ask to user to choose an entry.
 
-    :param title: A menu title
-    :param options: Dict that contains a key to return if chosen and a string to display
-    :param prompt: Prompt to display
-    :param default: A default value
-    :param none: Add a 'None of them' entry to meny
-    :return: Selected option key
+    Args:
+        title: A menu title
+        options: Dict that contains a key to return if chosen and a string to display
+        prompt: Prompt to display
+        default: A default value
+        none: Add a 'None of them' entry to meny
+
+    Returns:
+        Selected option key
     """
     # Craft choice list
     choices = sorted(options, key=options.get)
     prompt_choices = [format(i + 1) for i in range(0, len(choices))]
     default_choice = None
 
     # Define beaufiful padding according to options length
@@ -91,64 +132,133 @@
 
     # Return value
     return choices[index - 1]
 
 
 def create(title: str, api_list: ikcli.net.api.List, *args, **kwargs) -> ikcli.net.api.Object:
     """
-    Display spinners and infos about object creation.
+    Display spinners and info about object creation.
 
-    :param title: A title to display behind spinner
-    :param api_list: An API list object
-    :param args: Args to create object
-    :param kwargs: Kwargs to create object
-    :return: A newly created object
+    Args:
+        title: A title to display behind spinner
+        api_list: An API list object
+        args: Args to create object
+        kwargs: Kwargs to create object
+
+    Returns:
+        A newly created object
     """
     console = rich.console.Console()
     with console.status(f"[cyan]{title} ..."):
         api_object = api_list.create(*args, **kwargs)
     console.print(f"[green] {api_object}")
     return api_object
 
 
 def delete(api_object: ikcli.net.api.Object):
     """
     Prompt for object deletion.
 
-    :param api_object: API Object to delete
+    Args:
+        api_object: API Object to delete
     """
     console = rich.console.Console()
     if not rich.prompt.Confirm.ask(f"Do you really want to delete [red]'{api_object}'[/red] ?"):
         console.print("[orange3]Aborted by user")
         return
 
     with console.status(f"[cyan]Deleting {api_object} ..."):
         api_object.delete()
     console.print(f"[orange3]{api_object.__class__.__name__} deleted")
 
 
+def show_api_object_format(api_object: ikcli.net.api.Object, keys: List[str]) -> List[str]:
+    """
+    Format an API Object and return a list of str usable by show functions.
+
+    Args:
+        api_object: An API Object to format
+        keys: Key list name to show
+
+    Yields:
+        lines of str for each key
+    """
+    # For each key
+    for key in keys:
+
+        # Get value and format it, according to type
+        value = api_object[key]
+        if value is None:
+            value = "-"
+        elif isinstance(value, list):
+            value = ",".join(value)
+
+        if key in ["biography", "description"]:
+            value = f"\n {value}"
+
+        # Format key to get a fancy result
+        key = key.replace("_", " ").title()
+
+        # Yield line
+        yield f"[b]{key}[/b]: {value}"
+
+
+def show(api_object: ikcli.net.api.Object, title: str, keys: List, extra: List = None):
+    """
+    Display an API Object.
+
+    Args:
+        api_object: API Object to show
+        title: A title for rich Panel
+        keys: A list or object keys to show
+        extra: A list of extra things to display. Can be str or rich element.
+    """
+    # Format object
+    lines = list(show_api_object_format(api_object, keys))
+
+    # Append extra display if given
+    if extra is None:
+        extra = []
+    else:
+        lines.append("")
+
+    # Render panel
+    rich.print(
+        rich.panel.Panel(
+            rich.padding.Padding(
+                rich.console.Group(*lines, *extra),
+                (1, 1),
+            ),
+            title=title,
+            width=120,
+            border_style="bold white",
+        )
+    )
+
+
 def exception(e: Exception):
     """
     Try to properly display exception.
 
-    :param e: Exception to display
+    Args:
+        e: Exception to display
     """
     # Process some well known exceptions
     if isinstance(e, ikcli.net.http.exceptions.HTTPBadCodeError):
         title = e.__class__.__name__
         lines = []
         data = e.data()
         if e.code == 401:
             lines.append(
-                "\U0001F449 If you want to avoid be prompted for credentials,"
-                " may you have to define username and password as follow:"
+                "\U0001F449 Your API token is not set or expired.\n"
+                "May you have to call [red]ikcli login[/red] again or export token as follow:"
             )
             lines.append(
                 rich.padding.Padding(
-                    "$> export IKOMIA_USER='my-user-name'\n$> export IKOMIA_PWD='4-v3ry-s3cr3t-p4ssw0rd!'",
+                    "$> export IKOMIA_TOKEN='MyV4ryS3cr3tT0k3n'",
                     (1, 2),
                     style="green on grey11",
                     expand=False,
                 ),
             )
         elif isinstance(data, str):
             lines.append(f"\U0001F449 {data}")
@@ -164,25 +274,34 @@
                 lines.append("")
 
             # Remove last line return
             lines.pop()
     elif isinstance(e, ikcli.net.api.exceptions.ObjectNotFoundException):
         title = f"{e.object_class.__name__} not found"
         lines = [f"\U0001F449 {e.object_class.__name__} that match :"]
-        lines += [f"  - {k}: '{v}'" for k, v in e.kwargs.items()]
+        if len(e.kwargs) > 0:
+            lines += [f"  - {k}: '{v}'" for k, v in e.kwargs.items()]
+        else:
+            lines += ["    *nothing precise*"]
         lines.append("  was not found.")
     elif isinstance(e, ikcli.net.api.exceptions.NotUniqueObjectException):
         title = f"Not unique {e.object_class.__name__} found"
         lines = [f"\U0001F449 {len(e.pagination)} {e.object_class.__name__}(s) that match :"]
-        lines += [f"  - {k}: '{v}'" for k, v in e.kwargs.items()]
-        lines.append("  were found.")
+        if len(e.kwargs) > 0:
+            lines += [f"  - {k}: '{v}'" for k, v in e.kwargs.items()]
+        else:
+            lines += ["    *nothing precise*"]
+        lines.append("  were found :")
+        lines += [f"  - {o}" for o in e.pagination]
     else:
         # Common case exception
         title = e.__class__.__name__
         lines = ["\U0001F449 " + str(arg) for arg in e.args]
+        if hasattr(e, "__notes__"):  # Officially added to 3.11, but some code part already use it
+            lines += [""] + e.__notes__
 
     # Finally display
     rich.print(
         rich.panel.Panel(
             rich.padding.Padding(rich.console.Group(*lines), (1, 1), style="white"),
             title=title,
             width=80,
@@ -191,40 +310,92 @@
     )
 
 
 def show_image(path: str, title: str = None, **options) -> bool:
     """
     Use PIL ImageShow to display existing image without convert nor temporary save it.
 
-    :param path: A path to image to display
-    :param title: A title to give to image display (not well supported)
-    :param **options: Other options to give to ImageShow
-    :return: True if image was displayed, False otherwise
+    Args:
+        path: A path to image to display
+        title: A title to give to image display (not well supported)
+        **options: Other options to give to ImageShow
+
+    Returns:
+        True if image was displayed, False otherwise
     """
-    for viewer in ImageShow._viewers:
+    # Inspired from PIL core as there's no way to display image without converting it first
+    for viewer in ImageShow._viewers:  # pylint: disable=W0212
         if viewer.show_file(path, title=title, **options):
             return True
     return False
 
 
-def auth_panel_info():
-    lines = []
-    lines.append(
-        "\U0001F449 If you want to avoid being prompted for your credentials,"
-        " you may define username and password as follow:"
-    )
-    lines.append(
-        rich.padding.Padding(
-            "$> export IKOMIA_USER='my-user-name'\n$> export IKOMIA_PWD='4-v3ry-s3cr3t-p4ssw0rd!'",
-            (1, 2),
-            style="green on grey11",
-            expand=False,
-        ),
-    )
-    rich.print(
-        rich.panel.Panel(
-            rich.padding.Padding(rich.console.Group(*lines), (1, 1), style="white"),
-            title="Authentication information",
-            width=80,
-            border_style="cyan",
+class HTTPTransferProgress(ikcli.net.http.progress.ProgressObserver):
+    """A rich progress bar that display http transfer."""
+
+    def __init__(
+        self, title: str, http_request: ikcli.net.http.core.HTTPRequest, download: bool = True, upload: bool = False
+    ):
+        """
+        Initialize a new progress bar transfer monitor.
+
+        Args:
+            title: Progress bar title
+            http_request: HTTPRequest object to monitor.
+            download: Display download progress bar.
+            upload: Display upload progress bar.
+        """
+        super().__init__(http_request)
+        self.progress = rich.progress.Progress(
+            "{task.description} " + title,
+            rich.progress.BarColumn(),
+            rich.progress.DownloadColumn(),
+            rich.progress.TransferSpeedColumn(),
+            rich.progress.TimeRemainingColumn(),
         )
-    )
+
+        self.progress_upload_task = None
+        self.progress_download_task = None
+
+        if upload:
+            self.progress_upload_task = self.progress.add_task("[cyan]Uploading", total=None)
+        if download:
+            self.progress_download_task = self.progress.add_task("[magenta]Downloading", total=None)
+
+    def __enter__(self):
+        """Enable progress bar."""
+        super().__enter__()
+        self.progress.__enter__()
+
+    def __exit__(self, *args):
+        """
+        Disable progress bar.
+
+        Args:
+            *args: stuff given to ContextManager exit function.
+        """
+        super().__exit__(*args)
+        self.progress.__exit__(*args)
+
+    def downloading(self, total: int, completed: int):
+        """
+        Make download progress bar updated.
+
+        Args:
+            total: Total bytes to download
+            completed: Already downloaded bytes
+        """
+        if self.progress_download_task is None:
+            return
+        self.progress.update(self.progress_download_task, total=total, completed=completed)
+
+    def uploading(self, total: int, completed: int):
+        """
+        Make upload progress bar updated.
+
+        Args:
+            total: Total bytes to upload
+            completed: Already uploaded bytes
+        """
+        if self.progress_upload_task is None:
+            return
+        self.progress.update(self.progress_upload_task, total=total, completed=completed)
```

## Comparing `ikcli/algo/templates/process.pyt` & `ikcli/algos/templates/{{cookiecutter.plugin_dir}}/{{cookiecutter.algo_name}}_process.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,120 @@
+{%- if cookiecutter.base_class == "CWorkflowTask" %}
+{%-   set base_class_fqdn = "core.CWorkflowTask" %}
+{%- else %}
+{%-   set base_class_fqdn = "dataprocess." + cookiecutter.base_class %}
+{%- endif %}
 import copy
+
 from ikomia import core, dataprocess
 
 
 # --------------------
 # - Class to handle the process parameters
 # - Inherits core.CWorkflowTaskParam from Ikomia API
 # --------------------
-class {{ PluginClassName }}Param(core.CWorkflowTaskParam):
+class {{ cookiecutter.class_name }}Param(core.CWorkflowTaskParam):
 
     def __init__(self):
         core.CWorkflowTaskParam.__init__(self)
         # Place default value initialization here
         # Example : self.windowSize = 25
 
-    def setParamMap(self, param_map):
+    def set_values(self, params):
         # Set parameters values from Ikomia application
         # Parameters values are stored as string and accessible like a python dict
-        # Example : self.windowSize = int(param_map["windowSize"])
+        # Example : self.windowSize = int(params["windowSize"])
         pass
 
-    def getParamMap(self):
+    def get_values(self):
         # Send parameters values to Ikomia application
         # Create the specific dict structure (string container)
-        param_map = core.ParamMap()
-        # Example : paramMap["windowSize"] = str(self.windowSize)
-        return param_map
+        params = {}
+        # Example : params["windowSize"] = str(self.windowSize)
+        return params
 
 
 # --------------------
 # - Class which implements the process
 # - Inherits core.CWorkflowTask or derived from Ikomia API
 # --------------------
-class {{ PluginClassName }}({{ ProcessBaseClass }}):
+class {{ cookiecutter.class_name }}({{ base_class_fqdn }}):
 
     def __init__(self, name, param):
-        {{ ProcessBaseClass }}.__init__(self, name)
+        {{ base_class_fqdn }}.__init__(self, name)
         # Add input/output of the process here
-        # Example :  self.addInput(dataprocess.CImageIO())
-        #           self.addOutput(dataprocess.CImageIO())
+        # Example :  self.add_input(dataprocess.CImageIO())
+        #           self.add_output(dataprocess.CImageIO())
 
         # Create parameters class
         if param is None:
-            self.setParam({{ PluginClassName }}Param())
+            self.set_param_object({{ cookiecutter.class_name }}Param())
         else:
-            self.setParam(copy.deepcopy(param))
+            self.set_param_object(copy.deepcopy(param))
 
-    def getProgressSteps(self):
+    def get_progress_steps(self):
         # Function returning the number of progress steps for this process
         # This is handled by the main progress bar of Ikomia application
         return 1
 
     def run(self):
         # Core function of your process
-        # Call beginTaskRun for initialization
-        self.beginTaskRun()
+        # Call begin_task_run() for initialization
+        self.begin_task_run()
 
         # Examples :
         # Get input :
-        # input = self.getInput(indexOfInput)
+        # task_input = self.get_input(index_of_input)
 
         # Get output :
-        # output = self.getOutput(indexOfOutput)
+        # task_output = self.get_output(index_of_output)
 
         # Get parameters :
-        # param = self.getParam()
+        # param = self.get_param_object()
 
         # Get image from input/output (numpy array):
-        # srcImage = input.getImage()
+        # src_image = task_input.get_image()
 
         # Call to the process main routine
-        # dstImage = ...
+        # dst_image = ...
 
         # Set image of input/output (numpy array):
-        # output.setImage(dstImage)
+        # task_output.set_image(dst_image)
 
         # Step progress bar:
-        self.emitStepProgress()
+        self.emit_step_progress()
 
-        # Call endTaskRun to finalize process
-        self.endTaskRun()
+        # Call end_task_run() to finalize process
+        self.end_task_run()
 
 
 # --------------------
 # - Factory class to build process object
 # - Inherits dataprocess.CTaskFactory from Ikomia API
 # --------------------
-class {{ PluginClassName }}Factory(dataprocess.CTaskFactory):
+class {{ cookiecutter.class_name }}Factory(dataprocess.CTaskFactory):
 
     def __init__(self):
         dataprocess.CTaskFactory.__init__(self)
         # Set process information as string here
-        self.info.name = "{{ PluginName }}"
-        self.info.shortDescription = "your short description"
+        self.info.name = "{{ cookiecutter.algo_name }}"
+        self.info.short_description = "your short description"
         self.info.description = "your description"
         # relative path -> as displayed in Ikomia Studio process tree
         self.info.path = "Plugins/Python"
         self.info.version = "1.0.0"
-        # self.info.iconPath = "your path to a specific icon"
+        # self.info.icon_path = "your path to a specific icon"
         self.info.authors = "algorithm author"
         self.info.article = "title of associated research article"
         self.info.journal = "publication journal"
         self.info.year = 2022
         self.info.license = "MIT License"
         # URL of documentation
-        self.info.documentationLink = ""
+        self.info.documentation_link = ""
         # Code source repository
         self.info.repository = ""
         # Keywords used for search
         self.info.keywords = "your,keywords,here"
 
     def create(self, param=None):
         # Create process object
-        return {{ PluginClassName }}(self.info.name, param)
+        return {{ cookiecutter.class_name }}(self.info.name, param)
```

## Comparing `ikcli/algo/templates/test.pyt` & `ikcli/algos/templates/{{cookiecutter.plugin_dir}}/{{cookiecutter.algo_name}}_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 from ikomia.core import task
 from ikomia.utils.tests import run_for_test
 
-
 logger = logging.getLogger(__name__)
 
 
 def test(t, data_dict):
     logger.info(f"===== Test::{t.name} =====")
     # 1. Set task parameter if necessary. ex: task.set_parameters(t, {"iteration": 10, "size":3})
     # 2. Get input data from data_dict. ex: img = cv2.imread(data_dict["images"]["detection"]["coco"])[::-1]
```

## Comparing `ikomia_cli-0.1.0.dist-info/METADATA` & `ikomia_cli-0.2.0.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 Metadata-Version: 2.1
 Name: ikomia-cli
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ikomia command line interface
 Author-email: Denis Cavrois <denis.cavrois@ikomia.com>, Ludovic Barusseau <ludovic.barusseau@ikomia.com>
 Platform: any
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.10,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: click (<9.0.0,>=8.1.3)
 Requires-Dist: pyyaml (<7.0.0,>=6.0.0)
 Requires-Dist: requests (<3.0.0,>=2.28.1)
+Requires-Dist: requests-toolbelt (<1.0.0,>=0.10.0)
 Requires-Dist: pillow (<10.0.0,>=9.2.0)
 Requires-Dist: rich (<13.0.0,>=12.6.0)
-Requires-Dist: yarl (<2.0.0,>=1.8.1)
-Requires-Dist: ikomia (<1.0.0,>=0.8.1)
-Requires-Dist: requests-toolbelt (<1.0.0,>=0.10.0)
+Requires-Dist: yarl (<1.9.0,>=1.8.1)
+Provides-Extra: full
+Requires-Dist: cookiecutter (<3.0.0,>=2.1.1) ; extra == 'full'
+Requires-Dist: ikomia (<1.0.0,>=0.9.0) ; extra == 'full'
 
 # Ikomia command line interface
 
 ## Installation
 ```
 $> python3 -m venv .venv
 $> source .venv/bin/activate
 $> pip install ikomia-cli
 ```
 
 ## Manage Ikomia algorithms
 
 List local algorithms
 ```
-$> $ ikcli algo ls
+$> $ ikcli algo local ls
 ```
 
 Create a new empty algorithm
 ```
-$> $ ikcli algo create your_new_algo
+$> $ ikcli algo local create your_new_algo
+```
+
+List algorithms from Ikomia HUB
+```
+$> $ ikcli hub ls
 ```
 
-Publish algorithm to Ikomia HUB
+Show Ikomia HUB algorithm details
 ```
-$> $ ikcli algo publish your_new_algo
+$> $ ikcli hub show algo_name
 ```
```

