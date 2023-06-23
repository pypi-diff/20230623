# Comparing `tmp/spip2md-0.1.0.tar.gz` & `tmp/spip2md-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spip2md-0.1.0.tar", max compression
+gzip compressed data, was "spip2md-0.1.1.tar", max compression
```

## Comparing `spip2md-0.1.0.tar` & `spip2md-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      232 2023-06-15 13:25:44.522961 spip2md-0.1.0/LICENSE
--rw-r--r--   0        0        0     5465 2023-06-16 14:49:01.520522 spip2md-0.1.0/README.md
--rw-r--r--   0        0        0      966 2023-06-16 15:11:26.356332 spip2md-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0      108 2023-06-16 12:57:07.193988 spip2md-0.1.0/spip2md/__main__.py
--rw-r--r--   0        0        0     4451 2023-06-16 14:35:34.265401 spip2md-0.1.0/spip2md/config.py
--rw-r--r--   0        0        0    32719 2023-06-16 14:49:42.234721 spip2md-0.1.0/spip2md/extended_models.py
--rw-r--r--   0        0        0     5378 2023-06-16 12:55:47.019487 spip2md-0.1.0/spip2md/lib.py
--rw-r--r--   0        0        0     9339 2023-06-16 13:46:06.904464 spip2md-0.1.0/spip2md/regexmaps.py
--rw-r--r--   0        0        0    26967 2023-06-15 13:28:04.655846 spip2md-0.1.0/spip2md/spip_models.py
--rw-r--r--   0        0        0     1318 2023-06-15 13:28:07.173826 spip2md-0.1.0/spip2md/style.py
--rw-r--r--   0        0        0     6870 1970-01-01 00:00:00.000000 spip2md-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2023-06-15 13:25:44.522961 spip2md-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6152 2023-06-23 14:25:57.743431 spip2md-0.1.1/README.md
+-rw-r--r--   0        0        0      966 2023-06-23 14:47:12.002923 spip2md-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0      108 2023-06-23 14:25:57.744431 spip2md-0.1.1/spip2md/__main__.py
+-rw-r--r--   0        0        0     4684 2023-06-23 14:25:57.744431 spip2md-0.1.1/spip2md/config.py
+-rw-r--r--   0        0        0    36042 2023-06-23 14:25:57.744431 spip2md-0.1.1/spip2md/extended_models.py
+-rw-r--r--   0        0        0     5378 2023-06-23 14:25:57.744431 spip2md-0.1.1/spip2md/lib.py
+-rw-r--r--   0        0        0     9339 2023-06-23 14:25:57.744431 spip2md-0.1.1/spip2md/regexmaps.py
+-rw-r--r--   0        0        0    26967 2023-06-23 14:25:57.744431 spip2md-0.1.1/spip2md/spip_models.py
+-rw-r--r--   0        0        0     1318 2023-06-23 14:25:57.744431 spip2md-0.1.1/spip2md/style.py
+-rw-r--r--   0        0        0     7557 1970-01-01 00:00:00.000000 spip2md-0.1.1/PKG-INFO
```

### Comparing `spip2md-0.1.0/README.md` & `spip2md-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -82,31 +82,43 @@
 export_languages: ["en"] # Array of languages to export, two letter lang code
 # If set, directories will be created only for this language, according to this
 # language’s titles. Other languages will be written along with correct url: attribute
 storage_language: null
 output_dir: output/ # The directory in which files will be written
 
 # Destination directories names settings
-prepend_h1: false # Add title of articles as Markdown h1, looks better on certain themes
 # Prepend ID to directory slug, preventing collisions
 # If false, a counter will be appended in case of name collision
 prepend_id: false
-prepend_lang: false # Prepend lang of the object to directory slug (prenvents collision)
-title_max_length: 40 # Maximum length of a single filename
+# Prepend lang of the object to directory slug, prenventing collision between langs
+prepend_lang: false
+title_max_length: 42 # Maximum length (chars) of a single filename
+
+# Text body processing settings
+remove_html: true # Should we clean remaining HTML blocks
+metadata_markup: false # Should we keep markup (Markdown) in metadata fields, like title
+unknown_char_replacement: ?? # String to replace broken encoding that cannot be repaired
+prepend_h1: false # Add title of articles as Markdown h1, looks better on certain themes
+# Array of objects with 2 or 3 values, allowing to move some fields into others.
+# {src: moved_field_name, dest: destination_field_name, repr: "how to merge them"}
+# repr is formatted with "{}" being the moved field, and "_" the destination one
+# For example, to append a field "subtitle" to a field "title":
+#   - src: subtitle
+#     dest: title
+#     repr: "{} _" # (this is the default repr)
+move_fields: []
+# Some taxonomies (Spip Mots types) to not export, typically specific to Spip functions
+ignore_taxonomies: ["Gestion du site", "Gestion des articles", "Mise en page"]
+rename_taxonomies: { equipes: "tag-equipes" } # Rename taxonomies (prenvent conflict)
 
 # Ignored data settings
 export_drafts: true # Should we export drafts
 export_empty: true # Should we export empty articles
 ignore_patterns: [] # List of regexes : Matching sections or articles will be ignored
 
-# Text body processing settings
-remove_html: true # Should we clean remaining HTML blocks
-metadata_markup: true # Should we keep markup (Markdown) in metadata fields (like title)
-unknown_char_replacement: ?? # String to replace broken encoding that cannot be repaired
-
 # Settings you probably don’t want to modify
 clear_log: true # Clear logfile between runs instead of appending to
 clear_output: true # Clear output dir between runs instead of merging into
 
 logfile: log-spip2md.log # Name of the logs file
 loglevel: WARNING # Refer to Python’s loglevels
```

### Comparing `spip2md-0.1.0/pyproject.toml` & `spip2md-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spip2md"
-version = "0.1.0"
+version = "0.1.1"
 description = "Generate a static website with plain Markdown+YAML files from a SPIP CMS database"
 license = "GPL-2.0"
 
 authors = [
   "Guilhem Fauré <guilhem.faure@gfaure.eu>"
 ]
```

### Comparing `spip2md-0.1.0/spip2md/config.py` & `spip2md-0.1.1/spip2md/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,20 +62,23 @@
     db_user: str = "spip"  # A DB user with read access to SPIP database
     db_pass: str = "password"  # Password of db_user
     data_dir: str = "IMG/"  # The directory in which SPIP images & documents are stored
     export_languages = ("fr", "en")  # Languages that will be exported
     storage_language: Optional[str] = "fr"  # Language of files and directories names
     output_dir: str = "output/"  # The directory to which DB will be exported
     prepend_h1: bool = False  # Add the title of the article as a Markdown h1
+    move_fields: list[dict[str, str]] = []  # Alternative destination for fields
     prepend_id: bool = False  # Add the ID of object before slug
     prepend_lang: bool = False  # Add the lang of object before slug
     export_drafts: bool = True  # Should we export drafts as draft:true articles
     export_empty: bool = True  # Should we export empty articles
     remove_html: bool = True  # Should spip2md remove every HTML tags
-    metadata_markup: bool = True  # Should spip2md keep the markup in metadata fields
+    ignore_taxonomies = ("Gestion du site", "Gestion des articles", "Mise en page")
+    rename_taxonomies: dict[str, str] = {"equipes": "tag-equipes"}
+    metadata_markup: bool = False  # Should spip2md keep the markup in metadata fields
     title_max_length: int = 40  # Maximum length of a single title for directory names
     unknown_char_replacement: str = "??"  # Replaces unknown characters
     clear_log: bool = True  # Clear log before every run instead of appending to
     clear_output: bool = True  # Remove eventual output dir before running
     ignore_patterns: list[str] = []  # Ignore objects of which title match
     logfile: str = "log-spip2md.log"  # File where logs will be written, relative to wd
     loglevel: str = "WARNING"  # Minimum criticity of logs written in logfile
```

### Comparing `spip2md-0.1.0/spip2md/extended_models.py` & `spip2md-0.1.1/spip2md/extended_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,23 +48,28 @@
 )
 from spip2md.spip_models import (
     SpipArticles,
     SpipAuteurs,
     SpipAuteursLiens,
     SpipDocuments,
     SpipDocumentsLiens,
+    SpipMots,
+    SpipMotsLiens,
     SpipRubriques,
 )
 from spip2md.style import BOLD, CYAN, GREEN, WARNING_STYLE, YELLOW, esc
 
 DeepDict = dict[str, "list[DeepDict] | list[str] | str"]
 
 # Define logger for this file’s logs
 LOG = logging.getLogger(NAME + ".models")
 
+# Define type that images can have
+IMG_TYPES = ("jpg", "png", "jpeg", "gif", "webp", "ico")
+
 
 class SpipWritable:
     # From SPIP database
     texte: str
     lang: str
     titre: str
     descriptif: str
@@ -345,16 +350,18 @@
     date: DateTimeField
     maj: str
     id_secteur: BigIntegerField | int
     extra: str
     langue_choisie: str
     # Converted
     _text: str
+    _taxonomies: dict[str, list[str]] = {}
     _url_title: str  # Title in metadata of articles
     _parenturl: str  # URL relative to lang to direct parent
+    _static_img_path: Optional[str] = None  # Path to the static img of this article
 
     # Get rid of other lang than forced in text and modify lang to forced if found
     def translate_multi(
         self, forced_lang: str, text: str, change_lang: bool = True
     ) -> str:
         # LOG.debug(f"Translating <multi> blocks of `{self._url_title}`")
         # for each <multi> blocks, keep only forced lang
@@ -368,14 +375,17 @@
                     f"Keeping {forced_lang} translation of `{self._url_title}`: "
                     + f"`{trans}`"
                 )
                 if change_lang:
                     self.lang = forced_lang  # So write-all will not be cancelled
                 # Replace the mutli blocks with the text in the proper lang
                 text = text.replace(block.group(), lang.group(1))
+            else:
+                # Replace the mutli blocks with the text inside
+                text = text.replace(block.group(), block.group(1))
         if lang is None:
             LOG.debug(f"{forced_lang} not found in `{self._url_title}`")
         return text
 
     def replace_links(self, text: str) -> str:
         class LinkMappings:
             _link_types = IMAGE_LINK, DOCUMENT_LINK, SECTION_LINK, ARTICLE_LINK
@@ -559,14 +569,45 @@
             self._extra = ""
             return
         LOG.debug(f"Convert internal links of {self.lang} `{self._url_title}` extra")
         self._extra = self.replace_links(self._extra)
         LOG.debug(f"Apply conversions to {self.lang} `{self._url_title}` extra")
         self._extra = self.convert_field(self._extra, CFG.metadata_markup)
 
+    def convert_taxonomies(self, forcedlang: str) -> None:
+        self._taxonomies = {}
+
+        for tag in self.taxonomies():
+            taxonomy = str(tag.type)
+            if taxonomy not in CFG.ignore_taxonomies:
+                LOG.debug(
+                    f"Translate taxonomy of `{self._url_title}`: {tag.descriptif}"
+                )
+                if taxonomy in CFG.rename_taxonomies:
+                    LOG.debug(
+                        f"Rename taxonomy {taxonomy}: {CFG.rename_taxonomies[taxonomy]}"
+                    )
+                    taxonomy = CFG.rename_taxonomies[taxonomy]
+                if str(taxonomy) in self._taxonomies:
+                    self._taxonomies[taxonomy].append(
+                        self.convert_field(
+                            self.translate_multi(forcedlang, str(tag.descriptif), False)
+                        )
+                    )
+                else:
+                    self._taxonomies[taxonomy] = [
+                        self.convert_field(
+                            self.translate_multi(forcedlang, str(tag.descriptif), False)
+                        )
+                    ]
+
+        LOG.debug(
+            f"After translation, taxonomies of `{self._url_title}`: {self._taxonomies}"
+        )
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # Initialize converted fields, beginning with underscore
         self._choosen_language = self.langue_choisie == "oui"
 
     # Get related documents
     def documents(self) -> tuple[Document]:
@@ -622,14 +663,36 @@
         elif not CFG.export_empty:
             raise DontExportEmptyError
         # Same with an "extra" section
         if len(self._extra) > 0:
             body += "\n\n# EXTRA\n\n" + self._extra
         return body
 
+    def authors(self) -> tuple[SpipAuteurs, ...]:
+        LOG.debug(f"Initialize authors of `{self._url_title}`")
+        return (
+            SpipAuteurs.select()
+            .join(
+                SpipAuteursLiens,
+                on=(SpipAuteurs.id_auteur == SpipAuteursLiens.id_auteur),
+            )
+            .where(SpipAuteursLiens.id_objet == self._id)
+        )
+
+    def taxonomies(self) -> tuple[SpipMots, ...]:
+        LOG.debug(f"Initialize taxonomies of `{self._url_title}`")
+        return (
+            SpipMots.select()
+            .join(
+                SpipMotsLiens,
+                on=(SpipMots.id_mot == SpipMotsLiens.id_mot),
+            )
+            .where(SpipMotsLiens.id_objet == self._id)
+        )
+
     # Write all the documents of this object
     def write_children(
         self,
         children: tuple[Document] | tuple[Any],
         forcedlang: str,
     ) -> list[str]:
         LOG.debug(f"Writing documents of {type(self).__name__} `{self._url_title}`")
@@ -693,27 +756,48 @@
                             self._storage_title_append += 1
                             incompatible = True
                             break
 
         # Write the content of this object into a file named as self.filename()
         with open(self.dest_path(), "w") as f:
             f.write(self.content())
+        # Write the eventual static image of this object
+        if self._static_img_path:
+            copyfile(
+                self._static_img_path,
+                self.dest_directory() + basename(self._static_img_path),
+            )
         return self.dest_path()
 
+    # Append static images based on filename instead of DB to objects texts
+    def append_static_images(self, obj_str: str = "art", load_str: str = "on"):
+        for t in IMG_TYPES:
+            path: str = CFG.data_dir + obj_str + load_str + str(self._id) + "." + t
+            LOG.debug(f"Search static image of `{self._url_title}` at: {path}")
+            if isfile(path):
+                LOG.debug(f"Found static image of `{self._url_title}` at: {path}")
+                # Append static image to content
+                self._text += f"\n\n![]({basename(path)})"
+                # Store it’s path to write it later
+                self._static_img_path = path
+                break
+
     # Apply post-init conversions and cancel the export if self not of the right lang
     def convert(self, forced_lang: str) -> None:
         self.convert_title(forced_lang)
         self.convert_text(forced_lang)
         self.convert_extra()
+        self.convert_taxonomies(forced_lang)
         if self.lang != forced_lang:
             raise LangNotFoundError(
                 f"`{self._url_title}` lang is {self.lang} instead of the wanted"
                 + f" {forced_lang} and it don’t contains"
                 + f" {forced_lang} translation in Markup either"
             )
+        self.append_static_images()
 
 
 class Article(SpipRedactional, SpipArticles):
     _fileprefix: str = "index"
     _style = (BOLD, YELLOW)  # Articles accent color is yellow
 
     class Meta:
@@ -737,15 +821,17 @@
             "surtitle": self.surtitre,
             "subtitle": self.soustitre,
             "date": self.date_redac,
             "authors": [author.nom for author in self.authors()],
         }
         # Add debugging meta if needed
         if CFG.debug_meta:
-            meta = meta | {"spip_id_rubrique": self.id_rubrique}
+            meta |= {"spip_id_rubrique": self.id_rubrique}
+        if self._taxonomies:
+            meta |= self._taxonomies
         if append is not None:
             return super().frontmatter(meta | append)
         else:
             return super().frontmatter(meta)
 
     def content(self) -> str:
         body: str = super().content()
@@ -756,25 +842,14 @@
         if len(self._ps) > 0:
             body += "\n\n# POST-SCRIPTUM\n\n" + self._ps
         # Microblog
         if len(self._microblog) > 0:
             body += "\n\n# MICROBLOGGING\n\n" + self._microblog
         return body
 
-    def authors(self) -> list[SpipAuteurs]:
-        LOG.debug(f"Initialize authors of `{self._url_title}`")
-        return (
-            SpipAuteurs.select()
-            .join(
-                SpipAuteursLiens,
-                on=(SpipAuteurs.id_auteur == SpipAuteursLiens.id_auteur),
-            )
-            .where(SpipAuteursLiens.id_objet == self._id)
-        )
-
     # Perform all the write steps of this object
     def write_all(
         self,
         parentdepth: int,
         storage_parentdir: str,
         index: int,
         total: int,
@@ -849,7 +924,11 @@
             "msg": super().write_all(
                 parentdepth, storage_parentdir, index, total, parenturl
             ),
             "documents": self.write_children(self.documents(), forced_lang),
             "articles": self.write_children(self.articles(), forced_lang),
             "sections": self.write_children(self.sections(), forced_lang),
         }
+
+    # Append static images based on filename instead of DB to objects texts
+    def append_static_images(self, obj_str: str = "rub", load_str: str = "on"):
+        super().append_static_images(obj_str, load_str)
```

### Comparing `spip2md-0.1.0/spip2md/lib.py` & `spip2md-0.1.1/spip2md/lib.py`

 * *Files identical despite different names*

### Comparing `spip2md-0.1.0/spip2md/regexmaps.py` & `spip2md-0.1.1/spip2md/regexmaps.py`

 * *Files identical despite different names*

### Comparing `spip2md-0.1.0/spip2md/spip_models.py` & `spip2md-0.1.1/spip2md/spip_models.py`

 * *Files identical despite different names*

### Comparing `spip2md-0.1.0/spip2md/style.py` & `spip2md-0.1.1/spip2md/style.py`

 * *Files identical despite different names*

### Comparing `spip2md-0.1.0/PKG-INFO` & `spip2md-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spip2md
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate a static website with plain Markdown+YAML files from a SPIP CMS database
 Home-page: https://git.irsamc.ups-tlse.fr/LCPQ/spip2md
 License: GPL-2.0
 Keywords: Markdown,Static website,SPIP,Converter,Exporter
 Author: Guilhem Fauré
 Author-email: guilhem.faure@gfaure.eu
 Requires-Python: >=3.9,<4.0
@@ -109,31 +109,43 @@
 export_languages: ["en"] # Array of languages to export, two letter lang code
 # If set, directories will be created only for this language, according to this
 # language’s titles. Other languages will be written along with correct url: attribute
 storage_language: null
 output_dir: output/ # The directory in which files will be written
 
 # Destination directories names settings
-prepend_h1: false # Add title of articles as Markdown h1, looks better on certain themes
 # Prepend ID to directory slug, preventing collisions
 # If false, a counter will be appended in case of name collision
 prepend_id: false
-prepend_lang: false # Prepend lang of the object to directory slug (prenvents collision)
-title_max_length: 40 # Maximum length of a single filename
+# Prepend lang of the object to directory slug, prenventing collision between langs
+prepend_lang: false
+title_max_length: 42 # Maximum length (chars) of a single filename
+
+# Text body processing settings
+remove_html: true # Should we clean remaining HTML blocks
+metadata_markup: false # Should we keep markup (Markdown) in metadata fields, like title
+unknown_char_replacement: ?? # String to replace broken encoding that cannot be repaired
+prepend_h1: false # Add title of articles as Markdown h1, looks better on certain themes
+# Array of objects with 2 or 3 values, allowing to move some fields into others.
+# {src: moved_field_name, dest: destination_field_name, repr: "how to merge them"}
+# repr is formatted with "{}" being the moved field, and "_" the destination one
+# For example, to append a field "subtitle" to a field "title":
+#   - src: subtitle
+#     dest: title
+#     repr: "{} _" # (this is the default repr)
+move_fields: []
+# Some taxonomies (Spip Mots types) to not export, typically specific to Spip functions
+ignore_taxonomies: ["Gestion du site", "Gestion des articles", "Mise en page"]
+rename_taxonomies: { equipes: "tag-equipes" } # Rename taxonomies (prenvent conflict)
 
 # Ignored data settings
 export_drafts: true # Should we export drafts
 export_empty: true # Should we export empty articles
 ignore_patterns: [] # List of regexes : Matching sections or articles will be ignored
 
-# Text body processing settings
-remove_html: true # Should we clean remaining HTML blocks
-metadata_markup: true # Should we keep markup (Markdown) in metadata fields (like title)
-unknown_char_replacement: ?? # String to replace broken encoding that cannot be repaired
-
 # Settings you probably don’t want to modify
 clear_log: true # Clear logfile between runs instead of appending to
 clear_output: true # Clear output dir between runs instead of merging into
 
 logfile: log-spip2md.log # Name of the logs file
 loglevel: WARNING # Refer to Python’s loglevels
```

