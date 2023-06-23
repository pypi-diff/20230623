# Comparing `tmp/wagtail_non_admin_draftail-0.18.1.tar.gz` & `tmp/wagtail_non_admin_draftail-0.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_non_admin_draftail-0.18.1.tar", max compression
+gzip compressed data, was "wagtail_non_admin_draftail-0.18.2.tar", max compression
```

## Comparing `wagtail_non_admin_draftail-0.18.1.tar` & `wagtail_non_admin_draftail-0.18.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1548 2023-06-14 09:53:10.100242 wagtail_non_admin_draftail-0.18.1/LICENSE
--rw-r--r--   0        0        0     1107 2023-06-23 19:31:51.176047 wagtail_non_admin_draftail-0.18.1/pyproject.toml
--rwxr-xr-x   0        0        0      128 2023-06-23 15:04:27.743545 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/__init__.py
--rwxr-xr-x   0        0        0      117 2023-06-23 15:04:27.728220 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/apps.py
--rw-r--r--   0        0        0      181 2023-06-23 19:30:51.780625 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/conf.py
--rw-r--r--   0        0        0     2298 2023-06-23 19:30:51.782413 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/forms.py
--rw-r--r--   0        0        0     7906 2023-06-14 09:53:10.102702 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/draftail.css
--rw-r--r--   0        0        0     1090 2023-06-14 09:53:10.102790 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/draftail.css.map
--rw-r--r--   0        0        0     4337 2023-06-14 09:53:10.102891 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/modal-workflow.js
--rwxr-xr-x   0        0        0       25 2023-06-14 09:53:10.102997 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/.gitignore
--rwxr-xr-x   0        0        0      816 2023-06-23 15:04:27.754982 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/README.md
--rw-r--r--   0        0        0    13948 2023-06-14 09:53:10.104023 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/package-lock.json
--rwxr-xr-x   0        0        0      295 2023-06-23 15:04:27.739372 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/package.json
--rw-r--r--   0        0        0      129 2023-06-14 09:53:10.104195 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/src/index.scss
--rw-r--r--   0        0        0     1326 2023-06-14 09:53:10.104304 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/src/styles/chooser.scss
--rw-r--r--   0        0        0     1111 2023-06-14 09:53:10.104380 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/src/styles/editor.scss
--rw-r--r--   0        0        0     1285 2023-06-14 09:53:10.104452 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/src/styles/modal.scss
--rw-r--r--   0        0        0     3121 2023-06-14 09:53:10.104538 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/src/styles/tooltip.scss
--rw-r--r--   0        0        0      163 2023-06-23 15:04:27.729293 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/_draftail_css.html
--rw-r--r--   0        0        0     5223 2023-06-23 16:00:09.640526 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/_draftail_js.html
--rw-r--r--   0        0        0      658 2023-06-23 15:04:27.740823 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/document/upload.html
--rw-r--r--   0        0        0      123 2023-06-23 15:04:27.748923 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/draftail_media.html
--rw-r--r--   0        0        0      458 2023-06-23 15:04:27.732641 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/embed/chooser.html
--rw-r--r--   0        0        0      638 2023-06-23 15:04:27.738446 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/image/select_format.html
--rw-r--r--   0        0        0      713 2023-06-23 15:04:27.742621 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/image/upload.html
--rw-r--r--   0        0        0     1463 2023-06-23 15:04:27.737453 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/_link_types.html
--rw-r--r--   0        0        0      526 2023-06-23 15:04:27.741728 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/anchor_link.html
--rw-r--r--   0        0        0      523 2023-06-23 15:04:27.731565 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/email_link.html
--rw-r--r--   0        0        0      522 2023-06-23 15:04:27.727007 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/external_link.html
--rw-r--r--   0        0        0      522 2023-06-23 15:04:27.735276 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/phone_link.html
--rw-r--r--   0        0        0      269 2023-06-14 09:53:10.105707 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/modal_base.html
--rwxr-xr-x   0        0        0      202 2023-06-14 09:53:10.105815 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/widgets/non_admin_draftail_rich_text_area.html
--rw-r--r--   0        0        0        0 2023-06-14 09:53:10.105893 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templatetags/__init__.py
--rw-r--r--   0        0        0      182 2023-06-14 09:53:10.106004 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templatetags/wagtail_non_admin_draftail_tags.py
--rw-r--r--   0        0        0     1617 2023-06-23 15:04:27.724815 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/urls.py
--rw-r--r--   0        0        0        0 2023-06-14 09:53:10.106159 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/views/__init__.py
--rw-r--r--   0        0        0     3386 2023-06-23 18:55:57.604026 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/views/document.py
--rw-r--r--   0        0        0     3206 2023-06-23 15:04:27.753983 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/views/embed.py
--rw-r--r--   0        0        0     5514 2023-06-23 19:23:42.284434 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/views/image.py
--rw-r--r--   0        0        0     6349 2023-06-23 15:04:27.751124 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/views/link.py
--rwxr-xr-x   0        0        0      848 2023-06-23 15:04:27.746579 wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/widgets.py
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 wagtail_non_admin_draftail-0.18.1/PKG-INFO
+-rw-r--r--   0        0        0     1548 2023-06-14 09:53:10.100242 wagtail_non_admin_draftail-0.18.2/LICENSE
+-rw-r--r--   0        0        0     1107 2023-06-23 20:00:49.725435 wagtail_non_admin_draftail-0.18.2/pyproject.toml
+-rwxr-xr-x   0        0        0      128 2023-06-23 15:04:27.743545 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/__init__.py
+-rwxr-xr-x   0        0        0      117 2023-06-23 15:04:27.728220 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/apps.py
+-rw-r--r--   0        0        0      181 2023-06-23 19:30:51.780625 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/conf.py
+-rw-r--r--   0        0        0     2298 2023-06-23 19:30:51.782413 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/forms.py
+-rw-r--r--   0        0        0     7906 2023-06-14 09:53:10.102702 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/draftail.css
+-rw-r--r--   0        0        0     1090 2023-06-14 09:53:10.102790 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/draftail.css.map
+-rw-r--r--   0        0        0     4337 2023-06-14 09:53:10.102891 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/modal-workflow.js
+-rwxr-xr-x   0        0        0       25 2023-06-14 09:53:10.102997 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/.gitignore
+-rwxr-xr-x   0        0        0      816 2023-06-23 15:04:27.754982 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/README.md
+-rw-r--r--   0        0        0    13948 2023-06-14 09:53:10.104023 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/package-lock.json
+-rwxr-xr-x   0        0        0      295 2023-06-23 15:04:27.739372 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/package.json
+-rw-r--r--   0        0        0      129 2023-06-14 09:53:10.104195 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/src/index.scss
+-rw-r--r--   0        0        0     1326 2023-06-14 09:53:10.104304 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/src/styles/chooser.scss
+-rw-r--r--   0        0        0     1111 2023-06-14 09:53:10.104380 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/src/styles/editor.scss
+-rw-r--r--   0        0        0     1285 2023-06-14 09:53:10.104452 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/src/styles/modal.scss
+-rw-r--r--   0        0        0     3121 2023-06-14 09:53:10.104538 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/src/styles/tooltip.scss
+-rw-r--r--   0        0        0      163 2023-06-23 15:04:27.729293 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/_draftail_css.html
+-rw-r--r--   0        0        0     5223 2023-06-23 16:00:09.640526 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/_draftail_js.html
+-rw-r--r--   0        0        0      658 2023-06-23 15:04:27.740823 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/document/upload.html
+-rw-r--r--   0        0        0      123 2023-06-23 15:04:27.748923 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/draftail_media.html
+-rw-r--r--   0        0        0      458 2023-06-23 15:04:27.732641 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/embed/chooser.html
+-rw-r--r--   0        0        0      638 2023-06-23 15:04:27.738446 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/image/select_format.html
+-rw-r--r--   0        0        0      713 2023-06-23 15:04:27.742621 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/image/upload.html
+-rw-r--r--   0        0        0     1463 2023-06-23 15:04:27.737453 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/_link_types.html
+-rw-r--r--   0        0        0      526 2023-06-23 15:04:27.741728 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/anchor_link.html
+-rw-r--r--   0        0        0      523 2023-06-23 15:04:27.731565 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/email_link.html
+-rw-r--r--   0        0        0      522 2023-06-23 15:04:27.727007 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/external_link.html
+-rw-r--r--   0        0        0      522 2023-06-23 15:04:27.735276 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/phone_link.html
+-rw-r--r--   0        0        0      269 2023-06-14 09:53:10.105707 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/modal_base.html
+-rwxr-xr-x   0        0        0      202 2023-06-14 09:53:10.105815 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/widgets/non_admin_draftail_rich_text_area.html
+-rw-r--r--   0        0        0        0 2023-06-14 09:53:10.105893 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templatetags/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-14 09:53:10.106004 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templatetags/wagtail_non_admin_draftail_tags.py
+-rw-r--r--   0        0        0     1617 2023-06-23 15:04:27.724815 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/urls.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:53:10.106159 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/views/__init__.py
+-rw-r--r--   0        0        0     3386 2023-06-23 18:55:57.604026 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/views/document.py
+-rw-r--r--   0        0        0     3206 2023-06-23 15:04:27.753983 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/views/embed.py
+-rw-r--r--   0        0        0     5514 2023-06-23 19:23:42.284434 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/views/image.py
+-rw-r--r--   0        0        0     6349 2023-06-23 15:04:27.751124 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/views/link.py
+-rwxr-xr-x   0        0        0      840 2023-06-23 19:58:20.027274 wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/widgets.py
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 wagtail_non_admin_draftail-0.18.2/PKG-INFO
```

### Comparing `wagtail_non_admin_draftail-0.18.1/LICENSE` & `wagtail_non_admin_draftail-0.18.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/pyproject.toml` & `wagtail_non_admin_draftail-0.18.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wagtail_non_admin_draftail"
-version = "0.18.1"
+version = "0.18.2"
 description = "You can now use Wagtail Draftail editor on non-admin pages"
 authors = ["Tim Kamanin <tim@timonweb.com>"]
 license = "MIT"
 homepage = "https://timonweb.com"
 repository = "https://github.com/timonweb/wagtail-non-admin-draftail"
 
 [tool.poetry.dependencies]
```

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/forms.py` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/draftail.css` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/draftail.css`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/draftail.css.map` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/draftail.css.map`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/modal-workflow.js` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static/wagtail_non_admin_draftail/modal-workflow.js`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/README.md` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/package-lock.json` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/package-lock.json`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/src/styles/chooser.scss` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/src/styles/chooser.scss`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/src/styles/editor.scss` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/src/styles/editor.scss`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/src/styles/modal.scss` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/src/styles/modal.scss`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/static_src/src/styles/tooltip.scss` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/static_src/src/styles/tooltip.scss`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/_draftail_js.html` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/_draftail_js.html`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/document/upload.html` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/document/upload.html`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/image/select_format.html` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/image/select_format.html`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/image/upload.html` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/image/upload.html`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/_link_types.html` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/_link_types.html`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/anchor_link.html` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/anchor_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/email_link.html` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/email_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/external_link.html` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/external_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/phone_link.html` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/templates/wagtail_non_admin_draftail/link/phone_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/urls.py` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/views/document.py` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/views/document.py`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/views/embed.py` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/views/embed.py`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/views/image.py` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/views/image.py`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/views/link.py` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/views/link.py`

 * *Files identical despite different names*

### Comparing `wagtail_non_admin_draftail-0.18.1/wagtail_non_admin_draftail/widgets.py` & `wagtail_non_admin_draftail-0.18.2/wagtail_non_admin_draftail/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,8 @@
             class Meta:
                 model = Note
                 fields = ["text"]
                 widgets = {"text": NonAdminDraftailRichTextArea}
         ```
     """
 
-    template_name = "wagtail_non_admin_draftail/widgets/wagtail_non_admin_draftail_rich_text_area.html"
+    template_name = "wagtail_non_admin_draftail/widgets/non_admin_draftail_rich_text_area.html"
```

### Comparing `wagtail_non_admin_draftail-0.18.1/PKG-INFO` & `wagtail_non_admin_draftail-0.18.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-non-admin-draftail
-Version: 0.18.1
+Version: 0.18.2
 Summary: You can now use Wagtail Draftail editor on non-admin pages
 Home-page: https://timonweb.com
 License: MIT
 Author: Tim Kamanin
 Author-email: tim@timonweb.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

