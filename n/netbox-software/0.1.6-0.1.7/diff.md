# Comparing `tmp/netbox_software-0.1.6.tar.gz` & `tmp/netbox_software-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_software-0.1.6.tar", max compression
+gzip compressed data, was "netbox_software-0.1.7.tar", max compression
```

## Comparing `netbox_software-0.1.6.tar` & `netbox_software-0.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.1.6/LICENSE
--rw-r--r--   0        0        0     3420 2023-06-20 09:07:55.621872 netbox_software-0.1.6/README.md
--rw-r--r--   0        0        0      636 2023-06-22 13:33:06.697182 netbox_software-0.1.6/netbox_software/__init__.py
--rw-r--r--   0        0        0      616 2023-06-19 13:55:08.848877 netbox_software-0.1.6/netbox_software/admin.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.6/netbox_software/api/__init__.py
--rw-r--r--   0        0        0     3459 2023-06-20 10:54:23.034743 netbox_software-0.1.6/netbox_software/api/serializers.py
--rw-r--r--   0        0        0      399 2023-06-20 09:54:33.084309 netbox_software-0.1.6/netbox_software/api/urls.py
--rw-r--r--   0        0        0     1076 2023-06-20 09:54:33.056309 netbox_software-0.1.6/netbox_software/api/views.py
--rw-r--r--   0        0        0     1705 2023-06-20 11:07:06.570213 netbox_software-0.1.6/netbox_software/filtersets.py
--rw-r--r--   0        0        0     3975 2023-06-20 10:07:37.384282 netbox_software-0.1.6/netbox_software/forms.py
--rw-r--r--   0        0        0     5261 2023-06-20 10:12:28.772709 netbox_software-0.1.6/netbox_software/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.6/netbox_software/migrations/__init__.py
--rw-r--r--   0        0        0     5779 2023-06-22 13:29:04.297691 netbox_software-0.1.6/netbox_software/models.py
--rw-r--r--   0        0        0     2299 2023-06-20 09:07:55.625872 netbox_software-0.1.6/netbox_software/navigation.py
--rw-r--r--   0        0        0     1029 2023-06-20 09:54:33.080309 netbox_software-0.1.6/netbox_software/search.py
--rw-r--r--   0        0        0     2857 2023-06-20 09:54:33.060309 netbox_software-0.1.6/netbox_software/tables.py
--rw-r--r--   0        0        0     2133 2023-06-20 09:54:33.040309 netbox_software-0.1.6/netbox_software/template_content.py
--rw-r--r--   0        0        0     1455 2023-06-21 06:29:50.919881 netbox_software-0.1.6/netbox_software/templates/netbox_software/devicesoftware.html
--rw-r--r--   0        0        0      693 2023-06-20 10:19:13.746862 netbox_software-0.1.6/netbox_software/templates/netbox_software/devicesoftware_edit.html
--rw-r--r--   0        0        0     2230 2023-06-20 10:19:00.870666 netbox_software-0.1.6/netbox_software/templates/netbox_software/devicesoftware_include.html
--rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.1.6/netbox_software/templates/netbox_software/software_edit.html
--rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.1.6/netbox_software/templates/netbox_software/softwaretype.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.6/netbox_software/templates/netbox_software/softwaretype_edit.html
--rw-r--r--   0        0        0     1725 2023-06-22 12:45:05.033649 netbox_software-0.1.6/netbox_software/templates/netbox_software/vendor.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.6/netbox_software/templates/netbox_software/vendor_edit.html
--rw-r--r--   0        0        0     1352 2023-06-21 06:17:56.368583 netbox_software-0.1.6/netbox_software/templates/netbox_software/virtualmachinesoftware.html
--rw-r--r--   0        0        0      697 2023-06-20 10:19:00.898666 netbox_software-0.1.6/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html
--rw-r--r--   0        0        0     2372 2023-06-20 10:19:00.890666 netbox_software-0.1.6/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html
--rw-r--r--   0        0        0     2994 2023-06-20 09:54:33.052309 netbox_software-0.1.6/netbox_software/urls.py
--rw-r--r--   0        0        0     4296 2023-06-20 14:19:58.292417 netbox_software-0.1.6/netbox_software/views.py
--rw-r--r--   0        0        0      318 2023-06-22 13:33:06.701182 netbox_software-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3420 2023-06-20 09:07:55.621872 netbox_software-0.1.7/README.md
+-rw-r--r--   0        0        0      636 2023-06-23 08:10:05.968201 netbox_software-0.1.7/netbox_software/__init__.py
+-rw-r--r--   0        0        0      616 2023-06-19 13:55:08.848877 netbox_software-0.1.7/netbox_software/admin.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.7/netbox_software/api/__init__.py
+-rw-r--r--   0        0        0     3459 2023-06-20 10:54:23.034743 netbox_software-0.1.7/netbox_software/api/serializers.py
+-rw-r--r--   0        0        0      399 2023-06-20 09:54:33.084309 netbox_software-0.1.7/netbox_software/api/urls.py
+-rw-r--r--   0        0        0     1076 2023-06-20 09:54:33.056309 netbox_software-0.1.7/netbox_software/api/views.py
+-rw-r--r--   0        0        0     1705 2023-06-20 11:07:06.570213 netbox_software-0.1.7/netbox_software/filtersets.py
+-rw-r--r--   0        0        0     3975 2023-06-20 10:07:37.384282 netbox_software-0.1.7/netbox_software/forms.py
+-rw-r--r--   0        0        0     5261 2023-06-20 10:12:28.772709 netbox_software-0.1.7/netbox_software/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.7/netbox_software/migrations/__init__.py
+-rw-r--r--   0        0        0     5779 2023-06-22 13:29:04.297691 netbox_software-0.1.7/netbox_software/models.py
+-rw-r--r--   0        0        0     2299 2023-06-20 09:07:55.625872 netbox_software-0.1.7/netbox_software/navigation.py
+-rw-r--r--   0        0        0     1029 2023-06-20 09:54:33.080309 netbox_software-0.1.7/netbox_software/search.py
+-rw-r--r--   0        0        0     2857 2023-06-20 09:54:33.060309 netbox_software-0.1.7/netbox_software/tables.py
+-rw-r--r--   0        0        0     2663 2023-06-23 07:46:52.094449 netbox_software-0.1.7/netbox_software/template_content.py
+-rw-r--r--   0        0        0     1455 2023-06-21 06:29:50.919881 netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware.html
+-rw-r--r--   0        0        0      693 2023-06-20 10:19:13.746862 netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware_edit.html
+-rw-r--r--   0        0        0     2384 2023-06-23 07:56:09.499077 netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware_include.html
+-rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.1.7/netbox_software/templates/netbox_software/software_edit.html
+-rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.1.7/netbox_software/templates/netbox_software/softwaretype.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.7/netbox_software/templates/netbox_software/softwaretype_edit.html
+-rw-r--r--   0        0        0     1725 2023-06-22 12:45:05.033649 netbox_software-0.1.7/netbox_software/templates/netbox_software/vendor.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.7/netbox_software/templates/netbox_software/vendor_edit.html
+-rw-r--r--   0        0        0     1352 2023-06-21 06:17:56.368583 netbox_software-0.1.7/netbox_software/templates/netbox_software/virtualmachinesoftware.html
+-rw-r--r--   0        0        0      697 2023-06-20 10:19:00.898666 netbox_software-0.1.7/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html
+-rw-r--r--   0        0        0     2639 2023-06-23 07:56:09.487077 netbox_software-0.1.7/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html
+-rw-r--r--   0        0        0     2994 2023-06-20 09:54:33.052309 netbox_software-0.1.7/netbox_software/urls.py
+-rw-r--r--   0        0        0     4296 2023-06-20 14:19:58.292417 netbox_software-0.1.7/netbox_software/views.py
+-rw-r--r--   0        0        0      318 2023-06-23 08:10:05.972201 netbox_software-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.1.7/PKG-INFO
```

### Comparing `netbox_software-0.1.6/LICENSE` & `netbox_software-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/README.md` & `netbox_software-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/__init__.py` & `netbox_software-0.1.7/netbox_software/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from extras.plugins import PluginConfig
 
 
 class NetboxSoftware(PluginConfig):
     name = 'netbox_software'
     verbose_name = 'Установленное ПО'
     description = 'Manage device software in Netbox'
-    version = '0.1.6'
+    version = '0.1.7'
     author = 'Ilya Zakharov'
     author_email = 'me@izakharov.ru'
     min_version = '3.2.0'
     base_url = 'software'
     default_settings = {
         "enable_navigation_menu": True,
         "enable_device_software": True,
```

### Comparing `netbox_software-0.1.6/netbox_software/admin.py` & `netbox_software-0.1.7/netbox_software/admin.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/api/serializers.py` & `netbox_software-0.1.7/netbox_software/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/api/views.py` & `netbox_software-0.1.7/netbox_software/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/filtersets.py` & `netbox_software-0.1.7/netbox_software/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/forms.py` & `netbox_software-0.1.7/netbox_software/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/migrations/0001_initial.py` & `netbox_software-0.1.7/netbox_software/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/models.py` & `netbox_software-0.1.7/netbox_software/models.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/navigation.py` & `netbox_software-0.1.7/netbox_software/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/search.py` & `netbox_software-0.1.7/netbox_software/search.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/tables.py` & `netbox_software-0.1.7/netbox_software/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/template_content.py` & `netbox_software-0.1.7/netbox_software/template_content.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,45 +7,53 @@
 
 class DeviceSoftwareList(PluginTemplateExtension):
     model = 'dcim.device'
     def left_page(self):
         if plugin_settings.get('enable_device_software') and plugin_settings.get('device_software_location') == 'left':
 
             return self.render('netbox_software/devicesoftware_include.html', extra_context={
-                'device_software': DeviceSoftware.objects.filter(device=self.context['object']),
+                'device_software': DeviceSoftware.objects.filter(device=self.context['object'])[:20],
+                'soft_count': DeviceSoftware.objects.filter(device=self.context['object']).count(),
             })
         else:
             return ""
 
     def right_page(self):
         if plugin_settings.get('enable_device_software') and plugin_settings.get('device_software_location') == 'right':
 
             return self.render('netbox_software/devicesoftware_include.html', extra_context={
-                'device_software': DeviceSoftware.objects.filter(device=self.context['object']),
+                'device_software': DeviceSoftware.objects.filter(device=self.context['object'])[:20],
+                'soft_count': DeviceSoftware.objects.filter(device=self.context['object']).count(),
             })
         else:
             return ""
 
 
 class VirtualMachineSoftwareList(PluginTemplateExtension):
     model = 'virtualization.virtualmachine'
 
     def left_page(self):
         if plugin_settings.get('enable_virtual-machine_software') and plugin_settings.get('virtual-machine_software_location') == 'left':
 
             return self.render('netbox_software/virtualmachinesoftware_include.html', extra_context={
-                'virtual_machine_software': VirtualMachineSoftware.objects.filter(virtual_machine=self.context['object']),
+                'virtual_machine_software': VirtualMachineSoftware.objects.filter(
+                    virtual_machine=self.context['object']
+                )[:20],
+                'soft_count': VirtualMachineSoftware.objects.filter(virtual_machine=self.context['object']).count(),
             })
         else:
             return ""
 
     def right_page(self):
         if plugin_settings.get('enable_virtual-machine_software') and plugin_settings.get('virtual-machine_software_location') == 'right':
 
             return self.render('netbox_software/virtualmachinesoftware_include.html', extra_context={
-                'virtual_machine_software': VirtualMachineSoftware.objects.filter(virtual_machine=self.context['object']),
+                'virtual_machine_software': VirtualMachineSoftware.objects.filter(
+                    virtual_machine=self.context['object']
+                )[:20],
+                'soft_count': VirtualMachineSoftware.objects.filter(virtual_machine=self.context['object']).count(),
             })
         else:
             return ""
 
 
 template_extensions = [DeviceSoftwareList, VirtualMachineSoftwareList]
```

### Comparing `netbox_software-0.1.6/netbox_software/templates/netbox_software/devicesoftware.html` & `netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/templates/netbox_software/devicesoftware_edit.html` & `netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/templates/netbox_software/devicesoftware_include.html` & `netbox_software-0.1.7/netbox_software/templates/netbox_software/devicesoftware_include.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 {% load helpers %}
 
 <div class="card">
 <h5 class="card-header">
     ПО устройства
+    {% if device_software %}
+      <a href="{% url 'plugins:netbox_software:devicesoftware_list' %}?device={{ object.pk }}">
+        (всего: {{ soft_count }})</a>
+    {% endif %}
 </h5>
 <div class="card-body">
 {% if device_software %}
     <table class="table table-hover">
         <tr>
             <th>Название</th>
-            <th>источник</th>
             <th>версия</th>
-            <th>Тип</th>
             <th></th>
         </tr>
         {% for software in device_software %}
         <tr>
             <td>
                 {{ software.name }}
             </td>
-            <td>{{ software.vendor }}</td>
             <td>{{ software.version }}</td>
-            <td>{% badge software.get_software_type_display bg_color=software.get_software_type_color %}</td>
             <td class="text-end noprint">
                 <a href="{% url 'plugins:netbox_software:devicesoftware' pk=software.pk %}"
                    class="btn btn-primary btn-sm lh-1" title="Просмотреть">
                     <i class="mdi mdi-book" aria-hidden="true"></i>
                   </a>
                   <a href="{% url 'plugins:netbox_software:devicesoftware_edit' pk=software.pk %}?return_url=
                   {% url 'dcim:device' pk=object.pk %}" class="btn btn-warning btn-sm lh-1" title="Редактировать">
@@ -46,9 +46,12 @@
     {% endif %}
     </div>
         <div class="card-footer text-end noprint">
             <a href="{% url 'plugins:netbox_software:devicesoftware_add' %}?device={{ object.pk }}&return_url={% url 'dcim:device' pk=object.pk %}" class="btn btn-primary btn-sm">
                 <i class="mdi mdi-plus-thick" aria-hidden="true"></i>
                 Добавить ПО
             </a>
+            <a href="{% url 'plugins:netbox_software:devicesoftware_list' %}?device={{ object.pk }}" class="btn btn-primary btn-sm">
+                Все ПО хоста
+            </a>
         </div>
 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 {% load helpers %}
-** ÐÐ ÑÑÑÑÐ¾Ð¹ÑÑÐ²Ð° **
+** ÐÐ ÑÑÑÑÐ¾Ð¹ÑÑÐ²Ð° {% if device_software %} (Ð²ÑÐµÐ³Ð¾:_{
+{_soft_count_}}) {% endif %} **
 {% if device_software %}
-ÐÐ°Ð·Ð²�Ð¸ÑÑÐ¾�Ð²ÐµÑÑ�Ð¢Ð¸Ð¿
-                 {                {                {% badge
-{{ software.name {                {                software.get_software_type_display
-}}               software.vendor  software.version bg_color=software.get_software_type_color
-                 }}               }}               %}
+ÐÐ°Ð·Ð²Ð°Ð²ÐµÑÑÐ¸Ñ
+{{ software.name }} {{ software.version }}
 {% else %}
 ÐÐµÑ
 {% endif %}
  ÐÐ¾Ð±Ð°Ð²Ð¸ÑÑ_ÐÐ
+ ÐÑÐµ_ÐÐ_ÑÐ¾ÑÑÐ°
```

### Comparing `netbox_software-0.1.6/netbox_software/templates/netbox_software/software_edit.html` & `netbox_software-0.1.7/netbox_software/templates/netbox_software/software_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/templates/netbox_software/softwaretype.html` & `netbox_software-0.1.7/netbox_software/templates/netbox_software/softwaretype.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/templates/netbox_software/vendor.html` & `netbox_software-0.1.7/netbox_software/templates/netbox_software/vendor.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/templates/netbox_software/virtualmachinesoftware.html` & `netbox_software-0.1.7/netbox_software/templates/netbox_software/virtualmachinesoftware.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html` & `netbox_software-0.1.7/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html` & `netbox_software-0.1.7/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 {% load helpers %}
 
 <div class="card">
 <h5 class="card-header">
-    ПО виртуальных машин
+    ПО виртуальных машин {% if virtual_machine_software %}
+  <a href="{% url 'plugins:netbox_software:virtualmachinesoftware_list' %}?virtual_machine={{ object.pk }}">
+   (всего: {{ soft_count }})
+  </a>
+  {% endif %}
 </h5>
 <div class="card-body">
 {% if virtual_machine_software %}
     <table class="table table-hover">
         <tr>
             <th>Название</th>
-            <th>Разработчик</th>
             <th>Версия</th>
-            <th>Тип</th>
             <th></th>
         </tr>
         {% for software in virtual_machine_software %}
         <tr>
             <td>
                 {{ software.name }}
             </td>
-            <td>{{ software.vendor }}</td>
             <td>{{ software.version }}</td>
-            <td>{% badge software.get_software_type_display bg_color=software.get_software_type_color %}</td>
             <td class="text-end noprint">
                 <a href="{% url 'plugins:netbox_software:virtualmachinesoftware' pk=software.pk %}"
                    class="btn btn-primary btn-sm lh-1" title="Просмотреть">
                     <i class="mdi mdi-book" aria-hidden="true"></i>
                   </a>
                   <a href="{% url 'plugins:netbox_software:virtualmachinesoftware_edit' pk=software.pk %}?return_url=
                   {% url 'virtualization:virtualmachine' pk=object.pk %}" class="btn btn-warning btn-sm lh-1"
@@ -42,14 +42,20 @@
     {% else %}
         <div class="text-muted">
             Нет
         </div>
     {% endif %}
     </div>
         <div class="card-footer text-end noprint">
-            <a href="{% url 'plugins:netbox_software:virtualmachinesoftware_add' %}?virtualmachine={{ object.pk }}&
+            <a href="{% url 'plugins:netbox_software:virtualmachinesoftware_add' %}?virtual_machine={{ object.pk }}&
             return_url={% url 'virtualization:virtualmachine' pk=object.pk %}" class="btn btn-primary btn-sm">
               <i class="mdi mdi-plus-thick" aria-hidden="true"></i>
                 Добавить ПО
             </a>
+            {% if virtual_machine_software %}
+            <a href="{% url 'plugins:netbox_software:virtualmachinesoftware_list' %}?virtual_machine={{ object.pk }}"
+               class="btn btn-primary btn-sm">
+                  Все ПО хоста
+            </a>
+            {% endif %}
         </div>
 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 {% load helpers %}
-** ÐÐ Ð²Ð¸ÑÑÑÐ°Ð»ÑÐ½ÑÑ Ð¼Ð°ÑÐ¸Ð½ **
+** ÐÐ Ð²Ð¸ÑÑÑÐ°Ð»ÑÐ½ÑÑ Ð¼Ð°ÑÐ¸Ð½ {% if virtual_machine_software %}
+(Ð²ÑÐµÐ³Ð¾:_{{_soft_count_}}) {% endif %} **
 {% if virtual_machine_software %}
-ÐÐ°Ð·Ð²�Ð Ð°Ð·ÑÐ°Ð�ÐÐµÑÑ�Ð¢Ð¸Ð¿
-                                        {                {% badge
-{{ software.name {{ software.vendor }}  {                software.get_software_type_display
-}}                                      software.version bg_color=software.get_software_type_color
-                                        }}               %}
+ÐÐ°Ð·Ð²Ð°ÐÐµÑÑÐ¸Ñ
+{{ software.name }} {{ software.version }}
 {% else %}
 ÐÐµÑ
 {% endif %}
  ÐÐ¾Ð±Ð°Ð²Ð¸ÑÑ_ÐÐ
+ {% if virtual_machine_software %} ÐÑÐµ_ÐÐ_ÑÐ¾ÑÑÐ° {% endif %}
```

### Comparing `netbox_software-0.1.6/netbox_software/urls.py` & `netbox_software-0.1.7/netbox_software/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/netbox_software/views.py` & `netbox_software-0.1.7/netbox_software/views.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.6/PKG-INFO` & `netbox_software-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-software
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: izakharov
 Author-email: ilya.zakharov@domrf.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

