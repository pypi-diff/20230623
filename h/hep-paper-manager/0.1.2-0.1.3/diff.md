# Comparing `tmp/hep_paper_manager-0.1.2.tar.gz` & `tmp/hep_paper_manager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hep_paper_manager-0.1.2.tar", max compression
+gzip compressed data, was "hep_paper_manager-0.1.3.tar", max compression
```

## Comparing `hep_paper_manager-0.1.2.tar` & `hep_paper_manager-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     3614 2023-06-22 06:48:46.781243 hep_paper_manager-0.1.2/README.md
--rw-r--r--   0        0        0      366 2023-06-22 06:43:44.212689 hep_paper_manager-0.1.2/hpm/__init__.py
--rw-r--r--   0        0        0     5434 2023-06-22 06:34:34.711658 hep_paper_manager-0.1.2/hpm/cli.py
--rw-r--r--   0        0        0       29 2023-06-13 04:12:40.062240 hep_paper_manager-0.1.2/hpm/engines/__init__.py
--rw-r--r--   0        0        0     3648 2023-06-22 06:02:12.027147 hep_paper_manager-0.1.2/hpm/engines/inspire.py
--rw-r--r--   0        0        0       27 2023-06-13 04:13:59.907266 hep_paper_manager-0.1.2/hpm/notion/__init__.py
--rw-r--r--   0        0        0     3427 2023-06-18 11:18:06.400535 hep_paper_manager-0.1.2/hpm/notion/client.py
--rw-r--r--   0        0        0       54 2023-06-13 04:13:42.598101 hep_paper_manager-0.1.2/hpm/notion/objects/__init__.py
--rw-r--r--   0        0        0      962 2023-06-13 04:13:47.941688 hep_paper_manager-0.1.2/hpm/notion/objects/database.py
--rw-r--r--   0        0        0     3682 2023-06-13 04:13:54.692063 hep_paper_manager-0.1.2/hpm/notion/objects/page.py
--rw-r--r--   0        0        0     5166 2023-06-18 11:18:06.402552 hep_paper_manager-0.1.2/hpm/notion/properties.py
--rw-r--r--   0        0        0      215 2023-06-22 06:12:46.868533 hep_paper_manager-0.1.2/hpm/templates/paper.yml
--rw-r--r--   0        0        0      698 2023-06-22 06:43:54.226477 hep_paper_manager-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4263 1970-01-01 00:00:00.000000 hep_paper_manager-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-22 07:10:17.667054 hep_paper_manager-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3770 2023-06-23 10:34:03.963586 hep_paper_manager-0.1.3/README.md
+-rw-r--r--   0        0        0      366 2023-06-23 10:34:03.964059 hep_paper_manager-0.1.3/hpm/__init__.py
+-rw-r--r--   0        0        0     5864 2023-06-23 10:33:43.459023 hep_paper_manager-0.1.3/hpm/cli.py
+-rw-r--r--   0        0        0       29 2023-06-13 04:12:40.062240 hep_paper_manager-0.1.3/hpm/engines/__init__.py
+-rw-r--r--   0        0        0     3648 2023-06-22 07:01:11.908415 hep_paper_manager-0.1.3/hpm/engines/inspire.py
+-rw-r--r--   0        0        0       27 2023-06-13 04:13:59.907266 hep_paper_manager-0.1.3/hpm/notion/__init__.py
+-rw-r--r--   0        0        0     3427 2023-06-18 11:18:06.400535 hep_paper_manager-0.1.3/hpm/notion/client.py
+-rw-r--r--   0        0        0       54 2023-06-13 04:13:42.598101 hep_paper_manager-0.1.3/hpm/notion/objects/__init__.py
+-rw-r--r--   0        0        0      962 2023-06-13 04:13:47.941688 hep_paper_manager-0.1.3/hpm/notion/objects/database.py
+-rw-r--r--   0        0        0     3682 2023-06-23 10:04:15.831479 hep_paper_manager-0.1.3/hpm/notion/objects/page.py
+-rw-r--r--   0        0        0     5470 2023-06-23 10:33:43.460062 hep_paper_manager-0.1.3/hpm/notion/properties.py
+-rw-r--r--   0        0        0      215 2023-06-22 07:01:11.909628 hep_paper_manager-0.1.3/hpm/templates/paper.yml
+-rw-r--r--   0        0        0      698 2023-06-23 10:34:03.964999 hep_paper_manager-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 hep_paper_manager-0.1.3/PKG-INFO
```

### Comparing `hep_paper_manager-0.1.2/README.md` & `hep_paper_manager-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -35,30 +35,30 @@
    Journal: Select
    Authors: Multi-select
    Abstract: Text
    URL: URL
    Bibtex: Text
    Source: Select
    ```
-   ![database](https://imgur.com/L3pJk1h.png)
+   ![database](https://imgur.com/RjIKM7I.png)
    Tip: Consider adding Authors as a Relation property. This allows you to concentrate on specific authors or professors of interest. Just add the integration to the related professors' database. hpm will locate authors based on the page Title property in the related database and fetched names.
 
 2. Then set up `hpm` with `hpm init`:
-   ![hpm init](https://imgur.com/282SiHF.png)
+   ![hpm init](https://imgur.com/qm0uPH1.png)
 
 3. Before adding our paper to a database, review the default `paper.yml` template and insert the database ID:
-   ![paper.yml](https://imgur.com/nmXWNrB.png)
-   The database ID is in the database URL. For the database just created: "https://www.notion.so/star9daisy/67877176f7064ed982e177aaf70f27cb?v=ffcad911d3d9416bb91657814242fd27&pvs=4", "67877176f7064ed982e177aaf70f27cb" is the database ID.
+   ![paper.yml](https://imgur.com/zjzqYiT.png)
+   The database ID is in the database URL. For the database just created: "https://www.notion.so/star9daisy/d91282815e5143818ae36ff05132d3b7?v=1ed0289b07ae4e1c8edeeb6eaf1d722f&pvs=4", "d91282815e5143818ae36ff05132d3b7" is the database ID.
    
    Remember to structure your database as shown above and add the integration to the database!
 
 4. Now let's add the paper into the database:
-  ![hpm add](https://imgur.com/ycWCn3Y.png)
+  ![hpm add](https://imgur.com/twxP8cv.png)
    The database in Notion should now look like the following:
-  ![database](https://imgur.com/9U2jdSi.png)
+  ![database](https://imgur.com/DjJBOuG.png)
 
 ## Engines
 - `Inspire`: It fetches papers from the [Inspire HEP](https://inspirehep.net/). It serves the default engine for `hpm`.
   - Parameters: `arxiv_id`
   - Returns: `Paper(title, authors, abstract, journal, citations, url, bibtex, source)`
 
 ## Templates
@@ -76,13 +76,16 @@
     abstract: Abstract
     url: URL
     bibtex: Bibtex
     source: Source
   ```
 
 ## Updates
+### v0.1.3
+- Update `hpm add` to check if the paper already exists in the database.
+- You can now create a database with more properties then the template.
 ### v0.1.2
 - Update paper from Inspire engine to include url, bibtex, and source. 
 ### v0.1.1
 - Add `hpm init` for interactive setup.
 - Add `hpm add` for adding a paper to a Notion database.
 - Introduce the default `Inspire` engine and `paper.yml` template.
```

### Comparing `hep_paper_manager-0.1.2/hpm/cli.py` & `hep_paper_manager-0.1.3/hpm/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,39 +97,48 @@
         DatabaseRelation: Relation,
         DatabaseRichText: RichText,
         DatabaseSelect: Select,
         DatabaseTitle: Title,
         DatabaseURL: URL,
     }
 
-    # Use database properties for page properties
+    # Use template properties for page properties rather than database properties
+    # to allow for other properties that are not in the template but in the database
     page = Page(
         parent_id=database_id,
         properties={
-            name: property_database_to_page[type(property)]()
-            for name, property in database.properties.items()
+            name: property_database_to_page[type(database.properties[name])]()
+            for _, name in template["properties"].items()
         },
     )
 
     # Extract property values from engine results according to the template
     for source, target in template["properties"].items():
         property = page.properties[target]
         if type(property) == Relation:
             for i in getattr(engine_results, source):
                 if i in database.properties[target].value:
                     page.properties[target].value.append(database.properties[target].value[i])
         else:
+            if type(property) == Title:
+                page.title = getattr(engine_results, source)
             page.properties[target].value = getattr(engine_results, source)
 
+    # Check if the page already exists
+    for i in database.pages:
+        if i.title == page.title:
+            print("[red]Page already exists!")
+            raise typer.Exit(code=1)
+
     # Create the page
     response = client.create_page(database_id, page.properties_to_dict())
     if response.status_code == 200:
-        print("Page created successfully!")
+        print("[green]Page created successfully!")
     else:
-        print("Page creation failed!")
+        print("[red]Page creation failed!")
         print(response.text)
         raise typer.Exit(code=1)
 
 
 def version_callback(value: bool):
     if value:
         print(f"{__app_name__} v[yellow]{__app_version__}[/yellow]")
```

### Comparing `hep_paper_manager-0.1.2/hpm/engines/inspire.py` & `hep_paper_manager-0.1.3/hpm/engines/inspire.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.2/hpm/notion/client.py` & `hep_paper_manager-0.1.3/hpm/notion/client.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.2/hpm/notion/objects/database.py` & `hep_paper_manager-0.1.3/hpm/notion/objects/database.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.2/hpm/notion/objects/page.py` & `hep_paper_manager-0.1.3/hpm/notion/objects/page.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.2/hpm/notion/properties.py` & `hep_paper_manager-0.1.3/hpm/notion/properties.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "DatabaseMultiSelect",
     "DatabaseNumber",
     "DatabaseRelation",
     "DatabaseRichText",
     "DatabaseSelect",
     "DatabaseTitle",
     "DatabaseURL",
+    "OtherProperty",
     "Property",
     "read_property",
 ]
 
 
 def read_property(property: dict, source: str = "page") -> Property:
     if source == "page":
@@ -43,26 +44,41 @@
             "select": DatabaseSelect,
             "title": DatabaseTitle,
             "url": DatabaseURL,
         }
     else:
         raise ValueError(f"Invalid source: {source}, choose 'page' or 'database'")
 
-    return property_type_to_class[property["type"]].from_dict(property)
+    if property["type"] in property_type_to_class:
+        return property_type_to_class[property["type"]].from_dict(property)
+    else:
+        return OtherProperty()
 
 
 class Property(Protocol):
     value: Any
 
     @classmethod
     def from_dict(cls, property: dict) -> Property:
         ...
 
     def to_dict(self) -> dict:
         ...
+
+
+@dataclass
+class OtherProperty:
+    value: str = "Unknown"
+
+    @classmethod
+    def from_dict(cls, property: dict) -> Property:
+        ...
+
+    def to_dict(self) -> dict:
+        ...
 
 
 @dataclass
 class MultiSelect:
     value: list[str | None] = field(default_factory=list)
 
     @classmethod
```

### Comparing `hep_paper_manager-0.1.2/pyproject.toml` & `hep_paper_manager-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hep-paper-manager"
-version = "0.1.2"
+version = "0.1.3"
 description = "HPM is a command-line tool that adds High Energy Physics (HEP) papers to a Notion database."
 authors = ["Star9daisy <star9daisy@outlook.com>"]
 readme = "README.md"
 packages = [
     { include = "hpm" },
 ]
```

### Comparing `hep_paper_manager-0.1.2/PKG-INFO` & `hep_paper_manager-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hep-paper-manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: HPM is a command-line tool that adds High Energy Physics (HEP) papers to a Notion database.
 Author: Star9daisy
 Author-email: star9daisy@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -52,30 +52,30 @@
    Journal: Select
    Authors: Multi-select
    Abstract: Text
    URL: URL
    Bibtex: Text
    Source: Select
    ```
-   ![database](https://imgur.com/L3pJk1h.png)
+   ![database](https://imgur.com/RjIKM7I.png)
    Tip: Consider adding Authors as a Relation property. This allows you to concentrate on specific authors or professors of interest. Just add the integration to the related professors' database. hpm will locate authors based on the page Title property in the related database and fetched names.
 
 2. Then set up `hpm` with `hpm init`:
-   ![hpm init](https://imgur.com/282SiHF.png)
+   ![hpm init](https://imgur.com/qm0uPH1.png)
 
 3. Before adding our paper to a database, review the default `paper.yml` template and insert the database ID:
-   ![paper.yml](https://imgur.com/nmXWNrB.png)
-   The database ID is in the database URL. For the database just created: "https://www.notion.so/star9daisy/67877176f7064ed982e177aaf70f27cb?v=ffcad911d3d9416bb91657814242fd27&pvs=4", "67877176f7064ed982e177aaf70f27cb" is the database ID.
+   ![paper.yml](https://imgur.com/zjzqYiT.png)
+   The database ID is in the database URL. For the database just created: "https://www.notion.so/star9daisy/d91282815e5143818ae36ff05132d3b7?v=1ed0289b07ae4e1c8edeeb6eaf1d722f&pvs=4", "d91282815e5143818ae36ff05132d3b7" is the database ID.
    
    Remember to structure your database as shown above and add the integration to the database!
 
 4. Now let's add the paper into the database:
-  ![hpm add](https://imgur.com/ycWCn3Y.png)
+  ![hpm add](https://imgur.com/twxP8cv.png)
    The database in Notion should now look like the following:
-  ![database](https://imgur.com/9U2jdSi.png)
+  ![database](https://imgur.com/DjJBOuG.png)
 
 ## Engines
 - `Inspire`: It fetches papers from the [Inspire HEP](https://inspirehep.net/). It serves the default engine for `hpm`.
   - Parameters: `arxiv_id`
   - Returns: `Paper(title, authors, abstract, journal, citations, url, bibtex, source)`
 
 ## Templates
@@ -93,13 +93,16 @@
     abstract: Abstract
     url: URL
     bibtex: Bibtex
     source: Source
   ```
 
 ## Updates
+### v0.1.3
+- Update `hpm add` to check if the paper already exists in the database.
+- You can now create a database with more properties then the template.
 ### v0.1.2
 - Update paper from Inspire engine to include url, bibtex, and source. 
 ### v0.1.1
 - Add `hpm init` for interactive setup.
 - Add `hpm add` for adding a paper to a Notion database.
 - Introduce the default `Inspire` engine and `paper.yml` template.
```

