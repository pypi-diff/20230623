# Comparing `tmp/drf-excel-2.3.0.tar.gz` & `tmp/drf-excel-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-excel-2.3.0.tar", last modified: Mon Feb  6 19:32:28 2023, max compression
+gzip compressed data, was "/var/www-dev/tallen/drf-excel/dist/.tmp-is1kagv4/drf-excel-2.4.0.tar", last modified: Fri Jun 23 12:18:42 2023, max compression
```

## Comparing `drf-excel-2.3.0.tar` & `drf-excel-2.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-02-06 19:32:28.889753 drf-excel-2.3.0/
--rw-------   0 tallen   (86646) wrds     (60359)      581 2022-01-19 22:05:39.000000 drf-excel-2.3.0/.gitignore
--rw-------   0 tallen   (86646) wrds     (60359)     1582 2022-01-19 22:05:39.000000 drf-excel-2.3.0/LICENSE
--rw-------   0 tallen   (86646) wrds     (60359)    15477 2023-02-06 19:32:28.889753 drf-excel-2.3.0/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)    11553 2023-02-06 19:19:45.000000 drf-excel-2.3.0/README.md
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-02-06 19:32:28.887753 drf-excel-2.3.0/drf_excel/
--rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:05:39.000000 drf-excel-2.3.0/drf_excel/__init__.py
--rw-------   0 tallen   (86646) wrds     (60359)     6236 2023-02-06 19:19:45.000000 drf-excel-2.3.0/drf_excel/fields.py
--rw-------   0 tallen   (86646) wrds     (60359)     1174 2022-09-30 13:44:06.000000 drf-excel-2.3.0/drf_excel/mixins.py
--rw-------   0 tallen   (86646) wrds     (60359)    14077 2023-02-06 19:19:45.000000 drf-excel-2.3.0/drf_excel/renderers.py
--rw-------   0 tallen   (86646) wrds     (60359)     3520 2023-02-06 19:19:45.000000 drf-excel-2.3.0/drf_excel/utilities.py
-drwx------   0 tallen   (86646) wrds     (60359)        0 2023-02-06 19:32:28.889753 drf-excel-2.3.0/drf_excel.egg-info/
--rw-------   0 tallen   (86646) wrds     (60359)    15477 2023-02-06 19:32:28.000000 drf-excel-2.3.0/drf_excel.egg-info/PKG-INFO
--rw-------   0 tallen   (86646) wrds     (60359)      341 2023-02-06 19:32:28.000000 drf-excel-2.3.0/drf_excel.egg-info/SOURCES.txt
--rw-------   0 tallen   (86646) wrds     (60359)        1 2023-02-06 19:32:28.000000 drf-excel-2.3.0/drf_excel.egg-info/dependency_links.txt
--rw-------   0 tallen   (86646) wrds     (60359)        1 2022-02-18 19:28:21.000000 drf-excel-2.3.0/drf_excel.egg-info/not-zip-safe
--rw-------   0 tallen   (86646) wrds     (60359)       40 2023-02-06 19:32:28.000000 drf-excel-2.3.0/drf_excel.egg-info/requires.txt
--rw-------   0 tallen   (86646) wrds     (60359)       10 2023-02-06 19:32:28.000000 drf-excel-2.3.0/drf_excel.egg-info/top_level.txt
--rw-------   0 tallen   (86646) wrds     (60359)       38 2023-02-06 19:32:28.889753 drf-excel-2.3.0/setup.cfg
--rw-------   0 tallen   (86646) wrds     (60359)     1541 2022-09-30 13:53:21.000000 drf-excel-2.3.0/setup.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-06-23 12:18:42.467416 drf-excel-2.4.0/
+-rw-------   0 tallen   (86646) wrds     (60359)      581 2022-01-19 22:05:39.000000 drf-excel-2.4.0/.gitignore
+-rw-------   0 tallen   (86646) wrds     (60359)     1582 2022-01-19 22:05:39.000000 drf-excel-2.4.0/LICENSE
+-rw-------   0 tallen   (86646) wrds     (60359)    12704 2023-06-23 12:18:42.466416 drf-excel-2.4.0/PKG-INFO
+-rw-------   0 tallen   (86646) wrds     (60359)    11553 2023-02-06 19:19:45.000000 drf-excel-2.4.0/README.md
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-06-23 12:18:42.465416 drf-excel-2.4.0/drf_excel/
+-rw-------   0 tallen   (86646) wrds     (60359)        0 2022-01-19 22:05:39.000000 drf-excel-2.4.0/drf_excel/__init__.py
+-rw-------   0 tallen   (86646) wrds     (60359)     6236 2023-02-06 19:19:45.000000 drf-excel-2.4.0/drf_excel/fields.py
+-rw-------   0 tallen   (86646) wrds     (60359)     1174 2022-09-30 13:44:06.000000 drf-excel-2.4.0/drf_excel/mixins.py
+-rw-------   0 tallen   (86646) wrds     (60359)    14603 2023-06-23 11:54:49.000000 drf-excel-2.4.0/drf_excel/renderers.py
+-rw-------   0 tallen   (86646) wrds     (60359)     3520 2023-02-06 19:19:45.000000 drf-excel-2.4.0/drf_excel/utilities.py
+drwx------   0 tallen   (86646) wrds     (60359)        0 2023-06-23 12:18:42.466416 drf-excel-2.4.0/drf_excel.egg-info/
+-rw-------   0 tallen   (86646) wrds     (60359)    12704 2023-06-23 12:18:42.000000 drf-excel-2.4.0/drf_excel.egg-info/PKG-INFO
+-rw-------   0 tallen   (86646) wrds     (60359)      341 2023-06-23 12:18:42.000000 drf-excel-2.4.0/drf_excel.egg-info/SOURCES.txt
+-rw-------   0 tallen   (86646) wrds     (60359)        1 2023-06-23 12:18:42.000000 drf-excel-2.4.0/drf_excel.egg-info/dependency_links.txt
+-rw-------   0 tallen   (86646) wrds     (60359)        1 2022-02-18 19:28:21.000000 drf-excel-2.4.0/drf_excel.egg-info/not-zip-safe
+-rw-------   0 tallen   (86646) wrds     (60359)       40 2023-06-23 12:18:42.000000 drf-excel-2.4.0/drf_excel.egg-info/requires.txt
+-rw-------   0 tallen   (86646) wrds     (60359)       10 2023-06-23 12:18:42.000000 drf-excel-2.4.0/drf_excel.egg-info/top_level.txt
+-rw-------   0 tallen   (86646) wrds     (60359)       38 2023-06-23 12:18:42.467416 drf-excel-2.4.0/setup.cfg
+-rw-------   0 tallen   (86646) wrds     (60359)     1507 2023-06-23 11:49:11.000000 drf-excel-2.4.0/setup.py
```

### Comparing `drf-excel-2.3.0/.gitignore` & `drf-excel-2.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `drf-excel-2.3.0/LICENSE` & `drf-excel-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-excel-2.3.0/PKG-INFO` & `drf-excel-2.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,369 +1,367 @@
 Metadata-Version: 2.1
 Name: drf-excel
-Version: 2.3.0
+Version: 2.4.0
 Summary: Django REST Framework renderer for Excel spreadsheet (xlsx) files.
 Home-page: https://github.com/wharton/drf-excel
 Author: Timothy Allen
 Author-email: tallen@wharton.upenn.edu
-License: UNKNOWN
-Description: # DRF Excel: Django REST Framework Excel Spreadsheet (xlsx) Renderer
-        
-        `drf-excel` provides an Excel spreadsheet (xlsx) renderer for Django REST Framework. It uses OpenPyXL to create the spreadsheet and provide the file to the end user.
-        
-        ## Requirements
-        
-        We aim to support Django's [currently supported versions](https://www.djangoproject.com/download/), as well as:
-        
-        * Django REST Framework >= 3.14
-        * OpenPyXL >= 2.4
-        
-        ## Installation
-        
-        ```bash
-        pip install drf-excel
-        ```
-        
-        Then add the following to your `REST_FRAMEWORK` settings:
-        
-        ```python
-        REST_FRAMEWORK = {
-            ...
-        
-            'DEFAULT_RENDERER_CLASSES': (
-                'rest_framework.renderers.JSONRenderer',
-                'rest_framework.renderers.BrowsableAPIRenderer',
-                'drf_excel.renderers.XLSXRenderer',
-            ),
-        }
-        ```
-        
-        To avoid having a file streamed without a filename (which the browser will often default to the filename "download", with no extension), we need to use a mixin to override the `Content-Disposition` header. If no `filename` is provided, it will default to `export.xlsx`. For example:
-        
-        ```python
-        from rest_framework.viewsets import ReadOnlyModelViewSet
-        from drf_excel.mixins import XLSXFileMixin
-        from drf_excel.renderers import XLSXRenderer
-        
-        from .models import MyExampleModel
-        from .serializers import MyExampleSerializer
-        
-        class MyExampleViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-            queryset = MyExampleModel.objects.all()
-            serializer_class = MyExampleSerializer
-            renderer_classes = (XLSXRenderer,)
-            filename = 'my_export.xlsx'
-        ```
-        
-        The `XLSXFileMixin` also provides a `get_filename()` method which can be overridden, if you prefer to provide a filename programmatically instead of the `filename` attribute.
-        
-        ## Upgrading to 2.0.0
-        
-        To upgrade to `drf_excel` 2.0.0 from `drf_renderer_xlsx`, update your import paths:
-        
-        * `from drf_renderer_xlsx.mixins import XLSXFileMixin` becomes `from drf_excel.mixins import XLSXFileMixin`.
-        * `drf_renderer_xlsx.renderers.XLSXRenderer` becomes `drf_excel.renderers.XLSXRenderer`.
-        * `xlsx_date_format_mappings` has been removed in favor of `column_data_styles` which provides more flexibility
-        
-        ## Configuring Styles 
-        
-        Styles can be added to your worksheet header, column header row, body and column data from view attributes `header`, `column_header`, `body`, `column_data_styles`. Any arguments from [the OpenPyXL package](https://openpyxl.readthedocs.io/en/stable/styles.html) can be used for font, alignment, fill and border_side (border will always be all side of cell).
-        
-        If provided, column data styles will override body style
-        
-        Note that column data styles can take an extra 'format' argument that follows [openpyxl formats](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/styles/numbers.html).
-        
-        ```python
-        class MyExampleViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-            queryset = MyExampleModel.objects.all()
-            serializer_class = MyExampleSerializer
-            renderer_classes = (XLSXRenderer,)
-        
-            column_header = {
-                'titles': [
-                    "Column_1_name",
-                    "Column_2_name",
-                    "Column_3_name",
-                ],
-                'column_width': [17, 30, 17],
-                'height': 25,
-                'style': {
-                    'fill': {
-                        'fill_type': 'solid',
-                        'start_color': 'FFCCFFCC',
-                    },
-                    'alignment': {
-                        'horizontal': 'center',
-                        'vertical': 'center',
-                        'wrapText': True,
-                        'shrink_to_fit': True,
-                    },
-                    'border_side': {
-                        'border_style': 'thin',
-                        'color': 'FF000000',
-                    },
-                    'font': {
-                        'name': 'Arial',
-                        'size': 14,
-                        'bold': True,
-                        'color': 'FF000000',
-                    },
-                },
-            }
-            body = {
-                'style': {
-                    'fill': {
-                        'fill_type': 'solid',
-                        'start_color': 'FFCCFFCC',
-                    },
-                    'alignment': {
-                        'horizontal': 'center',
-                        'vertical': 'center',
-                        'wrapText': True,
-                        'shrink_to_fit': True,
-                    },
-                    'border_side': {
-                        'border_style': 'thin',
-                        'color': 'FF000000',
-                    },
-                    'font': {
-                        'name': 'Arial',
-                        'size': 14,
-                        'bold': False,
-                        'color': 'FF000000',
-                    }
-                },
-                'height': 40,
-            }
-            column_data_styles = {
-                'distance': {
-                    'alignment': {
-                        'horizontal': 'right',
-                        'vertical': 'top',
-                    },
-                    'format': '0.00E+00'
-                },
-                'created_at': {
-                    'format': 'd.m.y h:mm',
-                }
-            }
-        ```
-        
-        You can dynamically generate style attributes in methods `get_body`, `get_header`, `get_column_header`, `get_column_data_styles`.
-        
-        ```python
-        def get_header(self):
-            start_time, end_time = parse_times(request=self.request)
-            datetime_format = "%H:%M:%S %d.%m.%Y"
-            return {
-                'tab_title': 'MyReport', # title of tab/workbook
-                'use_header': True,  # show the header_title 
-                'header_title': 'Report from {} to {}'.format(
-                    start_time.strftime(datetime_format),
-                    end_time.strftime(datetime_format),
-                ),
-                'height': 45,
-                'img': 'app/images/MyLogo.png',
-                'style': {
-                    'fill': {
-                        'fill_type': 'solid',
-                        'start_color': 'FFFFFFFF',
-                    },
-                    'alignment': {
-                        'horizontal': 'center',
-                        'vertical': 'center',
-                        'wrapText': True,
-                        'shrink_to_fit': True,
-                    },
-                    'border_side': {
-                        'border_style': 'thin',
-                        'color': 'FF000000',
-                    },
-                    'font': {
-                        'name': 'Arial',
-                        'size': 16,
-                        'bold': True,
-                        'color': 'FF000000',
-                    }
-                }
-            }
-        ```
-        
-        Also, you can add the `row_color` field to your serializer and fill body rows.
-        
-        ```python
-        class ExampleSerializer(serializers.Serializer):
-            row_color = serializers.SerializerMethodField()
-        
-            def get_row_color(self, instance):
-                color_map = {'w': 'FFFFFFCC', 'a': 'FFFFCCCC'}
-                return color_map.get(instance.alarm_level, 'FFFFFFFF')
-        ```
-        
-        ## Configuring Sheet View Options
-        
-        View options follow [openpyxl sheet view options](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/worksheet/views.html#SheetView)
-        
-        They can be set in the view as a property `sheet_view_options`:
-        
-        ```python
-        class MyExampleViewSet(serializers.Serializer):
-            sheet_view_options = {
-                'rightToLeft': True, 
-                'showGridLines': False
-            }
-        ```
-        
-        or using method `get_sheet_view_options`:
-        
-        ```python
-        class MyExampleViewSet(serializers.Serializer):
-            
-            def get_sheet_view_options(self):
-                return {
-                    'rightToLeft': True, 
-                    'showGridLines': False
-                }
-        ```
-        ## Controlling XLSX headers and values
-        
-        ### Use Serializer Field labels as header names
-        
-        By default, headers will use the same 'names' as they are returned by the API. This can be changed by setting `xlsx_use_labels = True` inside your API View. 
-        
-        Instead of using the field names, the export will use the labels as they are defined inside your Serializer. A serializer field defined as `title = serializers.CharField(label=_("Some title"))` would return `Some title` instead of `title`, also supporting translations. If no label is set, it will fall back to using `title`.
-        
-        ### Ignore fields
-        
-        By default, all fields are exported, but you might want to exclude some fields from your export. To do so, you can set an array with fields you want to exclude: `xlsx_ignore_headers = [<excluded fields>]`.
-        
-        This also works with nested fields, separated with a dot (i.e. `icon.url`).
-        
-        ### Date/time and number formatting
-        Formatting for cells follows [openpyxl formats](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/styles/numbers.html).
-        
-        To set global formats, set the following variables in `settings.py`:
-        
-        ```python
-        # Date formats
-        DRF_EXCEL_DATETIME_FORMAT = 'mm-dd-yy h:mm AM/PM'
-        DRF_EXCEL_DATE_FORMAT = 'mm-dd-yy'
-        DRF_EXCEL_TIME_FORMAT = 'h:mm AM/PM'
-        
-        # Number formats
-        DRF_EXCEL_INTEGER_FORMAT = '0%'
-        DRF_EXCEL_DECIMAL_FORMAT = '0.00E+00'
-        ```
-        
-        ### Name boolean values
-        
-        `True` and `False` as values for boolean fields are not always the best representation and don't support translation. 
-        
-        This can be controlled with in you API view with `xlsx_boolean_labels`. 
-        
-        ```
-        xlsx_boolean_labels = {True: _('Yes'), False: _('No')}
-        ```
-        
-        will replace `True` with `Yes` and `False` with `No`.
-        
-        This can also be set globally in settings.py:
-        
-        ```
-        DRF_EXCEL_BOOLEAN_DISPLAY = {True: _('Yes'), False: _('No')}
-        ```
-        
-        
-        ### Custom columns
-        
-        You might find yourself explicitly returning a dict in your API response and would like to use its data to display additional columns. This can be done by passing `xlsx_custom_cols`.
-        
-        ```python
-        xlsx_custom_cols = {
-            'my_custom_col.val1.title': {
-                'label': 'Custom column!',
-                'formatter': custom_value_formatter
-            }
-        }
-        
-        ### Example function:
-        def custom_value_formatter(val):
-            return val + '!!!'
-        
-        ### Example response:
-        { 
-            results: [
-                {
-                    title: 'XLSX renderer',
-                    url: 'https://github.com/wharton/drf-excel'
-                    returned_dict: {
-                        val1: {
-                            title: 'Sometimes'
-                        },
-                        val2: {
-                            title: 'There is no way around'
-                        }
-                    }
-                }
-            ]
-        }
-        ```
-        
-        When no `label` is passed, `drf-excel` will display the key name in the header.
-        
-        `formatter` is also optional and accepts a function, which will then receive the value it is mapped to (it would receive "Sometimes" and return "Sometimes!!!" in our example).
-        
-        ### Custom mappings
-        
-        Assuming you have a field that returns a `dict` instead of a simple `str`, you might not want to return the whole object but only a value of it. Let's say `status` returns `{ value: 1, display: 'Active' }`. To return the `display` value in the `status` column, we can do this:
-        
-        ```python
-        xlsx_custom_mappings = {
-            'status': 'display'
-        }
-        ```
-        
-        A more common case is that you want to change how a value is formatted. `xlsx_custom_mappings` also takes functions as values. Assuming we have a field `description`, and for some strange reason want to reverse the text, we can do this:
-        
-        ```python
-        def reverse_text(val):
-            return val[::-1]
-        
-        xlsx_custom_mappings = {
-            'description': reverse_text
-        }
-        ```
-        
-        ## Release Notes and Contributors
-        
-        * [Release notes](https://github.com/wharton/drf-excel/releases)
-        * [Our wonderful contributors](https://github.com/wharton/drf-excel/graphs/contributors)
-        
-        ## Maintainers
-        
-        * [Timothy Allen](https://github.com/FlipperPA) at [The Wharton School](https://github.com/wharton)
-        * [Thomas Willems](https://github.com/willtho89)
-        * [Mathieu Rampant](https://github.com/rptmat57)
-        
-        This package was created by the staff of [Wharton Research Data Services](https://wrds.wharton.upenn.edu/). We are thrilled that [The Wharton School](https://www.wharton.upenn.edu/) allows us a certain amount of time to contribute to open-source projects. We add features as they are necessary for our projects, and try to keep up with Issues and Pull Requests as best we can. Due to constraints of time (our full time jobs!), Feature Requests without a Pull Request may not be implemented, but we are always open to new ideas and grateful for contributions and our users.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 4
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DRF Excel: Django REST Framework Excel Spreadsheet (xlsx) Renderer
+
+`drf-excel` provides an Excel spreadsheet (xlsx) renderer for Django REST Framework. It uses OpenPyXL to create the spreadsheet and provide the file to the end user.
+
+## Requirements
+
+We aim to support Django's [currently supported versions](https://www.djangoproject.com/download/), as well as:
+
+* Django REST Framework >= 3.14
+* OpenPyXL >= 2.4
+
+## Installation
+
+```bash
+pip install drf-excel
+```
+
+Then add the following to your `REST_FRAMEWORK` settings:
+
+```python
+REST_FRAMEWORK = {
+    ...
+
+    'DEFAULT_RENDERER_CLASSES': (
+        'rest_framework.renderers.JSONRenderer',
+        'rest_framework.renderers.BrowsableAPIRenderer',
+        'drf_excel.renderers.XLSXRenderer',
+    ),
+}
+```
+
+To avoid having a file streamed without a filename (which the browser will often default to the filename "download", with no extension), we need to use a mixin to override the `Content-Disposition` header. If no `filename` is provided, it will default to `export.xlsx`. For example:
+
+```python
+from rest_framework.viewsets import ReadOnlyModelViewSet
+from drf_excel.mixins import XLSXFileMixin
+from drf_excel.renderers import XLSXRenderer
+
+from .models import MyExampleModel
+from .serializers import MyExampleSerializer
+
+class MyExampleViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
+    queryset = MyExampleModel.objects.all()
+    serializer_class = MyExampleSerializer
+    renderer_classes = (XLSXRenderer,)
+    filename = 'my_export.xlsx'
+```
+
+The `XLSXFileMixin` also provides a `get_filename()` method which can be overridden, if you prefer to provide a filename programmatically instead of the `filename` attribute.
+
+## Upgrading to 2.0.0
+
+To upgrade to `drf_excel` 2.0.0 from `drf_renderer_xlsx`, update your import paths:
+
+* `from drf_renderer_xlsx.mixins import XLSXFileMixin` becomes `from drf_excel.mixins import XLSXFileMixin`.
+* `drf_renderer_xlsx.renderers.XLSXRenderer` becomes `drf_excel.renderers.XLSXRenderer`.
+* `xlsx_date_format_mappings` has been removed in favor of `column_data_styles` which provides more flexibility
+
+## Configuring Styles 
+
+Styles can be added to your worksheet header, column header row, body and column data from view attributes `header`, `column_header`, `body`, `column_data_styles`. Any arguments from [the OpenPyXL package](https://openpyxl.readthedocs.io/en/stable/styles.html) can be used for font, alignment, fill and border_side (border will always be all side of cell).
+
+If provided, column data styles will override body style
+
+Note that column data styles can take an extra 'format' argument that follows [openpyxl formats](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/styles/numbers.html).
+
+```python
+class MyExampleViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
+    queryset = MyExampleModel.objects.all()
+    serializer_class = MyExampleSerializer
+    renderer_classes = (XLSXRenderer,)
+
+    column_header = {
+        'titles': [
+            "Column_1_name",
+            "Column_2_name",
+            "Column_3_name",
+        ],
+        'column_width': [17, 30, 17],
+        'height': 25,
+        'style': {
+            'fill': {
+                'fill_type': 'solid',
+                'start_color': 'FFCCFFCC',
+            },
+            'alignment': {
+                'horizontal': 'center',
+                'vertical': 'center',
+                'wrapText': True,
+                'shrink_to_fit': True,
+            },
+            'border_side': {
+                'border_style': 'thin',
+                'color': 'FF000000',
+            },
+            'font': {
+                'name': 'Arial',
+                'size': 14,
+                'bold': True,
+                'color': 'FF000000',
+            },
+        },
+    }
+    body = {
+        'style': {
+            'fill': {
+                'fill_type': 'solid',
+                'start_color': 'FFCCFFCC',
+            },
+            'alignment': {
+                'horizontal': 'center',
+                'vertical': 'center',
+                'wrapText': True,
+                'shrink_to_fit': True,
+            },
+            'border_side': {
+                'border_style': 'thin',
+                'color': 'FF000000',
+            },
+            'font': {
+                'name': 'Arial',
+                'size': 14,
+                'bold': False,
+                'color': 'FF000000',
+            }
+        },
+        'height': 40,
+    }
+    column_data_styles = {
+        'distance': {
+            'alignment': {
+                'horizontal': 'right',
+                'vertical': 'top',
+            },
+            'format': '0.00E+00'
+        },
+        'created_at': {
+            'format': 'd.m.y h:mm',
+        }
+    }
+```
+
+You can dynamically generate style attributes in methods `get_body`, `get_header`, `get_column_header`, `get_column_data_styles`.
+
+```python
+def get_header(self):
+    start_time, end_time = parse_times(request=self.request)
+    datetime_format = "%H:%M:%S %d.%m.%Y"
+    return {
+        'tab_title': 'MyReport', # title of tab/workbook
+        'use_header': True,  # show the header_title 
+        'header_title': 'Report from {} to {}'.format(
+            start_time.strftime(datetime_format),
+            end_time.strftime(datetime_format),
+        ),
+        'height': 45,
+        'img': 'app/images/MyLogo.png',
+        'style': {
+            'fill': {
+                'fill_type': 'solid',
+                'start_color': 'FFFFFFFF',
+            },
+            'alignment': {
+                'horizontal': 'center',
+                'vertical': 'center',
+                'wrapText': True,
+                'shrink_to_fit': True,
+            },
+            'border_side': {
+                'border_style': 'thin',
+                'color': 'FF000000',
+            },
+            'font': {
+                'name': 'Arial',
+                'size': 16,
+                'bold': True,
+                'color': 'FF000000',
+            }
+        }
+    }
+```
+
+Also, you can add the `row_color` field to your serializer and fill body rows.
+
+```python
+class ExampleSerializer(serializers.Serializer):
+    row_color = serializers.SerializerMethodField()
+
+    def get_row_color(self, instance):
+        color_map = {'w': 'FFFFFFCC', 'a': 'FFFFCCCC'}
+        return color_map.get(instance.alarm_level, 'FFFFFFFF')
+```
+
+## Configuring Sheet View Options
+
+View options follow [openpyxl sheet view options](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/worksheet/views.html#SheetView)
+
+They can be set in the view as a property `sheet_view_options`:
+
+```python
+class MyExampleViewSet(serializers.Serializer):
+    sheet_view_options = {
+        'rightToLeft': True, 
+        'showGridLines': False
+    }
+```
+
+or using method `get_sheet_view_options`:
+
+```python
+class MyExampleViewSet(serializers.Serializer):
+    
+    def get_sheet_view_options(self):
+        return {
+            'rightToLeft': True, 
+            'showGridLines': False
+        }
+```
+## Controlling XLSX headers and values
+
+### Use Serializer Field labels as header names
+
+By default, headers will use the same 'names' as they are returned by the API. This can be changed by setting `xlsx_use_labels = True` inside your API View. 
+
+Instead of using the field names, the export will use the labels as they are defined inside your Serializer. A serializer field defined as `title = serializers.CharField(label=_("Some title"))` would return `Some title` instead of `title`, also supporting translations. If no label is set, it will fall back to using `title`.
+
+### Ignore fields
+
+By default, all fields are exported, but you might want to exclude some fields from your export. To do so, you can set an array with fields you want to exclude: `xlsx_ignore_headers = [<excluded fields>]`.
+
+This also works with nested fields, separated with a dot (i.e. `icon.url`).
+
+### Date/time and number formatting
+Formatting for cells follows [openpyxl formats](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/styles/numbers.html).
+
+To set global formats, set the following variables in `settings.py`:
+
+```python
+# Date formats
+DRF_EXCEL_DATETIME_FORMAT = 'mm-dd-yy h:mm AM/PM'
+DRF_EXCEL_DATE_FORMAT = 'mm-dd-yy'
+DRF_EXCEL_TIME_FORMAT = 'h:mm AM/PM'
+
+# Number formats
+DRF_EXCEL_INTEGER_FORMAT = '0%'
+DRF_EXCEL_DECIMAL_FORMAT = '0.00E+00'
+```
+
+### Name boolean values
+
+`True` and `False` as values for boolean fields are not always the best representation and don't support translation. 
+
+This can be controlled with in you API view with `xlsx_boolean_labels`. 
+
+```
+xlsx_boolean_labels = {True: _('Yes'), False: _('No')}
+```
+
+will replace `True` with `Yes` and `False` with `No`.
+
+This can also be set globally in settings.py:
+
+```
+DRF_EXCEL_BOOLEAN_DISPLAY = {True: _('Yes'), False: _('No')}
+```
+
+
+### Custom columns
+
+You might find yourself explicitly returning a dict in your API response and would like to use its data to display additional columns. This can be done by passing `xlsx_custom_cols`.
+
+```python
+xlsx_custom_cols = {
+    'my_custom_col.val1.title': {
+        'label': 'Custom column!',
+        'formatter': custom_value_formatter
+    }
+}
+
+### Example function:
+def custom_value_formatter(val):
+    return val + '!!!'
+
+### Example response:
+{ 
+    results: [
+        {
+            title: 'XLSX renderer',
+            url: 'https://github.com/wharton/drf-excel'
+            returned_dict: {
+                val1: {
+                    title: 'Sometimes'
+                },
+                val2: {
+                    title: 'There is no way around'
+                }
+            }
+        }
+    ]
+}
+```
+
+When no `label` is passed, `drf-excel` will display the key name in the header.
+
+`formatter` is also optional and accepts a function, which will then receive the value it is mapped to (it would receive "Sometimes" and return "Sometimes!!!" in our example).
+
+### Custom mappings
+
+Assuming you have a field that returns a `dict` instead of a simple `str`, you might not want to return the whole object but only a value of it. Let's say `status` returns `{ value: 1, display: 'Active' }`. To return the `display` value in the `status` column, we can do this:
+
+```python
+xlsx_custom_mappings = {
+    'status': 'display'
+}
+```
+
+A more common case is that you want to change how a value is formatted. `xlsx_custom_mappings` also takes functions as values. Assuming we have a field `description`, and for some strange reason want to reverse the text, we can do this:
+
+```python
+def reverse_text(val):
+    return val[::-1]
+
+xlsx_custom_mappings = {
+    'description': reverse_text
+}
+```
+
+## Release Notes and Contributors
+
+* [Release notes](https://github.com/wharton/drf-excel/releases)
+* [Our wonderful contributors](https://github.com/wharton/drf-excel/graphs/contributors)
+
+## Maintainers
+
+* [Timothy Allen](https://github.com/FlipperPA) at [The Wharton School](https://github.com/wharton)
+* [Thomas Willems](https://github.com/willtho89)
+* [Mathieu Rampant](https://github.com/rptmat57)
+
+This package was created by the staff of [Wharton Research Data Services](https://wrds.wharton.upenn.edu/). We are thrilled that [The Wharton School](https://www.wharton.upenn.edu/) allows us a certain amount of time to contribute to open-source projects. We add features as they are necessary for our projects, and try to keep up with Issues and Pull Requests as best we can. Due to constraints of time (our full time jobs!), Feature Requests without a Pull Request may not be implemented, but we are always open to new ideas and grateful for contributions and our users.
```

### Comparing `drf-excel-2.3.0/README.md` & `drf-excel-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `drf-excel-2.3.0/drf_excel/fields.py` & `drf-excel-2.4.0/drf_excel/fields.py`

 * *Files identical despite different names*

### Comparing `drf-excel-2.3.0/drf_excel/mixins.py` & `drf-excel-2.4.0/drf_excel/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-excel-2.3.0/drf_excel/renderers.py` & `drf-excel-2.4.0/drf_excel/renderers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from collections.abc import Iterable, MutableMapping
-from tempfile import NamedTemporaryFile
+from tempfile import TemporaryFile
 from typing import Dict
 
+from django.utils.functional import Promise
 from openpyxl import Workbook
 from openpyxl.drawing.image import Image
 from openpyxl.styles import PatternFill
 from openpyxl.utils import get_column_letter
 from openpyxl.worksheet.views import SheetView
 from openpyxl.writer.excel import save_workbook
 from rest_framework.fields import (
@@ -90,48 +91,61 @@
         column_count = 0
         row_count = 1
         if use_header:
             row_count += 1
         # Make column headers
         column_titles = column_header.get("titles", [])
 
-        # If we have results, then flatten field
-        # names
+        # If we have results, then flatten field names
         if len(results):
-
             # Set `xlsx_use_labels = True` inside the API View to enable labels.
             use_labels = getattr(drf_view, "xlsx_use_labels", False)
 
             # A list of header keys to ignore in our export
             self.ignore_headers = getattr(drf_view, "xlsx_ignore_headers", [])
 
             # Create a mapping dict named `xlsx_boolean_labels` inside the API View.
             # I.e.: xlsx_boolean_labels: {True: "Yes", False: "No"}
             self.boolean_display = getattr(drf_view, "xlsx_boolean_labels", None)
 
-            # Set dict named column_data_styles with headers as keys and style as value. i.e.
+            # Set dict named column_data_styles with headers as keys and styles as
+            # values, I.e.:
             # column_data_styles = {
             #     'distance': {
             # 	      'fill': {'fill_type': 'solid', 'start_color': 'FFCCFFCC'},
-            #         'alignment': {'horizontal': 'center', 'vertical': 'center', 'wrapText': True, 'shrink_to_fit': True},
+            #         'alignment': {
+            #             'horizontal': 'center',
+            #             'vertical': 'center',
+            #             'wrapText': True, 'shrink_to_fit': True
+            #         },
             # 	      'border_side': {'border_style': 'thin', 'color': 'FF000000'},
-            # 	      'font': {'name': 'Arial', 'size': 14, 'bold': True, 'color': 'FF000000'},
+            # 	      'font': {
+            #             'name': 'Arial',
+            #             'size': 14,
+            #             'bold': True,
+            #             'color': 'FF000000'
+            #         },
             # 	      'format': '0.00E+00'
             # 	  },
             # }
             self.column_data_styles = get_attribute(
                 drf_view, "column_data_styles", dict()
             )
 
             # Set dict of additional columns. Can be useful when wanting to add columns
             # that don't exist in the API response. For example, you could want to
             # show values of a dict in individual cols. Takes key, an optional label
             # and value than can be callable
             # Example:
-            # {"Additional Col": { label: "Something (optional)", formatter: my_function }}
+            # {
+            #     "Additional Col": {
+            #         label: "Something (optional)",
+            #         formatter: my_function
+            #     }
+            # }
             self.custom_cols = getattr(drf_view, "xlsx_custom_cols", dict())
 
             # Map a specific key to a column (I.e. if the field returns a json) or pass
             # a function to format the value
             # Example with key:
             # {"custom_choice": "display"}, showing 'display' in the
             # 'custom_choice' col
@@ -211,20 +225,18 @@
         # }
         self.sheet_view_options = get_attribute(drf_view, "sheet_view_options", dict())
         self.ws.views.sheetView[0] = SheetView(**self.sheet_view_options)
 
         return self._save_virtual_workbook(wb)
 
     def _save_virtual_workbook(self, wb):
-        tmp = NamedTemporaryFile()
-        save_workbook(wb, tmp.name)
-
-        tmp.seek(0)
-        virtual_workbook = tmp.read()
-        tmp.close()
+        with TemporaryFile() as tmp:
+            save_workbook(wb, tmp)
+            tmp.seek(0)
+            virtual_workbook = tmp.read()        
 
         return virtual_workbook
 
     def _check_validation_data(self, data):
         detail_key = "detail"
         return detail_key not in data
 
@@ -299,68 +311,81 @@
 
         return _header_dict
 
     def _flatten_data(self, data, parent_key="", key_sep=".") -> Dict[str, XLSXField]:
         items = []
         for k, v in data.items():
             new_key = f"{parent_key}{key_sep}{k}" if parent_key else k
+
+            # Trap Promise instances for when _lazy is used
+            if isinstance(v, Promise):
+                v = v.__class__._proxy____cast(v)
+
             if isinstance(v, MutableMapping):
                 items.extend(self._flatten_data(v, new_key, key_sep=key_sep).items())
             else:
                 xlsx_field = self._drf_to_xlsx_field(key=new_key, value=v)
                 items.append((new_key, xlsx_field))
+
         return dict(items)
 
     def _make_body(self, body, row, row_count):
         column_count = 0
         row_count += 1
         flattened_row = self._flatten_data(row)
+
         for header_key in self.combined_header_dict:
             if header_key == "row_color":
                 continue
             column_count += 1
             field = flattened_row.get(header_key)
             field.cell(self.ws, row_count, column_count) if field else self.ws.cell(
                 row_count, column_count
             )
+
         self.ws.row_dimensions[row_count].height = body.get("height", 40)
+
         if "row_color" in row:
             last_letter = get_column_letter(column_count)
             cell_range = self.ws[
                 f"A{row_count}" : f"{last_letter}{row_count}"
             ]
             fill = PatternFill(fill_type="solid", start_color=row["row_color"])
+
             for r in cell_range:
                 for c in r:
                     c.fill = fill
 
     def _drf_to_xlsx_field(self, key, value) -> XLSXField:
         field = self.fields_dict.get(key)
+
         cell_style = (
             XLSXStyle(self.column_data_styles.get(key))
             if key in self.column_data_styles
             else None
         )
+
         kwargs = {
             "key": key,
             "value": value,
             "field": field,
             "style": self.body_style,
             # Basically using formatter of custom col as a custom mapping
             "mapping": self.custom_cols.get(key, {}).get("formatter")
             or self.custom_mappings.get(key),
             "cell_style": cell_style,
         }
+
         if isinstance(field, BooleanField):
             return XLSXBooleanField(boolean_display=self.boolean_display, **kwargs)
         elif isinstance(field, (IntegerField, FloatField, DecimalField)):
             return XLSXNumberField(**kwargs)
         elif isinstance(field, (DateTimeField, DateField, TimeField)):
-            return XLSXDateField(**kwargs)
-        
+            return XLSXDateField(**kwargs)        
         elif (
             isinstance(field, ListField)
             or isinstance(value, Iterable)
             and not isinstance(value, str)
         ):
             return XLSXListField(list_sep=self.list_sep, **kwargs)
+
         return XLSXField(**kwargs)
```

### Comparing `drf-excel-2.3.0/drf_excel/utilities.py` & `drf-excel-2.4.0/drf_excel/utilities.py`

 * *Files identical despite different names*

### Comparing `drf-excel-2.3.0/drf_excel.egg-info/PKG-INFO` & `drf-excel-2.4.0/drf_excel.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,369 +1,367 @@
 Metadata-Version: 2.1
 Name: drf-excel
-Version: 2.3.0
+Version: 2.4.0
 Summary: Django REST Framework renderer for Excel spreadsheet (xlsx) files.
 Home-page: https://github.com/wharton/drf-excel
 Author: Timothy Allen
 Author-email: tallen@wharton.upenn.edu
-License: UNKNOWN
-Description: # DRF Excel: Django REST Framework Excel Spreadsheet (xlsx) Renderer
-        
-        `drf-excel` provides an Excel spreadsheet (xlsx) renderer for Django REST Framework. It uses OpenPyXL to create the spreadsheet and provide the file to the end user.
-        
-        ## Requirements
-        
-        We aim to support Django's [currently supported versions](https://www.djangoproject.com/download/), as well as:
-        
-        * Django REST Framework >= 3.14
-        * OpenPyXL >= 2.4
-        
-        ## Installation
-        
-        ```bash
-        pip install drf-excel
-        ```
-        
-        Then add the following to your `REST_FRAMEWORK` settings:
-        
-        ```python
-        REST_FRAMEWORK = {
-            ...
-        
-            'DEFAULT_RENDERER_CLASSES': (
-                'rest_framework.renderers.JSONRenderer',
-                'rest_framework.renderers.BrowsableAPIRenderer',
-                'drf_excel.renderers.XLSXRenderer',
-            ),
-        }
-        ```
-        
-        To avoid having a file streamed without a filename (which the browser will often default to the filename "download", with no extension), we need to use a mixin to override the `Content-Disposition` header. If no `filename` is provided, it will default to `export.xlsx`. For example:
-        
-        ```python
-        from rest_framework.viewsets import ReadOnlyModelViewSet
-        from drf_excel.mixins import XLSXFileMixin
-        from drf_excel.renderers import XLSXRenderer
-        
-        from .models import MyExampleModel
-        from .serializers import MyExampleSerializer
-        
-        class MyExampleViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-            queryset = MyExampleModel.objects.all()
-            serializer_class = MyExampleSerializer
-            renderer_classes = (XLSXRenderer,)
-            filename = 'my_export.xlsx'
-        ```
-        
-        The `XLSXFileMixin` also provides a `get_filename()` method which can be overridden, if you prefer to provide a filename programmatically instead of the `filename` attribute.
-        
-        ## Upgrading to 2.0.0
-        
-        To upgrade to `drf_excel` 2.0.0 from `drf_renderer_xlsx`, update your import paths:
-        
-        * `from drf_renderer_xlsx.mixins import XLSXFileMixin` becomes `from drf_excel.mixins import XLSXFileMixin`.
-        * `drf_renderer_xlsx.renderers.XLSXRenderer` becomes `drf_excel.renderers.XLSXRenderer`.
-        * `xlsx_date_format_mappings` has been removed in favor of `column_data_styles` which provides more flexibility
-        
-        ## Configuring Styles 
-        
-        Styles can be added to your worksheet header, column header row, body and column data from view attributes `header`, `column_header`, `body`, `column_data_styles`. Any arguments from [the OpenPyXL package](https://openpyxl.readthedocs.io/en/stable/styles.html) can be used for font, alignment, fill and border_side (border will always be all side of cell).
-        
-        If provided, column data styles will override body style
-        
-        Note that column data styles can take an extra 'format' argument that follows [openpyxl formats](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/styles/numbers.html).
-        
-        ```python
-        class MyExampleViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
-            queryset = MyExampleModel.objects.all()
-            serializer_class = MyExampleSerializer
-            renderer_classes = (XLSXRenderer,)
-        
-            column_header = {
-                'titles': [
-                    "Column_1_name",
-                    "Column_2_name",
-                    "Column_3_name",
-                ],
-                'column_width': [17, 30, 17],
-                'height': 25,
-                'style': {
-                    'fill': {
-                        'fill_type': 'solid',
-                        'start_color': 'FFCCFFCC',
-                    },
-                    'alignment': {
-                        'horizontal': 'center',
-                        'vertical': 'center',
-                        'wrapText': True,
-                        'shrink_to_fit': True,
-                    },
-                    'border_side': {
-                        'border_style': 'thin',
-                        'color': 'FF000000',
-                    },
-                    'font': {
-                        'name': 'Arial',
-                        'size': 14,
-                        'bold': True,
-                        'color': 'FF000000',
-                    },
-                },
-            }
-            body = {
-                'style': {
-                    'fill': {
-                        'fill_type': 'solid',
-                        'start_color': 'FFCCFFCC',
-                    },
-                    'alignment': {
-                        'horizontal': 'center',
-                        'vertical': 'center',
-                        'wrapText': True,
-                        'shrink_to_fit': True,
-                    },
-                    'border_side': {
-                        'border_style': 'thin',
-                        'color': 'FF000000',
-                    },
-                    'font': {
-                        'name': 'Arial',
-                        'size': 14,
-                        'bold': False,
-                        'color': 'FF000000',
-                    }
-                },
-                'height': 40,
-            }
-            column_data_styles = {
-                'distance': {
-                    'alignment': {
-                        'horizontal': 'right',
-                        'vertical': 'top',
-                    },
-                    'format': '0.00E+00'
-                },
-                'created_at': {
-                    'format': 'd.m.y h:mm',
-                }
-            }
-        ```
-        
-        You can dynamically generate style attributes in methods `get_body`, `get_header`, `get_column_header`, `get_column_data_styles`.
-        
-        ```python
-        def get_header(self):
-            start_time, end_time = parse_times(request=self.request)
-            datetime_format = "%H:%M:%S %d.%m.%Y"
-            return {
-                'tab_title': 'MyReport', # title of tab/workbook
-                'use_header': True,  # show the header_title 
-                'header_title': 'Report from {} to {}'.format(
-                    start_time.strftime(datetime_format),
-                    end_time.strftime(datetime_format),
-                ),
-                'height': 45,
-                'img': 'app/images/MyLogo.png',
-                'style': {
-                    'fill': {
-                        'fill_type': 'solid',
-                        'start_color': 'FFFFFFFF',
-                    },
-                    'alignment': {
-                        'horizontal': 'center',
-                        'vertical': 'center',
-                        'wrapText': True,
-                        'shrink_to_fit': True,
-                    },
-                    'border_side': {
-                        'border_style': 'thin',
-                        'color': 'FF000000',
-                    },
-                    'font': {
-                        'name': 'Arial',
-                        'size': 16,
-                        'bold': True,
-                        'color': 'FF000000',
-                    }
-                }
-            }
-        ```
-        
-        Also, you can add the `row_color` field to your serializer and fill body rows.
-        
-        ```python
-        class ExampleSerializer(serializers.Serializer):
-            row_color = serializers.SerializerMethodField()
-        
-            def get_row_color(self, instance):
-                color_map = {'w': 'FFFFFFCC', 'a': 'FFFFCCCC'}
-                return color_map.get(instance.alarm_level, 'FFFFFFFF')
-        ```
-        
-        ## Configuring Sheet View Options
-        
-        View options follow [openpyxl sheet view options](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/worksheet/views.html#SheetView)
-        
-        They can be set in the view as a property `sheet_view_options`:
-        
-        ```python
-        class MyExampleViewSet(serializers.Serializer):
-            sheet_view_options = {
-                'rightToLeft': True, 
-                'showGridLines': False
-            }
-        ```
-        
-        or using method `get_sheet_view_options`:
-        
-        ```python
-        class MyExampleViewSet(serializers.Serializer):
-            
-            def get_sheet_view_options(self):
-                return {
-                    'rightToLeft': True, 
-                    'showGridLines': False
-                }
-        ```
-        ## Controlling XLSX headers and values
-        
-        ### Use Serializer Field labels as header names
-        
-        By default, headers will use the same 'names' as they are returned by the API. This can be changed by setting `xlsx_use_labels = True` inside your API View. 
-        
-        Instead of using the field names, the export will use the labels as they are defined inside your Serializer. A serializer field defined as `title = serializers.CharField(label=_("Some title"))` would return `Some title` instead of `title`, also supporting translations. If no label is set, it will fall back to using `title`.
-        
-        ### Ignore fields
-        
-        By default, all fields are exported, but you might want to exclude some fields from your export. To do so, you can set an array with fields you want to exclude: `xlsx_ignore_headers = [<excluded fields>]`.
-        
-        This also works with nested fields, separated with a dot (i.e. `icon.url`).
-        
-        ### Date/time and number formatting
-        Formatting for cells follows [openpyxl formats](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/styles/numbers.html).
-        
-        To set global formats, set the following variables in `settings.py`:
-        
-        ```python
-        # Date formats
-        DRF_EXCEL_DATETIME_FORMAT = 'mm-dd-yy h:mm AM/PM'
-        DRF_EXCEL_DATE_FORMAT = 'mm-dd-yy'
-        DRF_EXCEL_TIME_FORMAT = 'h:mm AM/PM'
-        
-        # Number formats
-        DRF_EXCEL_INTEGER_FORMAT = '0%'
-        DRF_EXCEL_DECIMAL_FORMAT = '0.00E+00'
-        ```
-        
-        ### Name boolean values
-        
-        `True` and `False` as values for boolean fields are not always the best representation and don't support translation. 
-        
-        This can be controlled with in you API view with `xlsx_boolean_labels`. 
-        
-        ```
-        xlsx_boolean_labels = {True: _('Yes'), False: _('No')}
-        ```
-        
-        will replace `True` with `Yes` and `False` with `No`.
-        
-        This can also be set globally in settings.py:
-        
-        ```
-        DRF_EXCEL_BOOLEAN_DISPLAY = {True: _('Yes'), False: _('No')}
-        ```
-        
-        
-        ### Custom columns
-        
-        You might find yourself explicitly returning a dict in your API response and would like to use its data to display additional columns. This can be done by passing `xlsx_custom_cols`.
-        
-        ```python
-        xlsx_custom_cols = {
-            'my_custom_col.val1.title': {
-                'label': 'Custom column!',
-                'formatter': custom_value_formatter
-            }
-        }
-        
-        ### Example function:
-        def custom_value_formatter(val):
-            return val + '!!!'
-        
-        ### Example response:
-        { 
-            results: [
-                {
-                    title: 'XLSX renderer',
-                    url: 'https://github.com/wharton/drf-excel'
-                    returned_dict: {
-                        val1: {
-                            title: 'Sometimes'
-                        },
-                        val2: {
-                            title: 'There is no way around'
-                        }
-                    }
-                }
-            ]
-        }
-        ```
-        
-        When no `label` is passed, `drf-excel` will display the key name in the header.
-        
-        `formatter` is also optional and accepts a function, which will then receive the value it is mapped to (it would receive "Sometimes" and return "Sometimes!!!" in our example).
-        
-        ### Custom mappings
-        
-        Assuming you have a field that returns a `dict` instead of a simple `str`, you might not want to return the whole object but only a value of it. Let's say `status` returns `{ value: 1, display: 'Active' }`. To return the `display` value in the `status` column, we can do this:
-        
-        ```python
-        xlsx_custom_mappings = {
-            'status': 'display'
-        }
-        ```
-        
-        A more common case is that you want to change how a value is formatted. `xlsx_custom_mappings` also takes functions as values. Assuming we have a field `description`, and for some strange reason want to reverse the text, we can do this:
-        
-        ```python
-        def reverse_text(val):
-            return val[::-1]
-        
-        xlsx_custom_mappings = {
-            'description': reverse_text
-        }
-        ```
-        
-        ## Release Notes and Contributors
-        
-        * [Release notes](https://github.com/wharton/drf-excel/releases)
-        * [Our wonderful contributors](https://github.com/wharton/drf-excel/graphs/contributors)
-        
-        ## Maintainers
-        
-        * [Timothy Allen](https://github.com/FlipperPA) at [The Wharton School](https://github.com/wharton)
-        * [Thomas Willems](https://github.com/willtho89)
-        * [Mathieu Rampant](https://github.com/rptmat57)
-        
-        This package was created by the staff of [Wharton Research Data Services](https://wrds.wharton.upenn.edu/). We are thrilled that [The Wharton School](https://www.wharton.upenn.edu/) allows us a certain amount of time to contribute to open-source projects. We add features as they are necessary for our projects, and try to keep up with Issues and Pull Requests as best we can. Due to constraints of time (our full time jobs!), Feature Requests without a Pull Request may not be implemented, but we are always open to new ideas and grateful for contributions and our users.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 4
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DRF Excel: Django REST Framework Excel Spreadsheet (xlsx) Renderer
+
+`drf-excel` provides an Excel spreadsheet (xlsx) renderer for Django REST Framework. It uses OpenPyXL to create the spreadsheet and provide the file to the end user.
+
+## Requirements
+
+We aim to support Django's [currently supported versions](https://www.djangoproject.com/download/), as well as:
+
+* Django REST Framework >= 3.14
+* OpenPyXL >= 2.4
+
+## Installation
+
+```bash
+pip install drf-excel
+```
+
+Then add the following to your `REST_FRAMEWORK` settings:
+
+```python
+REST_FRAMEWORK = {
+    ...
+
+    'DEFAULT_RENDERER_CLASSES': (
+        'rest_framework.renderers.JSONRenderer',
+        'rest_framework.renderers.BrowsableAPIRenderer',
+        'drf_excel.renderers.XLSXRenderer',
+    ),
+}
+```
+
+To avoid having a file streamed without a filename (which the browser will often default to the filename "download", with no extension), we need to use a mixin to override the `Content-Disposition` header. If no `filename` is provided, it will default to `export.xlsx`. For example:
+
+```python
+from rest_framework.viewsets import ReadOnlyModelViewSet
+from drf_excel.mixins import XLSXFileMixin
+from drf_excel.renderers import XLSXRenderer
+
+from .models import MyExampleModel
+from .serializers import MyExampleSerializer
+
+class MyExampleViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
+    queryset = MyExampleModel.objects.all()
+    serializer_class = MyExampleSerializer
+    renderer_classes = (XLSXRenderer,)
+    filename = 'my_export.xlsx'
+```
+
+The `XLSXFileMixin` also provides a `get_filename()` method which can be overridden, if you prefer to provide a filename programmatically instead of the `filename` attribute.
+
+## Upgrading to 2.0.0
+
+To upgrade to `drf_excel` 2.0.0 from `drf_renderer_xlsx`, update your import paths:
+
+* `from drf_renderer_xlsx.mixins import XLSXFileMixin` becomes `from drf_excel.mixins import XLSXFileMixin`.
+* `drf_renderer_xlsx.renderers.XLSXRenderer` becomes `drf_excel.renderers.XLSXRenderer`.
+* `xlsx_date_format_mappings` has been removed in favor of `column_data_styles` which provides more flexibility
+
+## Configuring Styles 
+
+Styles can be added to your worksheet header, column header row, body and column data from view attributes `header`, `column_header`, `body`, `column_data_styles`. Any arguments from [the OpenPyXL package](https://openpyxl.readthedocs.io/en/stable/styles.html) can be used for font, alignment, fill and border_side (border will always be all side of cell).
+
+If provided, column data styles will override body style
+
+Note that column data styles can take an extra 'format' argument that follows [openpyxl formats](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/styles/numbers.html).
+
+```python
+class MyExampleViewSet(XLSXFileMixin, ReadOnlyModelViewSet):
+    queryset = MyExampleModel.objects.all()
+    serializer_class = MyExampleSerializer
+    renderer_classes = (XLSXRenderer,)
+
+    column_header = {
+        'titles': [
+            "Column_1_name",
+            "Column_2_name",
+            "Column_3_name",
+        ],
+        'column_width': [17, 30, 17],
+        'height': 25,
+        'style': {
+            'fill': {
+                'fill_type': 'solid',
+                'start_color': 'FFCCFFCC',
+            },
+            'alignment': {
+                'horizontal': 'center',
+                'vertical': 'center',
+                'wrapText': True,
+                'shrink_to_fit': True,
+            },
+            'border_side': {
+                'border_style': 'thin',
+                'color': 'FF000000',
+            },
+            'font': {
+                'name': 'Arial',
+                'size': 14,
+                'bold': True,
+                'color': 'FF000000',
+            },
+        },
+    }
+    body = {
+        'style': {
+            'fill': {
+                'fill_type': 'solid',
+                'start_color': 'FFCCFFCC',
+            },
+            'alignment': {
+                'horizontal': 'center',
+                'vertical': 'center',
+                'wrapText': True,
+                'shrink_to_fit': True,
+            },
+            'border_side': {
+                'border_style': 'thin',
+                'color': 'FF000000',
+            },
+            'font': {
+                'name': 'Arial',
+                'size': 14,
+                'bold': False,
+                'color': 'FF000000',
+            }
+        },
+        'height': 40,
+    }
+    column_data_styles = {
+        'distance': {
+            'alignment': {
+                'horizontal': 'right',
+                'vertical': 'top',
+            },
+            'format': '0.00E+00'
+        },
+        'created_at': {
+            'format': 'd.m.y h:mm',
+        }
+    }
+```
+
+You can dynamically generate style attributes in methods `get_body`, `get_header`, `get_column_header`, `get_column_data_styles`.
+
+```python
+def get_header(self):
+    start_time, end_time = parse_times(request=self.request)
+    datetime_format = "%H:%M:%S %d.%m.%Y"
+    return {
+        'tab_title': 'MyReport', # title of tab/workbook
+        'use_header': True,  # show the header_title 
+        'header_title': 'Report from {} to {}'.format(
+            start_time.strftime(datetime_format),
+            end_time.strftime(datetime_format),
+        ),
+        'height': 45,
+        'img': 'app/images/MyLogo.png',
+        'style': {
+            'fill': {
+                'fill_type': 'solid',
+                'start_color': 'FFFFFFFF',
+            },
+            'alignment': {
+                'horizontal': 'center',
+                'vertical': 'center',
+                'wrapText': True,
+                'shrink_to_fit': True,
+            },
+            'border_side': {
+                'border_style': 'thin',
+                'color': 'FF000000',
+            },
+            'font': {
+                'name': 'Arial',
+                'size': 16,
+                'bold': True,
+                'color': 'FF000000',
+            }
+        }
+    }
+```
+
+Also, you can add the `row_color` field to your serializer and fill body rows.
+
+```python
+class ExampleSerializer(serializers.Serializer):
+    row_color = serializers.SerializerMethodField()
+
+    def get_row_color(self, instance):
+        color_map = {'w': 'FFFFFFCC', 'a': 'FFFFCCCC'}
+        return color_map.get(instance.alarm_level, 'FFFFFFFF')
+```
+
+## Configuring Sheet View Options
+
+View options follow [openpyxl sheet view options](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/worksheet/views.html#SheetView)
+
+They can be set in the view as a property `sheet_view_options`:
+
+```python
+class MyExampleViewSet(serializers.Serializer):
+    sheet_view_options = {
+        'rightToLeft': True, 
+        'showGridLines': False
+    }
+```
+
+or using method `get_sheet_view_options`:
+
+```python
+class MyExampleViewSet(serializers.Serializer):
+    
+    def get_sheet_view_options(self):
+        return {
+            'rightToLeft': True, 
+            'showGridLines': False
+        }
+```
+## Controlling XLSX headers and values
+
+### Use Serializer Field labels as header names
+
+By default, headers will use the same 'names' as they are returned by the API. This can be changed by setting `xlsx_use_labels = True` inside your API View. 
+
+Instead of using the field names, the export will use the labels as they are defined inside your Serializer. A serializer field defined as `title = serializers.CharField(label=_("Some title"))` would return `Some title` instead of `title`, also supporting translations. If no label is set, it will fall back to using `title`.
+
+### Ignore fields
+
+By default, all fields are exported, but you might want to exclude some fields from your export. To do so, you can set an array with fields you want to exclude: `xlsx_ignore_headers = [<excluded fields>]`.
+
+This also works with nested fields, separated with a dot (i.e. `icon.url`).
+
+### Date/time and number formatting
+Formatting for cells follows [openpyxl formats](https://openpyxl.readthedocs.io/en/stable/_modules/openpyxl/styles/numbers.html).
+
+To set global formats, set the following variables in `settings.py`:
+
+```python
+# Date formats
+DRF_EXCEL_DATETIME_FORMAT = 'mm-dd-yy h:mm AM/PM'
+DRF_EXCEL_DATE_FORMAT = 'mm-dd-yy'
+DRF_EXCEL_TIME_FORMAT = 'h:mm AM/PM'
+
+# Number formats
+DRF_EXCEL_INTEGER_FORMAT = '0%'
+DRF_EXCEL_DECIMAL_FORMAT = '0.00E+00'
+```
+
+### Name boolean values
+
+`True` and `False` as values for boolean fields are not always the best representation and don't support translation. 
+
+This can be controlled with in you API view with `xlsx_boolean_labels`. 
+
+```
+xlsx_boolean_labels = {True: _('Yes'), False: _('No')}
+```
+
+will replace `True` with `Yes` and `False` with `No`.
+
+This can also be set globally in settings.py:
+
+```
+DRF_EXCEL_BOOLEAN_DISPLAY = {True: _('Yes'), False: _('No')}
+```
+
+
+### Custom columns
+
+You might find yourself explicitly returning a dict in your API response and would like to use its data to display additional columns. This can be done by passing `xlsx_custom_cols`.
+
+```python
+xlsx_custom_cols = {
+    'my_custom_col.val1.title': {
+        'label': 'Custom column!',
+        'formatter': custom_value_formatter
+    }
+}
+
+### Example function:
+def custom_value_formatter(val):
+    return val + '!!!'
+
+### Example response:
+{ 
+    results: [
+        {
+            title: 'XLSX renderer',
+            url: 'https://github.com/wharton/drf-excel'
+            returned_dict: {
+                val1: {
+                    title: 'Sometimes'
+                },
+                val2: {
+                    title: 'There is no way around'
+                }
+            }
+        }
+    ]
+}
+```
+
+When no `label` is passed, `drf-excel` will display the key name in the header.
+
+`formatter` is also optional and accepts a function, which will then receive the value it is mapped to (it would receive "Sometimes" and return "Sometimes!!!" in our example).
+
+### Custom mappings
+
+Assuming you have a field that returns a `dict` instead of a simple `str`, you might not want to return the whole object but only a value of it. Let's say `status` returns `{ value: 1, display: 'Active' }`. To return the `display` value in the `status` column, we can do this:
+
+```python
+xlsx_custom_mappings = {
+    'status': 'display'
+}
+```
+
+A more common case is that you want to change how a value is formatted. `xlsx_custom_mappings` also takes functions as values. Assuming we have a field `description`, and for some strange reason want to reverse the text, we can do this:
+
+```python
+def reverse_text(val):
+    return val[::-1]
+
+xlsx_custom_mappings = {
+    'description': reverse_text
+}
+```
+
+## Release Notes and Contributors
+
+* [Release notes](https://github.com/wharton/drf-excel/releases)
+* [Our wonderful contributors](https://github.com/wharton/drf-excel/graphs/contributors)
+
+## Maintainers
+
+* [Timothy Allen](https://github.com/FlipperPA) at [The Wharton School](https://github.com/wharton)
+* [Thomas Willems](https://github.com/willtho89)
+* [Mathieu Rampant](https://github.com/rptmat57)
+
+This package was created by the staff of [Wharton Research Data Services](https://wrds.wharton.upenn.edu/). We are thrilled that [The Wharton School](https://www.wharton.upenn.edu/) allows us a certain amount of time to contribute to open-source projects. We add features as they are necessary for our projects, and try to keep up with Issues and Pull Requests as best we can. Due to constraints of time (our full time jobs!), Feature Requests without a Pull Request may not be implemented, but we are always open to new ideas and grateful for contributions and our users.
```

### Comparing `drf-excel-2.3.0/setup.py` & `drf-excel-2.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,20 @@
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Framework :: Django",
-        "Framework :: Django :: 2",
         "Framework :: Django :: 3",
         "Framework :: Django :: 4",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     ],
 )
```

