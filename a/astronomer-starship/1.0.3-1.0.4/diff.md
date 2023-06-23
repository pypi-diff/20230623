# Comparing `tmp/astronomer_starship-1.0.3.tar.gz` & `tmp/astronomer_starship-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomer_starship-1.0.3.tar", max compression
+gzip compressed data, was "astronomer_starship-1.0.4.tar", max compression
```

## Comparing `astronomer_starship-1.0.3.tar` & `astronomer_starship-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      547 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/LICENSE
--rw-r--r--   0        0        0     9187 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/README.rst
--rw-r--r--   0        0        0        0 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/__init__.py
--rw-r--r--   0        0        0     2434 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/operators.py
--rw-r--r--   0        0        0     4126 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/plugins/__init__.py
--rw-r--r--   0        0        0      262 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/plugins/templates/aeroscope/formhelper.html
--rw-r--r--   0        0        0     2524 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/plugins/templates/aeroscope/main.html
--rw-r--r--   0        0        0     1561 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/aeroscope/util.py
--rw-r--r--   0        0        0        0 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/__init__.py
--rw-r--r--   0        0        0    14265 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/main.py
--rw-r--r--   0        0        0     7950 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/operators.py
--rw-r--r--   0        0        0        0 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/services/__init__.py
--rw-r--r--   0        0        0     7382 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/services/astro_client.py
--rw-r--r--   0        0        0     4416 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/services/local_airflow_client.py
--rw-r--r--   0        0        0     6601 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/services/remote_airflow_client.py
--rw-r--r--   0        0        0    39434 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/static/js/htmx.min.js
--rw-r--r--   0        0        0     7015 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/static/js/idiomorph.min.js
--rw-r--r--   0        0        0    20095 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/static/js/popper.js
--rw-r--r--   0        0        0    25717 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/static/js/tippy.js
--rw-r--r--   0        0        0     1309 2023-06-21 14:45:14.843371 astronomer_starship-1.0.3/astronomer/starship/static/tail-spin.svg
--rw-r--r--   0        0        0     2926 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/dag_row.html
--rw-r--r--   0        0        0      283 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/env_checkbox.html
--rw-r--r--   0        0        0      200 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/github_loop.html
--rw-r--r--   0        0        0      738 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/migrate_connection_button.html
--rw-r--r--   0        0        0      360 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/migrate_pool_button.html
--rw-r--r--   0        0        0      367 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/migrate_variable_button.html
--rw-r--r--   0        0        0     1194 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/tabs.html
--rw-r--r--   0        0        0     2088 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/tabs_loading.html
--rw-r--r--   0        0        0     1661 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/target_deployment_select.html
--rw-r--r--   0        0        0     1227 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/target_deployment_select_loading.html
--rw-r--r--   0        0        0      177 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/test_connection_label.html
--rw-r--r--   0        0        0     2644 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/token_modal.html
--rw-r--r--   0        0        0       15 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/user_label.html
--rw-r--r--   0        0        0     1759 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/connections.html
--rw-r--r--   0        0        0     1089 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/dags.html
--rw-r--r--   0        0        0     1847 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/env.html
--rw-r--r--   0        0        0      775 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/main.html
--rw-r--r--   0        0        0      980 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/migration.html
--rw-r--r--   0        0        0     1415 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/pools.html
--rw-r--r--   0        0        0     1376 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/templates/starship/variables.html
--rw-r--r--   0        0        0     1363 2023-06-21 14:45:14.847371 astronomer_starship-1.0.3/astronomer/starship/variables/operators.py
--rw-r--r--   0        0        0     3190 2023-06-21 14:45:14.855371 astronomer_starship-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    10034 1970-01-01 00:00:00.000000 astronomer_starship-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      547 2023-06-23 17:12:31.917882 astronomer_starship-1.0.4/LICENSE
+-rw-r--r--   0        0        0     9187 2023-06-23 17:12:31.917882 astronomer_starship-1.0.4/README.rst
+-rw-r--r--   0        0        0        0 2023-06-23 17:12:31.917882 astronomer_starship-1.0.4/astronomer/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 17:12:31.917882 astronomer_starship-1.0.4/astronomer/aeroscope/__init__.py
+-rw-r--r--   0        0        0     2434 2023-06-23 17:12:31.917882 astronomer_starship-1.0.4/astronomer/aeroscope/operators.py
+-rw-r--r--   0        0        0     4126 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/aeroscope/plugins/__init__.py
+-rw-r--r--   0        0        0      262 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/aeroscope/plugins/templates/aeroscope/formhelper.html
+-rw-r--r--   0        0        0     2524 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/aeroscope/plugins/templates/aeroscope/main.html
+-rw-r--r--   0        0        0     1561 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/aeroscope/util.py
+-rw-r--r--   0        0        0        0 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/__init__.py
+-rw-r--r--   0        0        0    14265 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/main.py
+-rw-r--r--   0        0        0     7950 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/operators.py
+-rw-r--r--   0        0        0        0 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/services/__init__.py
+-rw-r--r--   0        0        0     7382 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/services/astro_client.py
+-rw-r--r--   0        0        0     4416 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/services/local_airflow_client.py
+-rw-r--r--   0        0        0     6601 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/services/remote_airflow_client.py
+-rw-r--r--   0        0        0    39434 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/static/js/htmx.min.js
+-rw-r--r--   0        0        0     7015 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/static/js/idiomorph.min.js
+-rw-r--r--   0        0        0    20095 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/static/js/popper.js
+-rw-r--r--   0        0        0    25717 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/static/js/tippy.js
+-rw-r--r--   0        0        0     1309 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/static/tail-spin.svg
+-rw-r--r--   0        0        0     2926 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/dag_row.html
+-rw-r--r--   0        0        0      283 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/env_checkbox.html
+-rw-r--r--   0        0        0      200 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/github_loop.html
+-rw-r--r--   0        0        0      738 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/migrate_connection_button.html
+-rw-r--r--   0        0        0      360 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/migrate_pool_button.html
+-rw-r--r--   0        0        0      367 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/migrate_variable_button.html
+-rw-r--r--   0        0        0     1194 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/tabs.html
+-rw-r--r--   0        0        0     2088 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/tabs_loading.html
+-rw-r--r--   0        0        0     1696 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/target_deployment_select.html
+-rw-r--r--   0        0        0     1227 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/target_deployment_select_loading.html
+-rw-r--r--   0        0        0      177 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/test_connection_label.html
+-rw-r--r--   0        0        0     2644 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/token_modal.html
+-rw-r--r--   0        0        0       15 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/user_label.html
+-rw-r--r--   0        0        0     1759 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/connections.html
+-rw-r--r--   0        0        0     1089 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/dags.html
+-rw-r--r--   0        0        0     1847 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/env.html
+-rw-r--r--   0        0        0      775 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/main.html
+-rw-r--r--   0        0        0      980 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/migration.html
+-rw-r--r--   0        0        0     1415 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/pools.html
+-rw-r--r--   0        0        0     1376 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/templates/starship/variables.html
+-rw-r--r--   0        0        0     1363 2023-06-23 17:12:31.921882 astronomer_starship-1.0.4/astronomer/starship/variables/operators.py
+-rw-r--r--   0        0        0     3190 2023-06-23 17:12:31.929882 astronomer_starship-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    10034 1970-01-01 00:00:00.000000 astronomer_starship-1.0.4/PKG-INFO
```

### Comparing `astronomer_starship-1.0.3/LICENSE` & `astronomer_starship-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/README.rst` & `astronomer_starship-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/aeroscope/operators.py` & `astronomer_starship-1.0.4/astronomer/aeroscope/operators.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/aeroscope/plugins/__init__.py` & `astronomer_starship-1.0.4/astronomer/aeroscope/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/aeroscope/plugins/templates/aeroscope/main.html` & `astronomer_starship-1.0.4/astronomer/aeroscope/plugins/templates/aeroscope/main.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/aeroscope/util.py` & `astronomer_starship-1.0.4/astronomer/aeroscope/util.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/main.py` & `astronomer_starship-1.0.4/astronomer/starship/main.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/operators.py` & `astronomer_starship-1.0.4/astronomer/starship/operators.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/services/astro_client.py` & `astronomer_starship-1.0.4/astronomer/starship/services/astro_client.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/services/local_airflow_client.py` & `astronomer_starship-1.0.4/astronomer/starship/services/local_airflow_client.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/services/remote_airflow_client.py` & `astronomer_starship-1.0.4/astronomer/starship/services/remote_airflow_client.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/static/js/htmx.min.js` & `astronomer_starship-1.0.4/astronomer/starship/static/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/static/js/idiomorph.min.js` & `astronomer_starship-1.0.4/astronomer/starship/static/js/idiomorph.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/static/js/popper.js` & `astronomer_starship-1.0.4/astronomer/starship/static/js/popper.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/static/js/tippy.js` & `astronomer_starship-1.0.4/astronomer/starship/static/js/tippy.js`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/static/tail-spin.svg` & `astronomer_starship-1.0.4/astronomer/starship/static/tail-spin.svg`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/dag_row.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/dag_row.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/migrate_connection_button.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/migrate_connection_button.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/tabs.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/tabs.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/tabs_loading.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/tabs_loading.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/target_deployment_select.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/target_deployment_select.html`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                 </div>
                 <div class="col-lg-6">
                     <select id="selectedAstroDeployment" class="form-control" name="selectedAstroDeployment">
                         <option value="">Select deployment</option>
                         {% if deployments %}
                         {% for deploy in deployments.values() %}
                         <option value="{{deploy.id}}" {{'selected' if deploy.id == session.selectedAstroDeployment}}>
-                        {{deploy.label}}
+                        {{ deploy.label if deploy.label else deploy.name }}
                         </option>
                         {% endfor %}
                         {% endif %}
                     </select>
                 </div>
                 <div class="col-lg-3">
                     <button type="submit" class="btn btn-primary mb3-l">Select</button>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 Current user
 {{ username }} (Logout)
 Target Deployment
 {% if deployments %} {% for deploy in deployments.values() %}
-{'selected' if deploy.id == session.selectedAstroDeployment}}> {{deploy.label}}
+{'selected' if deploy.id == session.selectedAstroDeployment}}> {{ deploy.label
+if deploy.label else deploy.name }}
 {% endfor %} {% endif %}
 Select
```

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/target_deployment_select_loading.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/target_deployment_select_loading.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/components/token_modal.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/components/token_modal.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/connections.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/connections.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/dags.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/dags.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/env.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/env.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/main.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/main.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/migration.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/migration.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/pools.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/pools.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/templates/starship/variables.html` & `astronomer_starship-1.0.4/astronomer/starship/templates/starship/variables.html`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/astronomer/starship/variables/operators.py` & `astronomer_starship-1.0.4/astronomer/starship/variables/operators.py`

 * *Files identical despite different names*

### Comparing `astronomer_starship-1.0.3/pyproject.toml` & `astronomer_starship-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "astronomer-starship"
-version = "1.0.3"
+version = "1.0.4"
 description = "Migrations to Astro"
 authors = ["ADE Team <ade@astronomer.io>"]
 readme = "README.rst"
 repository = "https://github.com/astronomer/starship"
 homepage = "https://astronomer.io"
 license = "Proprietary"
 packages = [{include = "astronomer"}]  #, from = "." }]
```

### Comparing `astronomer_starship-1.0.3/PKG-INFO` & `astronomer_starship-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-starship
-Version: 1.0.3
+Version: 1.0.4
 Summary: Migrations to Astro
 Home-page: https://astronomer.io
 License: Proprietary
 Author: ADE Team
 Author-email: ade@astronomer.io
 Requires-Python: >=3.7.2,<4.0
 Classifier: License :: Other/Proprietary License
```

