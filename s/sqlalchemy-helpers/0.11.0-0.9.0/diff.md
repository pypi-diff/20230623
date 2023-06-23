# Comparing `tmp/sqlalchemy_helpers-0.11.0.tar.gz` & `tmp/sqlalchemy-helpers-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_helpers-0.11.0.tar", max compression
+gzip compressed data, was "sqlalchemy-helpers-0.9.0.tar", max compression
```

## Comparing `sqlalchemy_helpers-0.11.0.tar` & `sqlalchemy-helpers-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,30 @@
--rw-r--r--   0        0        0     7652 2017-09-30 07:16:26.000000 sqlalchemy_helpers-0.11.0/LICENSE
--rw-r--r--   0        0        0     2296 2023-06-23 15:41:00.668812 sqlalchemy_helpers-0.11.0/README.md
--rw-r--r--   0        0        0      156 2023-06-23 15:37:12.270527 sqlalchemy_helpers-0.11.0/docs/_source/sqlalchemy_helpers.aio.rst
--rw-r--r--   0        0        0      168 2023-06-23 15:37:12.272527 sqlalchemy_helpers-0.11.0/docs/_source/sqlalchemy_helpers.fastapi.rst
--rw-r--r--   0        0        0      176 2023-06-23 15:37:12.274527 sqlalchemy_helpers-0.11.0/docs/_source/sqlalchemy_helpers.flask_ext.rst
--rw-r--r--   0        0        0      168 2023-06-23 15:37:12.276527 sqlalchemy_helpers-0.11.0/docs/_source/sqlalchemy_helpers.manager.rst
--rw-r--r--   0        0        0      318 2023-06-23 15:37:12.268527 sqlalchemy_helpers-0.11.0/docs/_source/sqlalchemy_helpers.rst
--rw-r--r--   0        0        0     2410 2023-06-23 15:33:00.486843 sqlalchemy_helpers-0.11.0/docs/aio-env.py.example
--rw-r--r--   0        0        0     6629 2023-06-23 15:33:00.486843 sqlalchemy_helpers-0.11.0/docs/async.rst
--rw-r--r--   0        0        0     3801 2023-06-23 15:33:04.556902 sqlalchemy_helpers-0.11.0/docs/conf.py
--rw-r--r--   0        0        0     6549 2023-06-23 15:33:04.556902 sqlalchemy_helpers-0.11.0/docs/contributing.rst
--rw-r--r--   0        0        0      439 2023-06-23 15:33:04.556902 sqlalchemy_helpers-0.11.0/docs/index.rst
--rw-r--r--   0        0        0      634 2023-06-23 15:41:00.668812 sqlalchemy_helpers-0.11.0/docs/release_notes.rst
--rw-r--r--   0        0        0     8555 2023-06-23 15:33:04.556902 sqlalchemy_helpers-0.11.0/docs/user.rst
--rw-r--r--   0        0        0     3698 2023-06-23 15:41:00.668812 sqlalchemy_helpers-0.11.0/pyproject.toml
--rw-r--r--   0        0        0      734 2023-06-23 15:33:04.558902 sqlalchemy_helpers-0.11.0/sqlalchemy_helpers/__init__.py
--rw-r--r--   0        0        0     6995 2023-06-23 15:33:00.489843 sqlalchemy_helpers-0.11.0/sqlalchemy_helpers/aio.py
--rw-r--r--   0        0        0     1934 2023-06-23 15:33:00.489843 sqlalchemy_helpers-0.11.0/sqlalchemy_helpers/fastapi.py
--rw-r--r--   0        0        0     5394 2023-06-23 15:33:04.558902 sqlalchemy_helpers-0.11.0/sqlalchemy_helpers/flask_ext.py
--rw-r--r--   0        0        0     8632 2023-06-23 15:33:04.558902 sqlalchemy_helpers-0.11.0/sqlalchemy_helpers/manager.py
--rw-r--r--   0        0        0        0 2021-12-06 22:17:22.082613 sqlalchemy_helpers-0.11.0/tests/__init__.py
--rw-r--r--   0        0        0     1714 2023-06-23 15:33:04.558902 sqlalchemy_helpers-0.11.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2021-12-17 07:10:20.616267 sqlalchemy_helpers-0.11.0/tests/integration/__init__.py
--rw-r--r--   0        0        0        0 2021-12-17 08:10:52.236594 sqlalchemy_helpers-0.11.0/tests/integration/app_fixture/__init__.py
--rw-r--r--   0        0        0      639 2021-12-17 08:55:45.743995 sqlalchemy_helpers-0.11.0/tests/integration/app_fixture/app.py
--rw-r--r--   0        0        0       34 2021-12-17 11:27:36.594413 sqlalchemy_helpers-0.11.0/tests/integration/app_fixture/models/__init__.py
--rw-r--r--   0        0        0      225 2021-12-17 11:27:21.915367 sqlalchemy_helpers-0.11.0/tests/integration/app_fixture/models/user.py
--rw-r--r--   0        0        0     1472 2021-12-17 08:21:12.662529 sqlalchemy_helpers-0.11.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     1532 2023-06-23 15:33:04.558902 sqlalchemy_helpers-0.11.0/tests/integration/test_integration.py
--rw-r--r--   0        0        0        0 2021-12-17 07:10:41.279331 sqlalchemy_helpers-0.11.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      310 2023-06-23 15:33:04.558902 sqlalchemy_helpers-0.11.0/tests/unit/models.py
--rw-r--r--   0        0        0     5116 2023-06-23 15:33:00.489843 sqlalchemy_helpers-0.11.0/tests/unit/test_aio.py
--rw-r--r--   0        0        0     5074 2023-06-23 15:33:00.489843 sqlalchemy_helpers-0.11.0/tests/unit/test_fastapi.py
--rw-r--r--   0        0        0     3600 2023-06-23 15:33:04.558902 sqlalchemy_helpers-0.11.0/tests/unit/test_flask_ext.py
--rw-r--r--   0        0        0     3258 2023-06-23 15:33:04.559902 sqlalchemy_helpers-0.11.0/tests/unit/test_manager.py
--rw-r--r--   0        0        0      924 2023-06-23 15:33:04.559902 sqlalchemy_helpers-0.11.0/tox.ini
--rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 sqlalchemy_helpers-0.11.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2017-09-30 07:16:26.000000 sqlalchemy-helpers-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3554 2021-12-17 13:11:40.744889 sqlalchemy-helpers-0.9.0/README.md
+-rw-r--r--   0        0        0      176 2021-12-17 12:30:08.517115 sqlalchemy-helpers-0.9.0/docs/_source/sqlalchemy_helpers.flask_ext.rst
+-rw-r--r--   0        0        0      168 2021-12-17 12:30:08.519115 sqlalchemy-helpers-0.9.0/docs/_source/sqlalchemy_helpers.manager.rst
+-rw-r--r--   0        0        0      262 2021-12-17 12:30:08.514115 sqlalchemy-helpers-0.9.0/docs/_source/sqlalchemy_helpers.rst
+-rw-r--r--   0        0        0     3795 2021-12-17 12:59:27.224601 sqlalchemy-helpers-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0     6549 2021-12-14 16:10:51.103905 sqlalchemy-helpers-0.9.0/docs/contributing.rst
+-rw-r--r--   0        0        0      428 2021-12-17 12:59:27.224601 sqlalchemy-helpers-0.9.0/docs/index.rst
+-rw-r--r--   0        0        0       78 2021-12-06 22:17:52.731702 sqlalchemy-helpers-0.9.0/docs/release_notes.rst
+-rw-r--r--   0        0        0       61 2021-12-06 22:17:52.731702 sqlalchemy-helpers-0.9.0/docs/user.rst
+-rw-r--r--   0        0        0     4069 2021-12-17 13:07:47.247161 sqlalchemy-helpers-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      712 2021-12-17 10:59:40.713185 sqlalchemy-helpers-0.9.0/sqlalchemy_helpers/__init__.py
+-rw-r--r--   0        0        0     5199 2021-12-17 11:27:59.719485 sqlalchemy-helpers-0.9.0/sqlalchemy_helpers/flask_ext.py
+-rw-r--r--   0        0        0     6542 2021-12-17 11:27:51.856460 sqlalchemy-helpers-0.9.0/sqlalchemy_helpers/manager.py
+-rw-r--r--   0        0        0        0 2021-12-06 22:17:22.082613 sqlalchemy-helpers-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     1334 2021-12-17 08:44:57.990975 sqlalchemy-helpers-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2021-12-17 07:10:20.616267 sqlalchemy-helpers-0.9.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-17 08:10:52.236594 sqlalchemy-helpers-0.9.0/tests/integration/app_fixture/__init__.py
+-rw-r--r--   0        0        0      639 2021-12-17 08:55:45.743995 sqlalchemy-helpers-0.9.0/tests/integration/app_fixture/app.py
+-rw-r--r--   0        0        0       34 2021-12-17 11:27:36.594413 sqlalchemy-helpers-0.9.0/tests/integration/app_fixture/models/__init__.py
+-rw-r--r--   0        0        0      225 2021-12-17 11:27:21.915367 sqlalchemy-helpers-0.9.0/tests/integration/app_fixture/models/user.py
+-rw-r--r--   0        0        0     1472 2021-12-17 08:21:12.662529 sqlalchemy-helpers-0.9.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1548 2021-12-17 11:29:27.162757 sqlalchemy-helpers-0.9.0/tests/integration/test_integration.py
+-rw-r--r--   0        0        0        0 2021-12-17 07:10:41.279331 sqlalchemy-helpers-0.9.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      311 2021-12-17 07:11:40.034000 sqlalchemy-helpers-0.9.0/tests/unit/models.py
+-rw-r--r--   0        0        0     3602 2021-12-17 08:54:57.382844 sqlalchemy-helpers-0.9.0/tests/unit/test_flask_ext.py
+-rw-r--r--   0        0        0     2465 2021-12-17 07:13:02.229771 sqlalchemy-helpers-0.9.0/tests/unit/test_manager.py
+-rw-r--r--   0        0        0      984 2021-12-17 09:40:08.033299 sqlalchemy-helpers-0.9.0/tox.ini
+-rw-r--r--   0        0        0     4536 2021-12-17 13:15:10.576756 sqlalchemy-helpers-0.9.0/setup.py
+-rw-r--r--   0        0        0     4838 2021-12-17 13:15:10.577104 sqlalchemy-helpers-0.9.0/PKG-INFO
```

### Comparing `sqlalchemy_helpers-0.11.0/LICENSE` & `sqlalchemy-helpers-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_helpers-0.11.0/docs/conf.py` & `sqlalchemy-helpers-0.9.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,17 @@
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
 
 extlinks = {
-    "commit": ("https://github.com/fedora-infra/sqlalchemy-helpers/commit/%s", "%s"),
-    "issue": ("https://github.com/fedora-infra/sqlalchemy-helpers/issues/%s", "#%s"),
-    "pr": ("https://github.com/fedora-infra/sqlalchemy-helpers/pull/%s", "PR#%s"),
+    "commit": ("https://github.com/fedora-infra/sqlalchemy-helpers/commit/%s", ""),
+    "issue": ("https://github.com/fedora-infra/sqlalchemy-helpers/issues/%s", "#"),
+    "pr": ("https://github.com/fedora-infra/sqlalchemy-helpers/pull/%s", "PR#"),
 }
 
 # -- Misc -----
 
 
 def run_apidoc(_):
     from sphinx.ext import apidoc
```

### Comparing `sqlalchemy_helpers-0.11.0/docs/contributing.rst` & `sqlalchemy-helpers-0.9.0/docs/contributing.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 Guidelines
 ==========
 
 Python Support
 --------------
-SQLAlchemy Helpers supports Python 3.8 or greater. This is automatically enforced by the
+SQLAlchemy Helpers supports Python 3.6 or greater. This is automatically enforced by the
 continuous integration (CI) suite.
 
 
 Code Style
 ----------
 We follow the `PEP8 <https://www.python.org/dev/peps/pep-0008/>`_ style guide
 for Python. This is automatically enforced by the CI suite.
```

### Comparing `sqlalchemy_helpers-0.11.0/pyproject.toml` & `sqlalchemy-helpers-0.9.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-helpers"
-version = "0.11.0"
+version = "0.9.0"
 description = "SQLAlchemy Helpers"
 
 license = "LGPL-3.0-or-later"
 
 authors = [
   "Fedora Infrastructure <admin@fedoraproject.org>"
 ]
@@ -23,83 +23,64 @@
 ]
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Database",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8.0"
+python = "^3.6.2"
 SQLAlchemy = ">=1.3.0"
 alembic = ">=1.6.5"
-Flask = { version = "^2.0.0", optional = true }
-sphinx = {version = "*", optional = true}
-myst-parser = {version = "*", optional = true}
-sphinxcontrib-napoleon = {version = "*", optional = true}
+Flask = { version = "^2.0", optional = true }
+sphinx = {version = "^4", optional = true}
+myst-parser = {version = "^0.16.1", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-cov = "*"
 pytest-mock = "*"
-pytest-asyncio = "*"
 bandit = "*"
 black = "*"
 flake8 = "*"
 isort = "*"
 coverage = {extras = ["toml"], version = "*"}
 liccheck = "*"
-sphinx = "*"
+sphinx = "^4"
 pre-commit = "*"
-myst-parser = "*"
-towncrier = "*"
-aiosqlite = "*"
-psycopg2 = "*"
-asyncpg = "*"
-pydantic = "*"
+myst-parser = "^0.16.1"
 
 [tool.poetry.extras]
 flask = ["Flask"]
-docs = ["sphinx", "myst-parser", "Flask", "sphinxcontrib-napoleon"]
+docs = ["sphinx", "myst-parser"]
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
-[tool.black]
-target-version = ["py38"]
+[tool.isort]
+profile = "black"
+lines_after_imports = 2
+force_alphabetical_sort_within_sections = true
 
-[tool.ruff]
-select = ["E", "F", "W", "I", "UP", "S", "B", "RUF"]
-line-length = 100
-target-version = "py38"
-ignore = ["RUF010", "UP038"]
-
-[tool.ruff.per-file-ignores]
-"tests/*" = ["S101"]
-"tests/integration/*" = ["S603"]
-"news/get-authors.py" = ["S602", "S603", "S607"]
-"docs/conf.py" = ["I001"]
-"sqlalchemy_helpers/__init__.py" = ["F401"]
-
-[tool.ruff.isort]
-lines-after-imports = 2
-order-by-type = false
+[tool.black]
+target-version = ["py36"]
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
 testpaths = [
     "tests",
 ]
 
 [tool.coverage.run]
 branch = true
 source = ["sqlalchemy_helpers"]
@@ -116,15 +97,15 @@
 omit = [
     "sqlalchemy_helpers/__init__.py",
     "sqlalchemy_helpers/migrations/env.py",
 ]
 
 
 [tool.towncrier]
-package = "sqlalchemy_helpers"
+package = "sqlalchemy-helpers"
 filename = "docs/release_notes.rst"
 directory = "news/"
 title_format = "v{version}"
 issue_format = "{issue}"
 template = "news/_template.rst"
 underlines = "=^-"
 wrap = true
@@ -165,7 +146,43 @@
   name = "Other Changes"
   showcontent = true
 
   [[tool.towncrier.type]]
   directory = "author"
   name = "Contributors"
   showcontent = true
+
+
+[tool.liccheck]
+authorized_licenses = [
+  "bsd",
+  "new bsd",
+  "simplified bsd",
+  "apache",
+  "apache 2.0",
+  "apache software",
+  "gnu lgpl",
+  "gpl v2",
+  "GNU General Public License v2 or later (GPLv2+)",
+  "GNU General Public License v3 (GPLv3)",
+  "GNU General Public License v3 or later (GPLv3+)",
+  "GNU Library or Lesser General Public License (LGPL)",
+  "GNU Lesser General Public License v2 or later (LGPLv2+)",
+  "GNU Lesser General Public License v3 or later (LGPLv3+)",
+  "GPLv3+",
+  "LGPLv2+",
+  "gpl v3",
+  "lgpl with exceptions or zpl",
+  "isc",
+  "isc license (iscl)",
+  "mit",
+  "python software foundation",
+  "zpl 2.1",
+  "mpl-2.0",
+  "MPL 2.0",
+  "Mozilla Public License 2.0 (MPL 2.0)",
+  "lgpl",
+  "CC0 (copyright waived)",
+  "Public Domain",
+  "Public Domain <http://unlicense.org>",
+  "Zope Public",
+]
```

### Comparing `sqlalchemy_helpers-0.11.0/sqlalchemy_helpers/__init__.py` & `sqlalchemy-helpers-0.9.0/sqlalchemy_helpers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 
 A set of tools to integrate SQLAlchemy and Alembic in your project, with sane defauts.
 
 Attributes:
     __version__ (str): this package's version.
 """
 
-from .manager import (
+from .manager import (  # noqa: F401
     Base,
     DatabaseManager,
-    DatabaseStatus,
     exists_in_db,
     get_or_create,
     is_sqlite,
-    SyncResult,
 )
 
 
 # Set the version
 try:
     import importlib.metadata
```

### Comparing `sqlalchemy_helpers-0.11.0/sqlalchemy_helpers/aio.py` & `sqlalchemy-helpers-0.9.0/sqlalchemy_helpers/manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,215 +1,202 @@
 """
-Database management (async).
+Database management.
 
 This must remain independent from any web framework.
 
 Attributes:
     Base (object): SQLAlchemy's base class for models.
 """
 
+import enum
 import logging
-from functools import wraps
-from typing import Union
+import os
+from functools import partial
+from sqlite3 import Connection as SQLite3Connection
 
 from alembic import command
+from alembic.config import Config as AlembicConfig
 from alembic.migration import MigrationContext
-from sqlalchemy import exc as sa_exc
-from sqlalchemy import select
-from sqlalchemy.engine import make_url, URL
-from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine
-from sqlalchemy.orm import sessionmaker
+from alembic.script import ScriptDirectory
+from sqlalchemy import create_engine
+from sqlalchemy import event as sa_event
+from sqlalchemy import MetaData
+from sqlalchemy.engine import Engine
+from sqlalchemy.orm import declarative_base, scoped_session, sessionmaker
 from sqlalchemy.orm.exc import NoResultFound
 
-from .manager import Base, DatabaseManager, model_property, SyncResult
 
+Base = declarative_base()
+Base.metadata.naming_convention = {
+    "ix": "ix_%(column_0_label)s",
+    "uq": "uq_%(table_name)s_%(column_0_name)s",
+    "ck": "ck_%(table_name)s_%(constraint_name)s",
+    "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
+    "pk": "pk_%(table_name)s",
+}
 
 _log = logging.getLogger(__name__)
 
 
-def _async_from_sync_url(url: Union[URL, str]) -> URL:
-    """Create an async DB URL from a conventional one."""
-    sync_url = make_url(url)
-
-    try:
-        dialect, _ = sync_url.drivername.split("+", 1)
-    except ValueError:
-        dialect = sync_url.drivername
-
-    if dialect == "sqlite":
-        driver = "aiosqlite"
-    elif dialect == "postgresql":
-        driver = "asyncpg"
-    else:
-        raise ValueError(f"I don't know the asyncio driver for dialect {dialect}")
-
-    return sync_url.set(drivername=f"{dialect}+{driver}")
-
-
-class AsyncDatabaseManager(DatabaseManager):
-    """Helper for a SQLAlchemy and Alembic-powered database, asynchronous version.
+class DatabaseManager:
+    """Helper for a SQLAlchemy and Alembic-powered database
 
     Args:
         uri (str): the database URI
         alembic_location (str): a path to the alembic directory
-        engine_args (dict): additional arguments passed to ``create_async_engine``
 
     Attributes:
+        uri (str): the database URI
         alembic_cfg (alembic.config.Config): the Alembic configuration object
         engine (sqlalchemy.engine.Engine): the SQLAlchemy Engine instance
         Session (sqlalchemy.orm.scoped_session): the SQLAlchemy scoped session factory
     """
 
-    def __init__(self, uri, alembic_location, engine_args=None):
-        super().__init__(uri, alembic_location, engine_args=engine_args)
-        self.Session = sessionmaker(
-            class_=AsyncSession, expire_on_commit=False, bind=self.engine, future=True
+    def __init__(self, uri, alembic_location):
+        self.uri = uri
+        self.engine = create_engine(self.uri)
+        self.Session = scoped_session(
+            sessionmaker(autocommit=False, autoflush=False, bind=self.engine)
         )
-        Base.get_by_pk = model_property(get_by_pk)
-        Base.get_one = model_property(get_one)
-        Base.get_or_create = model_property(get_or_create)
-
-    def _make_engine(self, uri, engine_args):
-        """Create the SQLAlchemy engine.
-
-        Args:
-            uri (str): the database URI
-            engine_args (dict or None): additional arguments passed to ``create_async_engine``
-
-        Returns:
-            sqlalchemy.ext.asyncio.AsyncEngine: the SQLAlchemy engine
-        """
-        engine_args = engine_args or {}
-        engine_args["url"] = _async_from_sync_url(uri)
-        return create_async_engine(**engine_args)
-
-    def configured_connection(self, f):
-        @wraps(f)
-        def wrapper(sync_connection):
-            self.alembic_cfg.attributes["connection"] = sync_connection
-            try:
-                return f(sync_connection)
-            finally:
-                del self.alembic_cfg.attributes["connection"]
-
-        return wrapper
+        Base.query = self.Session.query_property()
+        Base.get_or_create = get_or_create_property(self.Session)
+        # Alembic
+        self.alembic_cfg = AlembicConfig(os.path.join(alembic_location, "alembic.ini"))
+        self.alembic_cfg.set_main_option("script_location", alembic_location)
+        self.alembic_cfg.set_main_option("sqlalchemy.url", self.uri)
 
-    async def get_current_revision(self, session):
+    def get_current_revision(self, session):
         """Get the current alembic database revision."""
-        alembic_context = MigrationContext.configure(
-            url=self.alembic_cfg.get_main_option("sqlalchemy.url")
-        )
-        try:
-            result = await session.execute(alembic_context._version.select())
-        except sa_exc.OperationalError:
-            # Table alembic_version does not exist yet
-            return None
-        current_versions = [row[0] for row in result]
-        if len(current_versions) != 1:
-            # Database is not setup
-            return None
-        return current_versions[0]
-
-    async def create(self):
-        """Create the database tables."""
+        alembic_context = MigrationContext.configure(session.connection())
+        return alembic_context.get_current_revision()
 
-        @self.configured_connection
-        def _run_stamp(connection):
-            Base.metadata.create_all(connection)
-            command.stamp(self.alembic_cfg, "head")
+    def get_latest_revision(self):
+        """Get the most up-to-date alembic database revision available."""
+        script_dir = ScriptDirectory.from_config(self.alembic_cfg)
+        return script_dir.get_current_head()
 
-        async with self.engine.begin() as conn:
-            await conn.run_sync(_run_stamp)
+    def create(self):
+        """Create the database tables."""
+        Base.metadata.create_all(bind=self.engine)
+        command.stamp(self.alembic_cfg, "head")
 
-    async def upgrade(self, target="head"):
+    def upgrade(self):
         """Upgrade the database schema."""
+        command.upgrade(self.alembic_cfg, "head")
 
-        @self.configured_connection
-        def _run_upgrade(_conn):
-            command.upgrade(self.alembic_cfg, target)
-
-        async with self.engine.begin() as conn:
-            await conn.run_sync(_run_upgrade)
-
-    async def drop(self):
+    def drop(self):
         """Drop all the database tables."""
-
-        @self.configured_connection
-        def _run_drop(connection):
-            Base.metadata.drop_all(connection)
-            # Also drop the Alembic version table
+        Base.metadata.drop_all(bind=self.engine)
+        # Also drop the Alembic version table
+        with self.engine.connect() as connection:
             alembic_context = MigrationContext.configure(connection)
             alembic_context._version.drop(bind=connection)
 
-        async with self.engine.begin() as conn:
-            await conn.run_sync(_run_drop)
-
-    async def get_status(self):
-        """Get the status of the database.
-
-        Returns:
-            DatabaseStatus member: see :class:`DatabaseStatus`."""
-        async with self.Session() as session:
-            current = await self.get_current_revision(session=session)
-        return self._compare_to_latest(current)
-
-    async def sync(self):
-        """Create or update the database schema.
-
-        Returns:
-            SyncResult member: see :class:`SyncResult`.
-        """
-        async with self.Session() as session:
-            current_rev = await self.get_current_revision(session)
+    def sync(self):
+        """Create or update the database schema."""
+        with self.Session() as session:
+            current_rev = self.get_current_revision(session)
         # If the database is empty, it should be created ; otherwise it should
         # be upgraded.
         if current_rev is None:
-            await self.create()
+            self.create()
             return SyncResult.CREATED
         elif current_rev == self.get_latest_revision():
             return SyncResult.ALREADY_UP_TO_DATE
         else:
-            await self.upgrade()
+            self.upgrade()
             return SyncResult.UPGRADED
 
 
-# Query helpers
-
-
-async def get_by_pk(pk, *, session, model):
-    """Get a model instance using its primary key.
-
-    Example: ``user = get_by_pk(42, session=session, model=User)``
-    """
-    return await session.get(model, pk)
+class SyncResult(enum.Enum):
+    """The result of a sync() call."""
 
+    ALREADY_UP_TO_DATE = enum.auto()
+    """Returned when the database schema was already up-to-date."""
+    CREATED = enum.auto()
+    """Returned when the database has been created."""
+    UPGRADED = enum.auto()
+    """Returned when the database schema has been upgraded."""
+
+
+# Events
+
+
+@sa_event.listens_for(Engine, "connect")
+def set_sqlite_pragma(dbapi_connection, connection_record):
+    """Automaticall activate foreign keys on SQLite databases."""
+    if isinstance(dbapi_connection, SQLite3Connection):  # pragma: no cover
+        cursor = dbapi_connection.cursor()
+        cursor.execute("PRAGMA foreign_keys=ON")
+        cursor.close()
 
-async def get_one(session: AsyncSession, model, **attrs) -> "Base":
-    """Get an object from the datbase.
 
-    :param session: The SQLAlchemy session to use
-    :param model: The SQLAlchemy model to query
-    :return: the object
-    """
-    return (await session.execute(select(model).filter_by(**attrs))).scalar_one()
+# Query helpers
 
 
-async def get_or_create(session, model, **attrs):
+def get_or_create(session, model, **attrs):
     """Function like Django's ``get_or_create()`` method.
 
     It will return a tuple, the first argument being the instance and the
     second being a boolean: ``True`` if the instance has been created and
     ``False`` otherwise.
 
     Example: ``user, created = get_or_create(session, User, name="foo")``
     """
     try:
-        obj = await get_one(session=session, model=model, **attrs)
+        return session.query(model).filter_by(**attrs).one(), False
     except NoResultFound:
         obj = model(**attrs)
         session.add(obj)
-        await session.flush()  # get an id
-        created = True
-    else:
-        created = False
+        session.flush()  # get an id
+        return obj, True
+
+
+def get_or_create_property(Session):
+    """Add a get_or_create property that behave like Django's.
+
+    Example: ``user, created = User.get_or_create(name="foo")``
+
+    See :func:`get_or_create` for return details.
+
+    Install in on your base model class with:
+    ``Base.get_or_create = get_or_create_property(Session)``
+    """
+    # https://docs.python.org/3/howto/descriptor.html
+    class accessor:
+        def __get__(self, obj, objtype=None):
+            session = Session()
+            return partial(get_or_create, session, objtype)
+
+    return accessor()
+
 
-    return obj, created
+# Migration helpers
+
+
+def is_sqlite(bind):
+    """Check whether the database is SQLite.
+
+    Returns:
+        bool: whether the database is SQLite."""
+    return bind.dialect.name == "sqlite"
+
+
+def exists_in_db(bind, tablename, columnname=None):
+    """Check whether a table and optionally a column exist in the database.
+
+    Args:
+        bind (sqlalchemy.engine.Engine): the database engine or connection.
+        tablename (str): the table to look for.
+        columnname (str, optional): the column to look for, if any. Defaults to None.
+
+    Returns:
+        bool: Whether the database (and column) exist.
+    """
+    md = MetaData()
+    md.reflect(bind=bind)
+    if columnname is None:
+        return tablename in md.tables
+    else:
+        return tablename in md.tables and columnname in [
+            c.name for c in md.tables[tablename].columns
+        ]
```

### Comparing `sqlalchemy_helpers-0.11.0/sqlalchemy_helpers/flask_ext.py` & `sqlalchemy-helpers-0.9.0/sqlalchemy_helpers/flask_ext.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Flask integration of database management.
 """
 
 import os
 
 import click
-from flask import abort, current_app, g, has_app_context
+from flask import _app_ctx_stack, abort, current_app, has_app_context
 from flask.cli import AppGroup
 from werkzeug.utils import find_modules, import_string
 
 from .manager import DatabaseManager, SyncResult
 
 
 def _get_manager():
@@ -38,16 +38,14 @@
 class DatabaseExtension:
     """A Flask extension to configure the database manager according the the app's configuration.
 
     It cleans up database connections at the end of the requests, and creates the CLI endpoint to
     sync the database schema.
     """
 
-    _context_instance_name = "_sqlah_database_manager"
-
     def __init__(self, app=None):
         self.app = app
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app):
         """Initialize the extention on the provided Flask app
@@ -66,15 +64,15 @@
         app.config.setdefault("DB_MODELS_LOCATION", f"{main_module}.models")
         # Connect hook
         app.before_request(self.before_request)
         # Disconnect hook
         app.teardown_appcontext(self.teardown)
         # CLI
         db_cli = AppGroup("db", help="Database operations.")
-        db_cli.command("sync", help="Create or migrate the database.")(_syncdb)
+        db_cli.command("syncdb", help="Create or migrate the database.")(_syncdb)
         app.cli.add_command(db_cli)
         # Import all modules here that might define models so that
         # they will be registered properly on the metadata.
         models_location = app.config["DB_MODELS_LOCATION"]
         try:
             for module in find_modules(
                 models_location, include_packages=True, recursive=True
@@ -82,54 +80,53 @@
                 import_string(module)
         except ValueError:
             # It's just a module, importing it is enough
             import_string(models_location)
 
     def teardown(self, exception):
         """Close the database connection at the end of each requests."""
-        if hasattr(g, self._context_instance_name):
-            getattr(g, self._context_instance_name).Session.remove()
+        ctx = _app_ctx_stack.top
+        if hasattr(ctx, "database_manager"):
+            ctx.database_manager.Session.remove()
 
     def before_request(self):
         """Prepare the database manager at the start of each request.
 
-        This is necessary to allow access to the ``Model.get_*`` methods.
+        This is necessary to allow access to the ``Model.query`` property.
         """
         # Just create the manager
-        self.manager  # noqa: B018
+        self.manager
 
     @property
     def session(self):
         """sqlalchemy.session.Session: the database Session instance to use."""
         return self.manager.Session()
 
     @property
     def manager(self):
         """DatabaseManager: the instance of the database manager."""
-        try:
-            if not hasattr(g, self._context_instance_name):
-                setattr(g, self._context_instance_name, _get_manager())
-            return getattr(g, self._context_instance_name)
-        except RuntimeError:
-            # RuntimeError: Working outside of application context.
-            return None
+        ctx = _app_ctx_stack.top
+        if ctx is not None:
+            if not hasattr(ctx, "database_manager"):
+                ctx.database_manager = _get_manager()
+            return ctx.database_manager
 
 
 # View helpers
 
 
-def get_or_404(Model, pk, description=None):
+def get_or_404(Model, ident, description=None):
     """Like ``query.get`` but aborts with 404 if not found.
 
     Args:
         Model (manager.Base): a model class.
-        pk (int or str): the primary key of the desired record.
+        ident (int or str): the primary key of the desired record.
         description (str, optional): a message for the 404 error if not found.
     """
-    rv = Model.get_by_pk(pk)
+    rv = Model.query.get(ident)
     if rv is None:
         abort(404, description=description)
     return rv
 
 
 def first_or_404(query, description=None):
     """Like ``query.first`` but aborts with 404 if not found.
@@ -146,15 +143,15 @@
 
 # Useful in alembic's env.py
 
 
 def get_url_from_app(app_factory):
     """Get the DB URI from the app configuration
 
-    Create the application if it hasn't been created yet. This is useful in Alembic's ``env.py``.
+    Create the application if it hasn't been created yet.
 
     Args: app_factory (callable): the Flask application factory, to be called if this function is
         called outside of and application context.
     """
     if not has_app_context():
         app = app_factory()
         return app.config["SQLALCHEMY_DATABASE_URI"]
```

### Comparing `sqlalchemy_helpers-0.11.0/tests/integration/app_fixture/app.py` & `sqlalchemy-helpers-0.9.0/tests/integration/app_fixture/app.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_helpers-0.11.0/tests/integration/conftest.py` & `sqlalchemy-helpers-0.9.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_helpers-0.11.0/tests/integration/test_integration.py` & `sqlalchemy-helpers-0.9.0/tests/integration/test_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 
 
 def test_sync_db(full_app, tmpdir):
     """Check that the CLI extension works."""
 
     def syncdb():
         return subprocess.run(
-            [sys.executable, "-m", "flask", "db", "sync"],
+            [sys.executable, "-m", "flask", "db", "syncdb"],
             check=True,
             stdout=subprocess.PIPE,
-            text=True,
+            universal_newlines=True,
         )
 
     result = syncdb()
     assert os.path.exists(os.path.join(tmpdir, "database.sqlite"))
     assert "Database created." in result.stdout
     result = syncdb()
     assert "Database already up-to-date." in result.stdout
```

### Comparing `sqlalchemy_helpers-0.11.0/tests/unit/test_flask_ext.py` & `sqlalchemy-helpers-0.9.0/tests/unit/test_flask_ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 def test_flask_ext_first_or_404(flask_app, flask_client):
     db = DatabaseExtension(flask_app)
     db.manager.create()
     user = make_user(db, "dummy")
 
     @flask_app.route("/user/<name>")
     def view(name):
-        user = first_or_404(db.session.query(User).filter_by(name=name), "no such user")
+        user = first_or_404(User.query.filter_by(name=name), "no such user")
         return jsonify(user.id)
 
     response = flask_client.get("/user/dummy")
     assert response.json == user.id
 
     response = flask_client.get("/user/nobody")
     assert response.status_code == 404
@@ -73,30 +73,30 @@
 def test_flask_ext_script(flask_app, mocker):
     db = DatabaseExtension(flask_app)
     with flask_app.app_context():
         alembic.command.revision(db.manager.alembic_cfg, rev_id="dummy")
         assert not exists_in_db(db.session.get_bind(), "users")
         assert db.manager.get_current_revision(db.session) is None
     assert "db" in flask_app.cli.commands
-    assert "sync" in flask_app.cli.commands["db"].commands
-    sync_cmd = flask_app.cli.commands["db"].commands["sync"]
+    assert "syncdb" in flask_app.cli.commands["db"].commands
+    syncdb_cmd = flask_app.cli.commands["db"].commands["syncdb"]
     runner = flask_app.test_cli_runner()
-    result = runner.invoke(sync_cmd)
+    result = runner.invoke(syncdb_cmd)
     with flask_app.app_context():
         assert exists_in_db(db.session.get_bind(), "users")
         assert db.manager.get_current_revision(db.session) is not None
     assert "Database created." in result.output
-    result = runner.invoke(sync_cmd)
+    result = runner.invoke(syncdb_cmd)
     assert "Database already up-to-date." in result.output
     with flask_app.app_context():
         alembic.command.revision(db.manager.alembic_cfg, rev_id="second")
-    result = runner.invoke(sync_cmd)
+    result = runner.invoke(syncdb_cmd)
     assert "Database upgraded." in result.output
     mocker.patch("sqlalchemy_helpers.flask_ext._get_manager")
-    result = runner.invoke(sync_cmd)
+    result = runner.invoke(syncdb_cmd)
     assert "Unexpected sync result:" in result.output
 
 
 def test_flask_ext_outside_context(flask_app):
     db = DatabaseExtension(flask_app)
     assert db.manager is None
```

### Comparing `sqlalchemy_helpers-0.11.0/tests/unit/test_manager.py` & `sqlalchemy-helpers-0.9.0/tests/unit/test_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,26 @@
-from unittest import mock
-
 import alembic
 import pytest
 
 from sqlalchemy_helpers.manager import (
     DatabaseManager,
-    DatabaseStatus,
     exists_in_db,
     get_or_create,
     is_sqlite,
     SyncResult,
 )
 
 from .models import User
 
 
 @pytest.fixture
 def manager(app):
     return DatabaseManager(app["db_uri"], app["alembic_dir"])
 
 
-def test_manager_engine_args(app, monkeypatch):
-    create_engine = mock.Mock()
-    monkeypatch.setattr("sqlalchemy_helpers.manager.create_engine", create_engine)
-    DatabaseManager(app["db_uri"], app["alembic_dir"], {"foo": "bar"})
-    create_engine.assert_called_once_with(url=app["db_uri"], foo="bar")
-
-
 def test_manager_no_revision(manager):
     assert manager.get_latest_revision() is None
 
 
 def test_manager_get_latest_revision(manager):
     alembic.command.revision(manager.alembic_cfg, rev_id="dummy")
     assert manager.get_latest_revision() == "dummy"
@@ -39,24 +29,14 @@
 def test_manager_create(manager):
     alembic.command.revision(manager.alembic_cfg, rev_id="dummy")
     manager.create()
     with manager.Session() as session:
         assert manager.get_current_revision(session) == "dummy"
 
 
-def test_manager_get_status(manager):
-    assert manager.get_status() == DatabaseStatus.NO_INFO
-    alembic.command.revision(manager.alembic_cfg, rev_id="first")
-    manager.create()
-    alembic.command.revision(manager.alembic_cfg, rev_id="second")
-    assert manager.get_status() == DatabaseStatus.UPGRADE_AVAILABLE
-    alembic.command.stamp(manager.alembic_cfg, "second")
-    assert manager.get_status() == DatabaseStatus.UP_TO_DATE
-
-
 def test_manager_sync(manager):
     alembic.command.revision(manager.alembic_cfg, rev_id="first")
     assert manager.sync() == SyncResult.CREATED
     alembic.command.revision(manager.alembic_cfg, rev_id="second")
     assert manager.sync() == SyncResult.UPGRADED
     assert manager.sync() == SyncResult.ALREADY_UP_TO_DATE
```

