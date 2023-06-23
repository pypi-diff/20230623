# Comparing `tmp/bl_hector-0.2.0.tar.gz` & `tmp/bl_hector-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_hector-0.2.0.tar", max compression
+gzip compressed data, was "bl_hector-0.3.0.tar", max compression
```

## Comparing `bl_hector-0.2.0.tar` & `bl_hector-0.3.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0    34523 2023-06-14 14:53:28.100751 bl_hector-0.2.0/LICENSE
--rw-r--r--   0        0        0     1854 2023-06-14 14:53:28.100751 bl_hector-0.2.0/README.md
--rw-r--r--   0        0        0      807 2023-06-14 14:53:28.100751 bl_hector-0.2.0/bl_hector/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.2.0/bl_hector/application/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.2.0/bl_hector/application/use_cases/__init__.py
--rw-r--r--   0        0        0     3793 2023-06-21 08:04:15.986384 bl_hector-0.2.0/bl_hector/application/use_cases/add_book.py
--rw-r--r--   0        0        0     2044 2023-06-21 08:04:15.986384 bl_hector-0.2.0/bl_hector/application/use_cases/display_book.py
--rw-r--r--   0        0        0     1971 2023-06-21 08:04:15.990384 bl_hector-0.2.0/bl_hector/application/use_cases/look_up_book.py
--rw-r--r--   0        0        0     3729 2023-06-21 08:04:15.990384 bl_hector-0.2.0/bl_hector/application/use_cases/search_books.py
--rw-r--r--   0        0        0     3793 2023-06-21 08:30:56.399424 bl_hector-0.2.0/bl_hector/application/use_cases/update_book.py
--rw-r--r--   0        0        0      944 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/configuration/__init__.py
--rw-r--r--   0        0        0      981 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/configuration/cli.py
--rw-r--r--   0        0        0      986 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/configuration/wsgi.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/__init__.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/entities.py
--rw-r--r--   0        0        0      808 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/enumerations.py
--rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/repositories.py
--rw-r--r--   0        0        0     1196 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/services.py
--rw-r--r--   0        0        0      931 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/administration/value_objects.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/collection_management/__init__.py
--rw-r--r--   0        0        0     1511 2023-06-21 08:04:15.990384 bl_hector-0.2.0/bl_hector/domain/collection_management/entities.py
--rw-r--r--   0        0        0     1505 2023-06-21 08:10:22.593917 bl_hector-0.2.0/bl_hector/domain/collection_management/errors.py
--rw-r--r--   0        0        0     1509 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/collection_management/repositories.py
--rw-r--r--   0        0        0     1173 2023-06-14 14:53:28.104751 bl_hector-0.2.0/bl_hector/domain/collection_management/services.py
--rw-r--r--   0        0        0     1630 2023-06-21 08:14:45.342810 bl_hector-0.2.0/bl_hector/domain/collection_management/validators.py
--rw-r--r--   0        0        0     3039 2023-06-21 08:13:37.175610 bl_hector-0.2.0/bl_hector/domain/collection_management/value_objects.py
--rw-r--r--   0        0        0     1453 2023-06-14 14:53:28.108751 bl_hector-0.2.0/bl_hector/infrastructure/__init__.py
--rw-r--r--   0        0        0     3547 2023-06-19 10:56:43.740572 bl_hector-0.2.0/bl_hector/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1064 2023-06-14 14:53:28.108751 bl_hector-0.2.0/bl_hector/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     1694 2023-06-19 12:33:58.012069 bl_hector-0.2.0/bl_hector/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     4178 2023-06-21 11:13:56.415653 bl_hector-0.2.0/bl_hector/infrastructure/flask/books/__init__.py
--rw-r--r--   0        0        0     3466 2023-06-14 14:53:28.108751 bl_hector-0.2.0/bl_hector/infrastructure/flask/services.py
--rw-r--r--   0        0        0   207302 2023-06-14 14:53:28.108751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
--rw-r--r--   0        0        0    73117 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0      664 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/hector.css
--rw-r--r--   0        0        0      655 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/favicon.svg
--rw-r--r--   0        0        0     1502 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
--rw-r--r--   0        0        0    42819 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
--rw-r--r--   0        0        0    97249 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
--rw-r--r--   0        0        0     6828 2023-06-14 14:53:28.112751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
--rw-r--r--   0        0        0   186112 2023-06-14 14:53:28.116751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-06-14 14:53:28.116751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-06-14 14:53:28.116751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-06-14 14:53:28.116751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-06-14 14:53:28.120751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     2364 2023-06-19 12:33:06.364676 bl_hector-0.2.0/bl_hector/infrastructure/flask/totp/__init__.py
--rw-r--r--   0        0        0     1441 2023-06-19 16:02:47.674444 bl_hector-0.2.0/bl_hector/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     4546 2023-06-19 12:33:06.392676 bl_hector-0.2.0/bl_hector/infrastructure/flask/webauthn/__init__.py
--rw-r--r--   0        0        0     3282 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/flask/webauthn/security.py
--rw-r--r--   0        0        0     1789 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/isbnlib/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/requests/__init__.py
--rw-r--r--   0        0        0     2615 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/settings.py
--rw-r--r--   0        0        0      721 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     8336 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0     2058 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/typer/__init__.py
--rw-r--r--   0        0        0     2886 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/typer/books.py
--rw-r--r--   0        0        0     2099 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/infrastructure/typer/services.py
--rw-r--r--   0        0        0     4007 2023-06-21 08:15:27.830313 bl_hector-0.2.0/bl_hector/interfaces/__init__.py
--rw-r--r--   0        0        0      761 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/interfaces/exceptions.py
--rw-r--r--   0        0        0     3363 2023-06-21 08:32:45.022087 bl_hector-0.2.0/bl_hector/interfaces/from_dict.py
--rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.124751 bl_hector-0.2.0/bl_hector/interfaces/from_json.py
--rw-r--r--   0        0        0     1690 2023-06-19 10:56:43.684572 bl_hector-0.2.0/bl_hector/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0     5368 2023-06-21 08:27:19.978166 bl_hector-0.2.0/bl_hector/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0     5976 2023-06-21 08:27:28.290073 bl_hector-0.2.0/bl_hector/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     2848 2023-06-19 15:46:44.511709 bl_hector-0.2.0/bl_hector/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0    14664 2023-06-21 11:05:08.153809 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     1350 2023-06-21 08:04:12.314430 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0     4202 2023-06-21 10:59:40.789623 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
--rw-r--r--   0        0        0     2100 2023-06-21 06:11:25.884842 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
--rw-r--r--   0        0        0     5740 2023-06-21 10:57:51.862891 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
--rw-r--r--   0        0        0     3569 2023-06-21 11:17:07.421426 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
--rw-r--r--   0        0        0      982 2023-06-14 14:53:28.128751 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     2045 2023-06-21 06:11:25.884842 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     1127 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
--rw-r--r--   0        0        0     4770 2023-06-21 11:06:30.368852 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
--rw-r--r--   0        0        0     1992 2023-06-21 06:11:25.888841 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
--rw-r--r--   0        0        0     1845 2023-06-21 06:11:25.888841 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
--rw-r--r--   0        0        0     2010 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
--rw-r--r--   0        0        0     2045 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
--rw-r--r--   0        0        0     1310 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_http/as_json/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_terminal/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-14 14:53:28.132751 bl_hector-0.2.0/bl_hector/interfaces/to_terminal/as_json.py
--rw-r--r--   0        0        0     5276 2023-06-21 08:04:15.994384 bl_hector-0.2.0/bl_hector/interfaces/to_terminal/as_text.py
--rw-r--r--   0        0        0     1519 2023-06-19 12:33:41.408264 bl_hector-0.2.0/bl_hector/interfaces/utils.py
--rw-r--r--   0        0        0     1570 2023-06-21 11:22:58.541331 bl_hector-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4606 2023-06-21 11:24:22.577414 bl_hector-0.2.0/setup.py
--rw-r--r--   0        0        0     3048 2023-06-21 11:24:22.579179 bl_hector-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-14 14:53:28.100751 bl_hector-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1854 2023-06-14 14:53:28.100751 bl_hector-0.3.0/README.md
+-rw-r--r--   0        0        0      807 2023-06-14 14:53:28.100751 bl_hector-0.3.0/bl_hector/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.3.0/bl_hector/application/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.100751 bl_hector-0.3.0/bl_hector/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3793 2023-06-21 11:30:42.239958 bl_hector-0.3.0/bl_hector/application/use_cases/add_book.py
+-rw-r--r--   0        0        0     2044 2023-06-21 11:30:42.239958 bl_hector-0.3.0/bl_hector/application/use_cases/display_book.py
+-rw-r--r--   0        0        0     1971 2023-06-21 11:30:42.239958 bl_hector-0.3.0/bl_hector/application/use_cases/look_up_book.py
+-rw-r--r--   0        0        0     3729 2023-06-21 11:30:42.239958 bl_hector-0.3.0/bl_hector/application/use_cases/search_books.py
+-rw-r--r--   0        0        0     3793 2023-06-21 11:30:42.243958 bl_hector-0.3.0/bl_hector/application/use_cases/update_book.py
+-rw-r--r--   0        0        0      944 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/configuration/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/configuration/cli.py
+-rw-r--r--   0        0        0      986 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/configuration/wsgi.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/__init__.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/entities.py
+-rw-r--r--   0        0        0      808 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/enumerations.py
+-rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/repositories.py
+-rw-r--r--   0        0        0     1196 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/services.py
+-rw-r--r--   0        0        0      931 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/administration/value_objects.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/collection_management/__init__.py
+-rw-r--r--   0        0        0     1511 2023-06-21 11:30:42.243958 bl_hector-0.3.0/bl_hector/domain/collection_management/entities.py
+-rw-r--r--   0        0        0     1505 2023-06-21 11:30:42.243958 bl_hector-0.3.0/bl_hector/domain/collection_management/errors.py
+-rw-r--r--   0        0        0     1509 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/collection_management/repositories.py
+-rw-r--r--   0        0        0     1173 2023-06-14 14:53:28.104751 bl_hector-0.3.0/bl_hector/domain/collection_management/services.py
+-rw-r--r--   0        0        0     1630 2023-06-21 11:30:42.243958 bl_hector-0.3.0/bl_hector/domain/collection_management/validators.py
+-rw-r--r--   0        0        0     3039 2023-06-21 11:30:42.243958 bl_hector-0.3.0/bl_hector/domain/collection_management/value_objects.py
+-rw-r--r--   0        0        0     1453 2023-06-14 14:53:28.108751 bl_hector-0.3.0/bl_hector/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3547 2023-06-21 11:30:42.247958 bl_hector-0.3.0/bl_hector/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1064 2023-06-14 14:53:28.108751 bl_hector-0.3.0/bl_hector/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     1694 2023-06-21 11:30:42.247958 bl_hector-0.3.0/bl_hector/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     4531 2023-06-23 16:03:54.837120 bl_hector-0.3.0/bl_hector/infrastructure/flask/books/__init__.py
+-rw-r--r--   0        0        0     3466 2023-06-23 15:58:56.080839 bl_hector-0.3.0/bl_hector/infrastructure/flask/services.py
+-rw-r--r--   0        0        0   207302 2023-06-14 14:53:28.108751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css
+-rw-r--r--   0        0        0    73117 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0      664 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/hector.css
+-rw-r--r--   0        0        0      655 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/favicon.svg
+-rw-r--r--   0        0        0     1502 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png
+-rw-r--r--   0        0        0    42819 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js
+-rw-r--r--   0        0        0    97249 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js
+-rw-r--r--   0        0        0     6828 2023-06-14 14:53:28.112751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js
+-rw-r--r--   0        0        0   186112 2023-06-14 14:53:28.116751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-06-14 14:53:28.116751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-06-14 14:53:28.116751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-06-14 14:53:28.116751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-06-14 14:53:28.120751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     2364 2023-06-21 11:30:42.247958 bl_hector-0.3.0/bl_hector/infrastructure/flask/totp/__init__.py
+-rw-r--r--   0        0        0     1479 2023-06-23 15:58:56.080839 bl_hector-0.3.0/bl_hector/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     4546 2023-06-21 11:30:42.251958 bl_hector-0.3.0/bl_hector/infrastructure/flask/webauthn/__init__.py
+-rw-r--r--   0        0        0     3282 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/flask/webauthn/security.py
+-rw-r--r--   0        0        0     1789 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/isbnlib/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/requests/__init__.py
+-rw-r--r--   0        0        0     2615 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/settings.py
+-rw-r--r--   0        0        0      721 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     8336 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2058 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/typer/__init__.py
+-rw-r--r--   0        0        0     2886 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/typer/books.py
+-rw-r--r--   0        0        0     2099 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/infrastructure/typer/services.py
+-rw-r--r--   0        0        0     4012 2023-06-23 06:50:37.016027 bl_hector-0.3.0/bl_hector/interfaces/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/interfaces/exceptions.py
+-rw-r--r--   0        0        0     3363 2023-06-21 11:30:42.251958 bl_hector-0.3.0/bl_hector/interfaces/from_dict.py
+-rw-r--r--   0        0        0     1659 2023-06-14 14:53:28.124751 bl_hector-0.3.0/bl_hector/interfaces/from_json.py
+-rw-r--r--   0        0        0     1690 2023-06-21 11:30:42.255958 bl_hector-0.3.0/bl_hector/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0     5371 2023-06-23 06:50:37.016027 bl_hector-0.3.0/bl_hector/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0     5979 2023-06-23 06:50:37.016027 bl_hector-0.3.0/bl_hector/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1842 2023-06-23 15:58:49.368922 bl_hector-0.3.0/bl_hector/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0    19488 2023-06-23 16:03:34.457374 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     1350 2023-06-21 11:30:42.255958 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0     4238 2023-06-23 15:58:56.080839 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/add.pug
+-rw-r--r--   0        0        0     2105 2023-06-23 15:58:49.368922 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/display.pug
+-rw-r--r--   0        0        0     5746 2023-06-23 15:58:56.080839 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/search.pug
+-rw-r--r--   0        0        0     3633 2023-06-23 15:58:56.084839 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/update.pug
+-rw-r--r--   0        0        0      982 2023-06-14 14:53:28.128751 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     2045 2023-06-23 16:11:12.983659 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     1127 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug
+-rw-r--r--   0        0        0     4768 2023-06-23 15:58:56.096839 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug
+-rw-r--r--   0        0        0     1992 2023-06-21 06:11:25.888841 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug
+-rw-r--r--   0        0        0     1845 2023-06-21 11:30:42.259958 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug
+-rw-r--r--   0        0        0     2010 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug
+-rw-r--r--   0        0        0     2045 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug
+-rw-r--r--   0        0        0     1310 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_http/as_json/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_terminal/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-14 14:53:28.132751 bl_hector-0.3.0/bl_hector/interfaces/to_terminal/as_json.py
+-rw-r--r--   0        0        0     5276 2023-06-21 11:30:42.259958 bl_hector-0.3.0/bl_hector/interfaces/to_terminal/as_text.py
+-rw-r--r--   0        0        0     1519 2023-06-19 12:33:41.408264 bl_hector-0.3.0/bl_hector/interfaces/utils.py
+-rw-r--r--   0        0        0     1570 2023-06-23 16:16:27.055745 bl_hector-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4606 2023-06-23 16:17:09.199821 bl_hector-0.3.0/setup.py
+-rw-r--r--   0        0        0     3048 2023-06-23 16:17:09.201573 bl_hector-0.3.0/PKG-INFO
```

### Comparing `bl_hector-0.2.0/LICENSE` & `bl_hector-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/README.md` & `bl_hector-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/__init__.py` & `bl_hector-0.3.0/bl_hector/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/application/__init__.py` & `bl_hector-0.3.0/bl_hector/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/application/use_cases/__init__.py` & `bl_hector-0.3.0/bl_hector/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/application/use_cases/add_book.py` & `bl_hector-0.3.0/bl_hector/application/use_cases/add_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/application/use_cases/display_book.py` & `bl_hector-0.3.0/bl_hector/application/use_cases/display_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/application/use_cases/look_up_book.py` & `bl_hector-0.3.0/bl_hector/application/use_cases/look_up_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/application/use_cases/search_books.py` & `bl_hector-0.3.0/bl_hector/application/use_cases/search_books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/application/use_cases/update_book.py` & `bl_hector-0.3.0/bl_hector/application/use_cases/update_book.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/configuration/__init__.py` & `bl_hector-0.3.0/bl_hector/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/configuration/cli.py` & `bl_hector-0.3.0/bl_hector/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/configuration/wsgi.py` & `bl_hector-0.3.0/bl_hector/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/__init__.py` & `bl_hector-0.3.0/bl_hector/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/administration/__init__.py` & `bl_hector-0.3.0/bl_hector/domain/administration/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/administration/entities.py` & `bl_hector-0.3.0/bl_hector/domain/administration/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/administration/enumerations.py` & `bl_hector-0.3.0/bl_hector/domain/administration/enumerations.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/administration/repositories.py` & `bl_hector-0.3.0/bl_hector/domain/administration/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/administration/services.py` & `bl_hector-0.3.0/bl_hector/domain/administration/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/administration/value_objects.py` & `bl_hector-0.3.0/bl_hector/domain/administration/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/collection_management/__init__.py` & `bl_hector-0.3.0/bl_hector/domain/collection_management/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/collection_management/entities.py` & `bl_hector-0.3.0/bl_hector/domain/collection_management/entities.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/collection_management/errors.py` & `bl_hector-0.3.0/bl_hector/domain/collection_management/errors.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/collection_management/repositories.py` & `bl_hector-0.3.0/bl_hector/domain/collection_management/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/collection_management/services.py` & `bl_hector-0.3.0/bl_hector/domain/collection_management/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/collection_management/validators.py` & `bl_hector-0.3.0/bl_hector/domain/collection_management/validators.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/domain/collection_management/value_objects.py` & `bl_hector-0.3.0/bl_hector/domain/collection_management/value_objects.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/__init__.py` & `bl_hector-0.3.0/bl_hector/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/__init__.py` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/aliases/__init__.py` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/auth/__init__.py` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/books/__init__.py` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/books/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,60 +37,61 @@
     get_flashed_messages()  # FIXME… wtf?!
     flash(message, type)
 
 
 @blueprint.get("")
 @presenter_to_response
 def search() -> Any:
-    presenter = presenters.SearchBooks(
-        request.args, htmx(request).target, user=services.get_user()
-    )
+    presenter: search_books.Presenter
+    if htmx:
+        presenter = presenters.SearchBooksFragment(
+            htmx.target, request.args, user=services.get_user()
+        )
+    else:
+        presenter = presenters.SearchBooks(request.args, user=services.get_user())
     interactor = search_books.Interactor(presenter, services.get_books())
     controller = controllers.SearchBooks(request.args)
     controller.call(interactor)
     return presenter
 
 
-@blueprint.post("@<string:attribute>")
+@blueprint.post("__validate__")
 @presenter_to_response
-def validate(attribute: str) -> Any:
-    return presenters.ValidateBook(
-        attribute, request.form.get(attribute, ""), user=services.get_user()
-    )
+def validate() -> Any:
+    return presenters.ValidateBook(request.form, user=services.get_user())
 
 
-@blueprint.get("__new__")
+@blueprint.get("__add__")
 @presenter_to_response
-def add() -> Any:
-    return presenters.AddBook(
-        request.form, htmx(request).target, notify, user=services.get_user()
-    )
+def add_form() -> Any:
+    return presenters.AddBookForm(user=services.get_user())
 
 
-@blueprint.post("__new__")
+@blueprint.post("__add__")
 @presenter_to_response
-def add_POST() -> Any:
-    presenter = presenters.AddBook(
-        request.form,
-        htmx(request).target,
-        notify,
-        user=services.get_user(),
-    )
+def add() -> Any:
+    presenter: add_book.Presenter
+    if htmx:
+        presenter = presenters.AddBookFragment(
+            htmx.target, request.form, notify, user=services.get_user()
+        )
+    else:
+        presenter = presenters.AddBook(request.form, notify, user=services.get_user())
     interactor = add_book.Interactor(
         presenter,
         services.get_books(),
         services.get_calendar(),
         services.get_permissions(),
     )
     controller = controllers.AddBook(request.form, str(services.get_user().id))
     controller.call(interactor)
     return presenter
 
 
-@blueprint.post("__info__")
+@blueprint.post("__look_up__")
 @presenter_to_response
 def look_up() -> Any:
     presenter = presenters.LookUpBook(user=services.get_user())
     interactor = look_up_book.Interactor(
         presenter, services.get_book_info_provider(), services.get_cover_provider()
     )
     interactor.execute(look_up_book.Request(request.form.get("isbn", "")))
@@ -104,27 +105,33 @@
     interactor = display_book.Interactor(presenter, services.get_books())
     interactor.execute(display_book.Request(isbn))
     return presenter
 
 
 @blueprint.get("<string:isbn>/__update__")
 @presenter_to_response
-def update(isbn: str) -> Any:
-    presenter = presenters.DisplayBookToUpdate(isbn, notify, user=services.get_user())
+def update_form(isbn: str) -> Any:
+    presenter = presenters.UpdateBookForm(isbn, notify, user=services.get_user())
     interactor = display_book.Interactor(presenter, services.get_books())
     interactor.execute(display_book.Request(isbn))
     return presenter
 
 
 @blueprint.post("<string:isbn>/__update__")
 @presenter_to_response
-def update_POST(isbn: str) -> Any:
-    presenter = presenters.UpdateBook(
-        isbn, request.form, htmx(request).target, notify, user=services.get_user()
-    )
+def update(isbn: str) -> Any:
+    presenter: update_book.Presenter
+    if htmx:
+        presenter = presenters.UpdateBookFragment(
+            htmx.target, isbn, request.form, notify, user=services.get_user()
+        )
+    else:
+        presenter = presenters.UpdateBook(
+            isbn, request.form, notify, user=services.get_user()
+        )
     interactor = update_book.Interactor(
         presenter,
         services.get_books(),
         services.get_calendar(),
         services.get_permissions(),
     )
     controller = controllers.UpdateBook(isbn, request.form, str(services.get_user().id))
```

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/services.py` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/bulma@0.9.4.min.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/css/hector.css` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/css/hector.css`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/favicon.svg` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/img/placeholders/320x480.png`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/htmx@1.9.2.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/hyperscript@0.9.8.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/js/simplewebauthn-browser@7.2.0.umd.min.js`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/totp/__init__.py` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/totp/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/utils.py` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,36 +10,38 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from dataclasses import dataclass
 from functools import wraps
 from typing import Any, Callable
 
-from flask import Request, Response
+from flask import Response, request
 
 from bl_hector.interfaces.to_http import HttpPresenter
 
 
-@dataclass
 class Htmx:
-    target: str
+    def __bool__(self) -> bool:
+        return "HX-Request" in request.headers
 
-
-def htmx(request: Request) -> Htmx:
-    return Htmx(request.headers.get("Hx-Target", ""))
+    @property
+    def target(self) -> str:
+        return request.headers.get("HX-Target", "")
 
 
 def presenter_to_response(f: Callable[..., HttpPresenter]) -> Callable[[], Response]:
     @wraps(f)
     def decorated_function(*args: Any, **kwargs: Any) -> Response:
         presenter = f(*args, **kwargs)
         return Response(
             status=presenter.status_code(),
             headers=presenter.headers(),
             response=presenter.data(),
         )
 
     return decorated_function
+
+
+htmx = Htmx()
```

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/webauthn/__init__.py` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/webauthn/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/flask/webauthn/security.py` & `bl_hector-0.3.0/bl_hector/infrastructure/flask/webauthn/security.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/isbnlib/__init__.py` & `bl_hector-0.3.0/bl_hector/infrastructure/isbnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/requests/__init__.py` & `bl_hector-0.3.0/bl_hector/infrastructure/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/settings.py` & `bl_hector-0.3.0/bl_hector/infrastructure/settings.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/sqlalchemy/__init__.py` & `bl_hector-0.3.0/bl_hector/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/sqlalchemy/repositories.py` & `bl_hector-0.3.0/bl_hector/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/typer/__init__.py` & `bl_hector-0.3.0/bl_hector/infrastructure/typer/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/typer/books.py` & `bl_hector-0.3.0/bl_hector/infrastructure/typer/books.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/infrastructure/typer/services.py` & `bl_hector-0.3.0/bl_hector/infrastructure/typer/services.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/__init__.py` & `bl_hector-0.3.0/bl_hector/interfaces/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,12 +106,12 @@
     if isinstance(error, errors.UnknownBook):
         return translator("unknown-book")
     if isinstance(error, errors.NotAnIsbn):
         return translator("not-an-isbn")
     if isinstance(error, errors.MissingAuthor):
         return translator("missing-author")
     if isinstance(error, errors.BeforeCreationOfIsbn):
-        return translator("before-creation-of-isbn", year=error.year)
+        return translator("before-creation-of-isbn", year=str(error.year))
     if isinstance(error, errors.InvalidValue):
         return translator("incorrect-value")
 
     return translator("unknown-error")
```

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/exceptions.py` & `bl_hector-0.3.0/bl_hector/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/from_dict.py` & `bl_hector-0.3.0/bl_hector/interfaces/from_dict.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/from_json.py` & `bl_hector-0.3.0/bl_hector/interfaces/from_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/l10n/__init__.py` & `bl_hector-0.3.0/bl_hector/interfaces/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/l10n/en-GB/main.ftl` & `bl_hector-0.3.0/bl_hector/interfaces/l10n/en-GB/main.ftl`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 # min (float) The minimum value
 number-too-small = The minimal value is { $min }.
 # max (float) The maximum value
 number-too-big = The maximal value is { $max }.
 unknown-book = Unknown book
 not-an-isbn = This is not an ISBN!
 missing-author = A book must have an author.
-# year (int) The year of creation
+# year (string) The year of creation
 before-creation-of-isbn = ISBN system was introduced in { $year }.
 
 auth-login-title = Log in
 # method (string) The sign in method
 auth-login-method = Sign in using { $method }
 
 webauthn-register-title = Device registration
```

#### html2text {}

```diff
@@ -30,15 +30,15 @@
 unknown-error = An unknown error has occurred! mandatory-value = This value is
 mandatory! incorrect-value = Incorrect value! # min (int) The minimum length
 string-too-short = The minimal length is { $min }. # max (int) The maximum
 length string-too-long = The maximal length is { $max }. # min (float) The
 minimum value number-too-small = The minimal value is { $min }. # max (float)
 The maximum value number-too-big = The maximal value is { $max }. unknown-book
 = Unknown book not-an-isbn = This is not an ISBN! missing-author = A book must
-have an author. # year (int) The year of creation before-creation-of-isbn =
+have an author. # year (string) The year of creation before-creation-of-isbn =
 ISBN system was introduced in { $year }. auth-login-title = Log in # method
 (string) The sign in method auth-login-method = Sign in using { $method }
 webauthn-register-title = Device registration webauthn-register-description =
 Your browser should be asking you to tap your security deviceâ¦ webauthn-
 register-success = Your security device has been succesfully registered!
 webauthn-register-failure = Your security device could not be registered!?
 webauthn-login-title = Log in webauthn-login-description = Your browser should
```

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/l10n/fr-FR/main.ftl` & `bl_hector-0.3.0/bl_hector/interfaces/l10n/fr-FR/main.ftl`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 # min (float) The minimum value
 number-too-small = La valeur minimale est { $min }.
 # max (float) The maximum value
 number-too-big = La valeur maximale est { $max }.
 unknown-book = Livre inconnu.
 not-an-isbn = Ceci n'est pas un ISBN !
 missing-author = Un livre doit absolument avoir un·e aut·rice·eur.
-# year (int) The year of creation
+# year (string) The year of creation
 before-creation-of-isbn = Le système ISBN n'est entré en vigueur qu'en { $year }.
 
 auth-login-title = Connexion
 # method (string) The sign in method
 auth-login-method = Sign in using { $method }
 
 webauthn-register-title = Association du dispositif de sécurité
```

#### html2text {}

```diff
@@ -33,15 +33,15 @@
 obligatoireÂ ! incorrect-value = Cette valeur est incorrecteÂ ! # min (int) The
 minimum length string-too-short = La longueur minimale est { $min }. # max
 (int) The maximum length string-too-long = La longueur maximale est { $max }. #
 min (float) The minimum value number-too-small = La valeur minimale est { $min
 }. # max (float) The maximum value number-too-big = La valeur maximale est
 { $max }. unknown-book = Livre inconnu. not-an-isbn = Ceci n'est pas un ISBNÂ !
 missing-author = Un livre doit absolument avoir unÂ·e autÂ·riceÂ·eur. # year
-(int) The year of creation before-creation-of-isbn = Le systÃ¨me ISBN n'est
+(string) The year of creation before-creation-of-isbn = Le systÃ¨me ISBN n'est
 entrÃ© en vigueur qu'en { $year }. auth-login-title = Connexion # method
 (string) The sign in method auth-login-method = Sign in using { $method }
 webauthn-register-title = Association du dispositif de sÃ©curitÃ© webauthn-
 register-description = Votre navigateur devrait Ãªtre en train de vous demander
 de toucher votre dispositif de sÃ©curitÃ©â¦ webauthn-register-success = Votre
 dispositif de sÃ©curitÃ© a Ã©tÃ© correctement associÃ©Â ! webauthn-register-
 failure = Votre dispositif de sÃ©curitÃ© n'a pas pu Ãªtre associÃ©Â !?
```

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/__init__.py` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -29,58 +29,34 @@
         ...
 
     @abstractmethod
     def data(self) -> str:
         ...
 
 
-class HttpMeta:
-    def __init__(
-        self,
-        content_type: str,
-        /,
-        *,
-        status: int = HTTP.OK,
-        is_logged_in: bool = False,
-        is_htmx: bool = False,
-    ) -> None:
-        self.__status_code: int = status
-        self.__headers: dict[str, Any] = {"Content-Type": content_type}
-        self.__is_logged_in = is_logged_in
-        self.__is_htmx = is_htmx
-
+class HttpMeta(ABC):
+    @abstractmethod
     def see_other(self, target: str, /, *, permanent: bool = False) -> None:
-        self.__status_code = HTTP.MOVED_PERMANENTLY if permanent else HTTP.SEE_OTHER
-
-        if "Content-Type" in self.__headers:
-            del self.__headers["Content-Type"]
-
-        if self.__is_htmx:
-            self.__headers["HX-Location"] = target
-        else:
-            self.__headers["Location"] = target
+        ...
 
+    @abstractmethod
     def bad_request(self) -> None:
-        self.__status_code = HTTP.BAD_REQUEST
+        ...
 
+    @abstractmethod
     def not_authorized(self) -> None:
-        if self.__is_logged_in:
-            self.__status_code = HTTP.FORBIDDEN
-        else:
-            self.__status_code = HTTP.UNAUTHORIZED
+        ...
 
+    @abstractmethod
     def status_code(self) -> int:
-        # TODO set status only if not htmx, for it only handles 2xx and 3xx
-        return self.__status_code
+        ...
 
+    @abstractmethod
     def headers(self) -> dict[str, Any]:
-        # Disable cache for htmx requests
-        if self.__is_htmx:
-            self.__headers["Cache-Control"] = "no-store, max-age=0"
-        return self.__headers
+        ...
 
 
 class Redirection(HttpPresenter):
     def __init__(self, cible: str, code_statut: HTTP = HTTP.SEE_OTHER) -> None:
         self.__cible = cible
         self.__code_statut = code_statut
```

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/__init__.py` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -49,16 +49,76 @@
 def url_for(*args: Any, **kwargs: Any) -> str:
     if "url_for" not in ENVIRONMENT.globals:
         raise RuntimeError("`url_for` is not declared on the environment!")
     return ENVIRONMENT.globals["url_for"](*args, **kwargs)  # type: ignore
 
 
 class HtmlMeta(HttpMeta):
-    def __init__(self, **kwargs: Any) -> None:
-        super().__init__("text/html; charset=UTF-8", **kwargs)
+    def __init__(self, /, *, status: int = HTTP.OK, is_logged_in: bool = False) -> None:
+        self.__status_code: int = status
+        self.__headers: dict[str, Any] = {"Content-Type": "text/html; charset=UTF-8"}
+        self.__is_logged_in = is_logged_in
+
+    def see_other(self, target: str, /, *, permanent: bool = False) -> None:
+        self.__status_code = HTTP.MOVED_PERMANENTLY if permanent else HTTP.SEE_OTHER
+
+        if "Content-Type" in self.__headers:
+            del self.__headers["Content-Type"]
+
+        self.__headers["Location"] = target
+
+    def bad_request(self) -> None:
+        self.__status_code = HTTP.BAD_REQUEST
+
+    def not_authorized(self) -> None:
+        if self.__is_logged_in:
+            self.__status_code = HTTP.FORBIDDEN
+        else:
+            self.__status_code = HTTP.UNAUTHORIZED
+
+    def status_code(self) -> int:
+        return self.__status_code
+
+    def headers(self) -> dict[str, Any]:
+        return self.__headers
+
+
+class HtmxMeta(HttpMeta):
+    def __init__(self, /, *, status: int = HTTP.OK, is_logged_in: bool = False) -> None:
+        self.__status_code: int = status
+        self.__headers: dict[str, Any] = {"Content-Type": "text/html; charset=UTF-8"}
+        self.__is_logged_in = is_logged_in
+
+    def see_other(self, target: str, /, *, permanent: bool = False) -> None:
+        self.__status_code = HTTP.MOVED_PERMANENTLY if permanent else HTTP.SEE_OTHER
+
+        if "Content-Type" in self.__headers:
+            del self.__headers["Content-Type"]
+
+        self.__headers["HX-Location"] = target
+
+    def replace(self, target: str) -> None:
+        self.__headers["HX-Push-Url"] = target
+
+    def bad_request(self) -> None:
+        self.__status_code = HTTP.BAD_REQUEST
+
+    def not_authorized(self) -> None:
+        if self.__is_logged_in:
+            self.__status_code = HTTP.FORBIDDEN
+        else:
+            self.__status_code = HTTP.UNAUTHORIZED
+
+    def status_code(self) -> int:
+        return self.__status_code
+
+    def headers(self) -> dict[str, Any]:
+        # Prevent problem when navigating with the back button
+        self.__headers["Cache-Control"] = "no-store, max-age=0"
+        return self.__headers
 
 
 class HtmlContent:
     def __init__(self, target: str, context: Optional[dict[str, Any]] = None) -> None:
         self.__template, self.__fragment = self.__parse(target)
         self.__context = context or {}
 
@@ -136,27 +196,40 @@
         _ = l10n.translator_for(user.locale if user else "")
         self.meta = HtmlMeta(status=HTTP.BAD_REQUEST)
         self.content = HtmlContent(
             "error", {"user": user, "_": _, "message": _("bad-request")}
         )
 
 
-class SearchBooks(HtmlOverHttpMixin, HttpPresenter, search_books.Presenter):
+class SearchBooksOptionalFragment(
+    HtmlOverHttpMixin, HttpPresenter, search_books.Presenter
+):
     def __init__(
         self,
         data: MultiDict[str, Any],
-        fragment: str,
         /,
         *,
+        fragment: str = "",
         user: Optional[User] = None,
     ) -> None:
         self._ = l10n.translator_for(user.locale if user else "")
         pager = Pager(url_for("books.search", **data))
 
-        self.meta = HtmlMeta(is_htmx=bool(fragment))
+        if fragment:
+            self.meta = HtmxMeta()
+            self.meta.replace(
+                url_for(
+                    "books.search",
+                    # Remove empty values and page number
+                    **{k: v for k, v in data.items() if v and k != "page"},
+                )
+            )
+        else:
+            self.meta = HtmlMeta()
+
         self.content = HtmlContent(
             f"books/search#{fragment}",
             {"_": self._, "user": user, "data": data, "errors": {}, "pager": pager},
         )
 
         if data:  # Handle the case when the search returns no book.
             self.content.set("books", [])
@@ -184,28 +257,59 @@
                 "authors": [str(a) for a in book.authors],
                 "genres": [str(g) for g in book.genres],
                 "cover": str(book.cover) if book.cover else "",
             },
         )
 
 
-class AddBook(HtmlOverHttpMixin, HttpPresenter, add_book.Presenter):
+class SearchBooksFragment(SearchBooksOptionalFragment):
     def __init__(
         self,
-        data: MultiDict[str, Any],
         fragment: str,
+        data: MultiDict[str, Any],
+        /,
+        *,
+        user: Optional[User] = None,
+    ) -> None:
+        super().__init__(data, fragment=fragment, user=user)
+
+
+class SearchBooks(SearchBooksOptionalFragment):
+    def __init__(
+        self, data: MultiDict[str, Any], /, *, user: Optional[User] = None
+    ) -> None:
+        super().__init__(data, user=user)
+
+
+class AddBookForm(HtmlOverHttpMixin, HttpPresenter):
+    def __init__(self, /, *, user: Optional[User] = None) -> None:
+        self._ = l10n.translator_for(user.locale if user else "")
+        self.meta = HtmlMeta(is_logged_in=bool(user))
+        self.content = HtmlContent(
+            "books/add", {"user": user, "_": self._, "data": {}, "errors": {}}
+        )
+
+
+class AddBookOptionalFragment(HtmlOverHttpMixin, HttpPresenter, add_book.Presenter):
+    def __init__(
+        self,
+        data: MultiDict[str, Any],
         notify: Callable[[str, str], None],
         /,
         *,
+        fragment: str = "",
         user: Optional[User] = None,
     ) -> None:
         self._ = l10n.translator_for(user.locale if user else "")
-        self.meta = HtmlMeta(is_logged_in=bool(user), is_htmx=bool(fragment))
+        if fragment:
+            self.meta = HtmxMeta(is_logged_in=bool(user))
+        else:
+            self.meta = HtmlMeta(is_logged_in=bool(user))
         self.content = HtmlContent(
-            f"books/add#{fragment}",
+            "books/add",
             {"user": user, "_": self._, "data": data, "errors": {}},
         )
         self.__notify = notify
 
     def bad_request(self, errors: add_book.Errors) -> None:
         self.content.set(
             "errors",
@@ -229,14 +333,39 @@
                 url=url_for("books.display", isbn=str(book.isbn)),
             ),
             "success",
         )
         self.meta.see_other(url_for("books.add"))
 
 
+class AddBookFragment(AddBookOptionalFragment):
+    def __init__(
+        self,
+        fragment: str,
+        data: MultiDict[str, Any],
+        notify: Callable[[str, str], None],
+        /,
+        *,
+        user: Optional[User] = None,
+    ) -> None:
+        super().__init__(data, notify, fragment=fragment, user=user)
+
+
+class AddBook(AddBookOptionalFragment):
+    def __init__(
+        self,
+        data: MultiDict[str, Any],
+        notify: Callable[[str, str], None],
+        /,
+        *,
+        user: Optional[User] = None,
+    ) -> None:
+        super().__init__(data, notify, user=user)
+
+
 class LookUpBook(HtmlOverHttpMixin, HttpPresenter, look_up_book.Presenter):
     def __init__(self, /, *, user: Optional[User] = None) -> None:
         self._ = l10n.translator_for(user.locale if user else "")
         self.meta = HtmlMeta()
         self.content = HtmlContent(
             "books/add#form", {"user": user, "_": self._, "data": {}, "errors": {}}
         )
@@ -301,15 +430,15 @@
                 "authors": ", ".join([str(a) for a in book.authors]),
                 "genres": ", ".join([str(g) for g in book.genres]),
                 "cover": str(book.cover) if book.cover else "",
             },
         )
 
 
-class DisplayBookToUpdate(HtmlOverHttpMixin, HttpPresenter, display_book.Presenter):
+class UpdateBookForm(HtmlOverHttpMixin, HttpPresenter, display_book.Presenter):
     def __init__(
         self,
         isbn: str,
         notify: Callable[[str, str], None],
         /,
         *,
         user: Optional[User] = None,
@@ -343,27 +472,32 @@
                 "authors": ", ".join([str(a) for a in book.authors]),
                 "genres": ", ".join([str(g) for g in book.genres]),
                 "cover": str(book.cover) if book.cover else "",
             },
         )
 
 
-class UpdateBook(HtmlOverHttpMixin, HttpPresenter, update_book.Presenter):
+class UpdateBookOptionalFragment(
+    HtmlOverHttpMixin, HttpPresenter, update_book.Presenter
+):
     def __init__(
         self,
         isbn: str,
         data: MultiDict[str, Any],
-        fragment: str,
         notify: Callable[[str, str], None],
         /,
         *,
+        fragment: str = "",
         user: Optional[User] = None,
     ) -> None:
         self._ = l10n.translator_for(user.locale if user else "")
-        self.meta = HtmlMeta(is_logged_in=bool(user), is_htmx=bool(fragment))
+        if fragment:
+            self.meta = HtmxMeta(is_logged_in=bool(user))
+        else:
+            self.meta = HtmlMeta(is_logged_in=bool(user))
         self.content = HtmlContent(
             f"books/update#{fragment}",
             {"user": user, "_": self._, "isbn": isbn, "data": data, "errors": {}},
         )
         self.__notify = notify
 
     def bad_request(self, errors: update_book.Errors) -> None:
@@ -381,26 +515,53 @@
         self.meta.see_other(url_for("books.search"))
 
     def book_updated(self, book: Book) -> None:
         self.__notify(self._("update-book-success"), "success")
         self.meta.see_other(url_for("books.display", isbn=str(book.isbn)))
 
 
+class UpdateBookFragment(UpdateBookOptionalFragment):
+    def __init__(
+        self,
+        fragment: str,
+        isbn: str,
+        data: MultiDict[str, Any],
+        notify: Callable[[str, str], None],
+        /,
+        *,
+        user: Optional[User] = None,
+    ) -> None:
+        super().__init__(isbn, data, notify, fragment=fragment, user=user)
+
+
+class UpdateBook(UpdateBookOptionalFragment):
+    def __init__(
+        self,
+        isbn: str,
+        data: MultiDict[str, Any],
+        notify: Callable[[str, str], None],
+        /,
+        *,
+        user: Optional[User] = None,
+    ) -> None:
+        super().__init__(isbn, data, notify, user=user)
+
+
 class ValidateBook(HtmlOverHttpMixin, HttpPresenter):
     def __init__(
-        self, attribute: str, value: str, /, *, user: Optional[User] = None
+        self, data: MultiDict[str, Any], /, *, user: Optional[User] = None
     ) -> None:
+        if len(data.keys()) != 1:
+            raise RuntimeError("Only one attribute can be validated at a time!")
+        attribute = list(data.keys())[0]
+        value = data[attribute]
+
         self._ = l10n.translator_for(user.locale if user else "")
         errors = self.__validate(attribute, value)
-        context = {
-            "user": user,
-            "_": self._,
-            "data": {attribute: value},
-            "errors": errors,
-        }
+        context = {"user": user, "_": self._, "data": data, "errors": errors}
 
         self.meta = HtmlMeta()
         # We use `search` as it contains all fields as not required.
         self.content = HtmlContent(f"books/search#{attribute}", context)
 
     def __validate(self, attribute: str, value: str) -> dict[str, str]:
         errors: dict[str, str] = {}
```

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/add.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/add.pug`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     .container
       h1.title.is-3= _("add-book-title")
 
       block form
         include mixins/form
         form#form(
           method="POST"
-          action=""
-          hx-post=""
+          action=url_for("books.add")
+          hx-post=url_for("books.add")
           hx-target="#form"
         )
           .columns
             .column.is-one-quarter
               input#coverUploader.is-hidden(
                 accept="image/*"
                 type="file"
```

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/display.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/display.pug`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 block content
   section.section
     .container
       //- Fixes a spacing problem.
       .buttons.is-pulled-right(style="margin-bottom: -1rem")
         if user.can_update_book
-          a.button.is-link(href="#{url_for('books.update', isbn=book.isbn)}")
+          a.button.is-link(href="#{url_for('books.update_form', isbn=book.isbn)}")
             span.icon: i.fas.fa-edit
             span= _("update-book-action")
         else
           button.button.is-link.is-disabled(disabled title=_("update-book-requires-authentification"))
             span.icon: i.fas.fa-edit
             span= _("update-book-action")
```

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/search.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/search.pug`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   title= _("hector") + " – " + _("search-books-title")
 
 block content
   section.section
     .container
       .buttons.is-pulled-right
         if user.can_add_book
-          a.button.is-link(href=url_for("books.add"))
+          a.button.is-link(href=url_for("books.add_form"))
             span.icon: i.fas.fa-plus
             span= _("add-book-action")
         else
           button.button.is-link.is-disabled(disabled title=_("add-book-requires-authentification"))
             span.icon: i.fas.fa-plus
             span= _("add-book-action")
 
@@ -38,15 +38,15 @@
         #search
           include mixins/form
           form(
             method="GET"
             action=url_for("books.search")
             hx-get=url_for("books.search")
             hx-target="#search"
-            hx-push-url="true"
+            hx-push-url="false"
           )
             +hidden_input("page", data.page or "1")
 
             block isbn
               include mixins/form
               +isbn_field(data.isbn, errors.isbn)
```

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/books/update.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/books/update.pug`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     .container
       h1.title.is-3= _("update-book-title", isbn=isbn)
 
       block form
         include mixins/form
         form#form(
           method="POST"
-          action=""
-          hx-post=""
+          action=url_for("books.update", isbn=isbn)
+          hx-post=url_for("books.update", isbn=isbn)
           hx-target="#form"
         )
           .columns
             .column.is-one-quarter
               input#coverUploader.is-hidden(
                 accept="image/*"
                 type="file"
```

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/error.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/layout.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/layout.pug`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
     link(rel="icon" type="image/svg" href="#{url_for('static', filename='favicon.svg')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/bulma@0.9.4.min.css')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/font-awesome@5.14.0.css')}")
     link(rel="stylesheet" href="#{url_for('static', filename='css/hector.css')}")
     block links
 
+    script(src="#{url_for('static', filename='js/hyperscript@0.9.8.min.js')}")
+    script(src="#{url_for('static', filename='js/htmx@1.9.2.min.js')}")
     block head_scripts
 
   body(hx-boost="true")
     +navbar()
 
     .page
       - var messages = get_flashed_messages(with_categories=true)
@@ -47,10 +49,8 @@
     footer.footer
       .content.has-text-centered
         p
           span= _("copyright", version=version, years="2023", holders="Bioneland") | safe
           br
           span= _("license", name="AGPL", url="https://www.gnu.org/licenses/agpl-3.0.fr.html") | safe
 
-    script(src="#{url_for('static', filename='js/hyperscript@0.9.8.min.js')}")
-    script(src="#{url_for('static', filename='js/htmx@1.9.2.min.js')}")
     block scripts
```

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/flash.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/form.pug`

 * *Files 2% similar despite different names*

```diff
@@ -110,21 +110,21 @@
     p.help= field.description
 
 mixin render_hidden(field)
   input(type="hidden" name="#{field.name}" value="#{field.data}")
 
 
 mixin isbn_field(data, error)
-  .field(hx-trigger="blur from:#isbn" hx-post=url_for("books.validate", attribute="isbn") hx-target="this" hx-push-url="false")
+  .field(hx-trigger="blur from:#isbn" hx-post=url_for("books.validate") hx-target="this" hx-params="isbn" hx-push-url="false")
     +text_input("isbn", data, error=error, icon="calendar", placeholder=_('book-isbn'))
     +error_message(error)
     +help_message(_("book-isbn-description"))
 
 mixin year_field(data, error)
-  .field(hx-trigger="blur from:#year" hx-post=url_for("books.validate", attribute="year") hx-target="this" hx-push-url="false")
+  .field(hx-trigger="blur from:#year" hx-post=url_for("books.validate") hx-target="this" hx-params="year" hx-push-url="false")
     +number_input("year", data, error=error, icon="calendar", placeholder=_("book-year"))
     +error_message(error)
     +help_message(_("book-year-description"))
 
 //- At the bottom of the file for it f**ks up the highlighting!?
 mixin render_input(field, placeholder="")
   - var classes = "input"
```

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/mixins/navbar.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/totp/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/login.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_html/templates/webauthn/register.pug`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_http/as_json/__init__.py` & `bl_hector-0.3.0/bl_hector/interfaces/to_http/as_json/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_terminal/__init__.py` & `bl_hector-0.3.0/bl_hector/interfaces/to_terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_terminal/as_json.py` & `bl_hector-0.3.0/bl_hector/interfaces/to_terminal/as_json.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/to_terminal/as_text.py` & `bl_hector-0.3.0/bl_hector/interfaces/to_terminal/as_text.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/bl_hector/interfaces/utils.py` & `bl_hector-0.3.0/bl_hector/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `bl_hector-0.2.0/pyproject.toml` & `bl_hector-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bl_hector"
-version = "0.2.0"
+version = "0.3.0"
 description = "A collection manager."
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://git.easter-eggs.org/bioneland/hector"
 
 exclude = [
```

### Comparing `bl_hector-0.2.0/setup.py` & `bl_hector-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 {'totp': ['pyotp>=2.8.0,<3.0.0'], 'webauthn': ['webauthn>=1.8.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['hector = bl_hector.configuration.cli:cli']}
 
 setup_kwargs = {
     'name': 'bl-hector',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'A collection manager.',
     'long_description': '# Hector — a collection manager\n\n## Install\n\nHector is available on PyPI under the name `bl_hector`.\nTo install, just run `python -m pip install bl_hector`.\n\n\n## Configure\n\nHector is configured using environment variables.\nSee [the `settings` module](bl_hector/infrastructure/settings.py) for\na comprehensive list of configuration variables.\n\nAll the variable names must be prefixed with `HECTOR_`. For instance\xa0:\n\n```console\n# The secret can be generated using the `secrets.token_hex()` function.\n$ export HECTOR_SECRET_KEY="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"\n\n# Additional Python database drivers might be required depending on the DSN.\n$ export HECTOR_DSN="sqlite:///data.sqlite"\n```\n\n\n## Authentication\n\nTo enable WebAuthn authentication, you must install extra dependencies (`bl-hector[webauthn]`)\nand enable it explicitly:\n\n```console\n$ export HECTOR_WEBAUTHN_ENABLED=1\n```\n\nTOTP authentication is provided to be able to login on servers that do not (yet) support\nthe `cryptography` module. You must install extra dependencies (`bl-hector[totp]`)\nand enable it explicitly by setting a base32 random secret:\n\n```console\n# The secret can be generated using the `pyotp.random_base32()` function.\n$ export HECTOR_TOTP_SECRET=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX\n```\n\nNote that it is a highly insecure way of authenticating, as anyone gaining access to your\nOTP generator would be able to login.\n\n\n## Initialise\n\nOnce configured, you must initialise Hector\'s database with the dedicated command:\n\n```console\n$ hector init-db\n```\n\n\n## Run\n\nHector being a Flask application, it can be run using any WSGI server,\nfor instance, with [Gunicorn](https://gunicorn.org):\n\n```console\n$ gunicorn --access-logfile="-" -w 4 -b 127.0.0.1:3000 "bl_hector.configuration.wsgi:app()"\n```\n\n\n## Contributing\n\nSee [CONTRIBUTING.md]() to set up a development environment.\n',
     'author': 'Tanguy Le Carrour',
     'author_email': 'tanguy@bioneland.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://git.easter-eggs.org/bioneland/hector',
```

### Comparing `bl_hector-0.2.0/PKG-INFO` & `bl_hector-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bl-hector
-Version: 0.2.0
+Version: 0.3.0
 Summary: A collection manager.
 Home-page: https://git.easter-eggs.org/bioneland/hector
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

