# Comparing `tmp/invenio-oauthclient-3.1.1.tar.gz` & `tmp/invenio-oauthclient-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-oauthclient-3.1.1.tar", last modified: Wed Jun 21 08:06:18 2023, max compression
+gzip compressed data, was "dist/invenio-oauthclient-3.1.2.tar", last modified: Fri Jun 23 09:35:34 2023, max compression
```

## Comparing `invenio-oauthclient-3.1.1.tar` & `invenio-oauthclient-3.1.2.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3919 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      920 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7820 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7461 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10206 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/examplesapp.rst
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7007 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (122)      169 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/examples/app-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)       85 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/examples/app-teardown.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/examples/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/examples/github_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/examples/github_app_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/examples/globus_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/examples/globus_app_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4561 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/examples/orcid_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/examples/orcid_app_rest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      848 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/_compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py
--rw-r--r--   0 runner    (1001) docker     (122)    12518 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17979 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/cern.py
--rw-r--r--   0 runner    (1001) docker     (122)    15246 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/cern_openid.py
--rw-r--r--   0 runner    (1001) docker     (122)    11557 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/github.py
--rw-r--r--   0 runner    (1001) docker     (122)    11134 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/globus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/keycloak/
--rw-r--r--   0 runner    (1001) docker     (122)     3919 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/keycloak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5168 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/keycloak/handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3570 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/keycloak/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/keycloak/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)    10486 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/openaire_aai.py
--rw-r--r--   0 runner    (1001) docker     (122)    10133 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/orcid.py
--rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     7962 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10451 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8780 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/handlers/rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     6403 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/handlers/ui.py
--rw-r--r--   0 runner    (1001) docker     (122)     9562 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7862 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/postmessage.html
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/rejected.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/signup.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/rejected.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      987 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2843 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     3312 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (122)    11195 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/views/
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9008 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/views/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/invenio_oauthclient/views/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7820 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      939 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      346 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/run-i18n-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1303 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3138 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    17922 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-21 08:06:18.000000 invenio-oauthclient-3.1.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/data/cern_openid_response_content.json
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/data/keycloak_realm_info.json
--rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/data/keycloak_token_response.json
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/data/keycloak_userinfo_response.json
--rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/data/oauth_response_content.json
--rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/data/orcid_bio.json
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_base_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_contrib_cern_openid.py
--rw-r--r--   0 runner    (1001) docker     (122)    11031 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_contrib_cern_openid_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)    13036 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_contrib_github.py
--rw-r--r--   0 runner    (1001) docker     (122)    14224 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_contrib_github_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)    10374 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_contrib_globus.py
--rw-r--r--   0 runner    (1001) docker     (122)    14371 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_contrib_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (122)     9540 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_contrib_orcid.py
--rw-r--r--   0 runner    (1001) docker     (122)     9849 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_contrib_orcid_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_examples_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     9560 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_handlers_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5072 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_handlers_ui.py
--rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    10261 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    17496 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    15887 2023-06-21 08:06:08.000000 invenio-oauthclient-3.1.1/tests/test_views_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7947 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7461 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10206 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/examplesapp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7007 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      169 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/app-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)       85 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/app-teardown.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/github_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/github_app_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/globus_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/globus_app_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4561 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/orcid_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/examples/orcid_app_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      848 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12518 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17979 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/cern.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15246 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/cern_openid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11557 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11134 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/globus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/
+-rw-r--r--   0 runner    (1001) docker     (122)     3919 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5168 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3570 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10486 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/openaire_aai.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10133 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/orcid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7962 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10451 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8780 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6403 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9562 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7862 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/postmessage.html
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/rejected.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/signup.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/rejected.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      987 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2843 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3312 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (122)    11195 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9194 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/views/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/invenio_oauthclient/views/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7947 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      939 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-23 09:35:33.000000 invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      346 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/run-i18n-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1303 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3138 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    17922 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-23 09:35:34.000000 invenio-oauthclient-3.1.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/cern_openid_response_content.json
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/keycloak_realm_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/keycloak_token_response.json
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/keycloak_userinfo_response.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/oauth_response_content.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/data/orcid_bio.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_base_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_cern_openid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11031 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_cern_openid_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13036 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_github.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14224 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_github_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10374 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_globus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14371 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9540 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_orcid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9849 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_contrib_orcid_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_examples_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9560 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_handlers_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5072 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_handlers_ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10261 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17496 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15887 2023-06-23 09:35:26.000000 invenio-oauthclient-3.1.2/tests/test_views_rest.py
```

### Comparing `invenio-oauthclient-3.1.1/.editorconfig` & `invenio-oauthclient-3.1.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/.tx/config` & `invenio-oauthclient-3.1.2/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/AUTHORS.rst` & `invenio-oauthclient-3.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/CHANGES.rst` & `invenio-oauthclient-3.1.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 3.1.2 (released 2023-06-23)
+
+- client: preserve "next" URL param on login redirection
+
 Version 3.1.1 (released 2023-06-21)
 
 - client: fix user confirmation
 
 Version 3.1.0 (released 2023-06-20)
 
 - client: add provider's logout url
```

### Comparing `invenio-oauthclient-3.1.1/CONTRIBUTING.rst` & `invenio-oauthclient-3.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/LICENSE` & `invenio-oauthclient-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/MANIFEST.in` & `invenio-oauthclient-3.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/PKG-INFO` & `invenio-oauthclient-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-oauthclient
-Version: 3.1.1
+Version: 3.1.2
 Summary: "Invenio module that provides OAuth web authorization support."
 Home-page: https://github.com/inveniosoftware/invenio-oauthclient
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -56,14 +56,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.1.2 (released 2023-06-23)
+        
+        - client: preserve "next" URL param on login redirection
+        
         Version 3.1.1 (released 2023-06-21)
         
         - client: fix user confirmation
         
         Version 3.1.0 (released 2023-06-20)
         
         - client: add provider's logout url
```

### Comparing `invenio-oauthclient-3.1.1/README.rst` & `invenio-oauthclient-3.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/docs/Makefile` & `invenio-oauthclient-3.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/docs/api.rst` & `invenio-oauthclient-3.1.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/docs/conf.py` & `invenio-oauthclient-3.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/docs/examplesapp.rst` & `invenio-oauthclient-3.1.2/docs/examplesapp.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/docs/index.rst` & `invenio-oauthclient-3.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/docs/make.bat` & `invenio-oauthclient-3.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/docs/overview.rst` & `invenio-oauthclient-3.1.2/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/docs/usage.rst` & `invenio-oauthclient-3.1.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/examples/app.py` & `invenio-oauthclient-3.1.2/examples/app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/examples/github_app.py` & `invenio-oauthclient-3.1.2/examples/github_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/examples/github_app_rest.py` & `invenio-oauthclient-3.1.2/examples/github_app_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/examples/globus_app.py` & `invenio-oauthclient-3.1.2/examples/globus_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/examples/globus_app_rest.py` & `invenio-oauthclient-3.1.2/examples/globus_app_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/examples/orcid_app.py` & `invenio-oauthclient-3.1.2/examples/orcid_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/examples/orcid_app_rest.py` & `invenio-oauthclient-3.1.2/examples/orcid_app_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/_compat.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/_compat.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/admin.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/config.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/config.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/cern.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/cern.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/cern_openid.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/cern_openid.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/github.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/github.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/globus.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/globus.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/keycloak/__init__.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/keycloak/handlers.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/handlers.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/keycloak/helpers.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/keycloak/settings.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/keycloak/settings.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/openaire_aai.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/openaire_aai.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/orcid.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/orcid.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/contrib/settings.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/contrib/settings.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/errors.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/ext.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/handlers/__init__.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/handlers/base.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/base.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/handlers/rest.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/handlers/ui.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/ui.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/handlers/utils.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/models.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/models.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/signals.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/signals.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/_macros.html` & `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/login_user.html` & `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html` & `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/templates/invenio_oauthclient/signup.html` & `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/invenio_oauthclient/signup.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html` & `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html` & `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html` & `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html` & `invenio-oauthclient-3.1.2/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/da/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/da/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/es/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/es/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/translations/messages.pot` & `invenio-oauthclient-3.1.2/invenio_oauthclient/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/utils.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/views/client.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/views/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,23 @@
     auto_redirect_enabled = current_app.config.get(
         "OAUTHCLIENT_AUTO_REDIRECT_TO_EXTERNAL_LOGIN", False
     )
     would_redirect = auto_redirect_enabled and not local_login_enabled
     remote_apps = list(current_oauthclient.oauth.remote_apps)
 
     if would_redirect and len(remote_apps) == 1:
-        # if local login is disabled and we only have one OAuth2 remote app
-        # configured, we forward directly to that
-        url = url_for("invenio_oauthclient.login", remote_app=remote_apps[0])
+        redirect_args = {
+            # if local login is disabled and we only have one OAuth2 remote app
+            # configured, we forward directly to that
+            "remote_app": remote_apps[0],
+        }
+        next_url = request.args.get("next")
+        if next_url:
+            redirect_args["next"] = next_url
+        url = url_for("invenio_oauthclient.login", **redirect_args)
         return redirect(url)
 
     else:
         return base_login(*args, **kwargs)
 
 
 def _login(remote_app, authorized_view_name):
```

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient/views/settings.py` & `invenio-oauthclient-3.1.2/invenio_oauthclient/views/settings.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/PKG-INFO` & `invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-oauthclient
-Version: 3.1.1
+Version: 3.1.2
 Summary: "Invenio module that provides OAuth web authorization support."
 Home-page: https://github.com/inveniosoftware/invenio-oauthclient
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -56,14 +56,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.1.2 (released 2023-06-23)
+        
+        - client: preserve "next" URL param on login redirection
+        
         Version 3.1.1 (released 2023-06-21)
         
         - client: fix user confirmation
         
         Version 3.1.0 (released 2023-06-20)
         
         - client: add provider's logout url
```

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/SOURCES.txt` & `invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/entry_points.txt` & `invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/invenio_oauthclient.egg-info/requires.txt` & `invenio-oauthclient-3.1.2/invenio_oauthclient.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/requirements-devel.txt` & `invenio-oauthclient-3.1.2/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/run-tests.sh` & `invenio-oauthclient-3.1.2/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/setup.cfg` & `invenio-oauthclient-3.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/conftest.py` & `invenio-oauthclient-3.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/data/keycloak_realm_info.json` & `invenio-oauthclient-3.1.2/tests/data/keycloak_realm_info.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/data/keycloak_token_response.json` & `invenio-oauthclient-3.1.2/tests/data/keycloak_token_response.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/data/oauth_response_content.json` & `invenio-oauthclient-3.1.2/tests/data/oauth_response_content.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/data/orcid_bio.json` & `invenio-oauthclient-3.1.2/tests/data/orcid_bio.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/helpers.py` & `invenio-oauthclient-3.1.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_admin.py` & `invenio-oauthclient-3.1.2/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_app.py` & `invenio-oauthclient-3.1.2/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_base_handlers.py` & `invenio-oauthclient-3.1.2/tests/test_base_handlers.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_contrib_cern_openid.py` & `invenio-oauthclient-3.1.2/tests/test_contrib_cern_openid.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_contrib_cern_openid_rest.py` & `invenio-oauthclient-3.1.2/tests/test_contrib_cern_openid_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_contrib_github.py` & `invenio-oauthclient-3.1.2/tests/test_contrib_github.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_contrib_github_rest.py` & `invenio-oauthclient-3.1.2/tests/test_contrib_github_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_contrib_globus.py` & `invenio-oauthclient-3.1.2/tests/test_contrib_globus.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_contrib_keycloak.py` & `invenio-oauthclient-3.1.2/tests/test_contrib_keycloak.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_contrib_orcid.py` & `invenio-oauthclient-3.1.2/tests/test_contrib_orcid.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_contrib_orcid_rest.py` & `invenio-oauthclient-3.1.2/tests/test_contrib_orcid_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_examples_app.py` & `invenio-oauthclient-3.1.2/tests/test_examples_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_handlers_rest.py` & `invenio-oauthclient-3.1.2/tests/test_handlers_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_handlers_ui.py` & `invenio-oauthclient-3.1.2/tests/test_handlers_ui.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_models.py` & `invenio-oauthclient-3.1.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_utils.py` & `invenio-oauthclient-3.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_views.py` & `invenio-oauthclient-3.1.2/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-3.1.1/tests/test_views_rest.py` & `invenio-oauthclient-3.1.2/tests/test_views_rest.py`

 * *Files identical despite different names*

