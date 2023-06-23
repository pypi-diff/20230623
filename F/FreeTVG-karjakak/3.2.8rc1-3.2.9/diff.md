# Comparing `tmp/FreeTVG-karjakak-3.2.8rc1.tar.gz` & `tmp/FreeTVG-karjakak-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTVG-karjakak-3.2.8rc1.tar", last modified: Mon May 22 07:21:13 2023, max compression
+gzip compressed data, was "FreeTVG-karjakak-3.2.9.tar", last modified: Sat May 27 02:52:52 2023, max compression
```

## Comparing `FreeTVG-karjakak-3.2.8rc1.tar` & `FreeTVG-karjakak-3.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 07:21:13.925195 FreeTVG-karjakak-3.2.8rc1/
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 07:21:13.919670 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/
--rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      463 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/SOURCES.txt
--rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/dependency_links.txt
--rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/entry_points.txt
--rw-r--r--   0 karja      (501) staff       (20)      151 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/requires.txt
--rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-22 07:21:13.000000 FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/top_level.txt
--rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.8rc1/LICENSE.txt
--rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-22 07:21:13.925277 FreeTVG-karjakak-3.2.8rc1/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.8rc1/README.md
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 07:21:13.921853 FreeTVG-karjakak-3.2.8rc1/TVG/
--rw-r--r--   0 karja      (501) staff       (20)   146320 2023-05-22 01:33:43.000000 FreeTVG-karjakak-3.2.8rc1/TVG/FreeTVG.py
--rw-r--r--   0 karja      (501) staff       (20)   360883 2023-05-17 06:38:49.000000 FreeTVG-karjakak-3.2.8rc1/TVG/Tutorial TVG.pdf
--rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.8rc1/TVG/__init__.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 07:21:13.923122 FreeTVG-karjakak-3.2.8rc1/TVG/structure/
--rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.8rc1/TVG/structure/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)    14894 2023-05-16 16:03:03.000000 FreeTVG-karjakak-3.2.8rc1/TVG/structure/frame_layouts.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-22 07:21:13.924897 FreeTVG-karjakak-3.2.8rc1/TVG/utility/
--rw-r--r--   0 karja      (501) staff       (20)      923 2023-05-16 14:56:03.000000 FreeTVG-karjakak-3.2.8rc1/TVG/utility/RegMail.py
--rw-r--r--   0 karja      (501) staff       (20)       84 2023-05-15 12:31:08.000000 FreeTVG-karjakak-3.2.8rc1/TVG/utility/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)     7090 2023-05-22 07:20:50.000000 FreeTVG-karjakak-3.2.8rc1/TVG/utility/mdh.py
--rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.8rc1/pyproject.toml
--rw-r--r--   0 karja      (501) staff       (20)      979 2023-05-22 07:21:13.925567 FreeTVG-karjakak-3.2.8rc1/setup.cfg
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-27 02:52:52.530965 FreeTVG-karjakak-3.2.9/
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-27 02:52:52.527339 FreeTVG-karjakak-3.2.9/FreeTVG_karjakak.egg-info/
+-rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-27 02:52:52.000000 FreeTVG-karjakak-3.2.9/FreeTVG_karjakak.egg-info/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      463 2023-05-27 02:52:52.000000 FreeTVG-karjakak-3.2.9/FreeTVG_karjakak.egg-info/SOURCES.txt
+-rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-27 02:52:52.000000 FreeTVG-karjakak-3.2.9/FreeTVG_karjakak.egg-info/dependency_links.txt
+-rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-27 02:52:52.000000 FreeTVG-karjakak-3.2.9/FreeTVG_karjakak.egg-info/entry_points.txt
+-rw-r--r--   0 karja      (501) staff       (20)      165 2023-05-27 02:52:52.000000 FreeTVG-karjakak-3.2.9/FreeTVG_karjakak.egg-info/requires.txt
+-rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-27 02:52:52.000000 FreeTVG-karjakak-3.2.9/FreeTVG_karjakak.egg-info/top_level.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.9/LICENSE.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-27 02:52:52.531067 FreeTVG-karjakak-3.2.9/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.9/README.md
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-27 02:52:52.529434 FreeTVG-karjakak-3.2.9/TVG/
+-rw-r--r--   0 karja      (501) staff       (20)   142250 2023-05-27 02:03:17.000000 FreeTVG-karjakak-3.2.9/TVG/FreeTVG.py
+-rw-r--r--   0 karja      (501) staff       (20)   394226 2023-05-27 02:41:03.000000 FreeTVG-karjakak-3.2.9/TVG/Tutorial TVG.pdf
+-rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.9/TVG/__init__.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-27 02:52:52.529948 FreeTVG-karjakak-3.2.9/TVG/structure/
+-rw-r--r--   0 karja      (501) staff       (20)       98 2023-05-27 02:14:47.000000 FreeTVG-karjakak-3.2.9/TVG/structure/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)    14910 2023-05-27 02:22:53.000000 FreeTVG-karjakak-3.2.9/TVG/structure/frame_layouts.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-27 02:52:52.530725 FreeTVG-karjakak-3.2.9/TVG/utility/
+-rw-r--r--   0 karja      (501) staff       (20)      923 2023-05-16 14:56:03.000000 FreeTVG-karjakak-3.2.9/TVG/utility/RegMail.py
+-rw-r--r--   0 karja      (501) staff       (20)       84 2023-05-27 02:17:26.000000 FreeTVG-karjakak-3.2.9/TVG/utility/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     7403 2023-05-27 02:51:08.000000 FreeTVG-karjakak-3.2.9/TVG/utility/mdh.py
+-rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.9/pyproject.toml
+-rw-r--r--   0 karja      (501) staff       (20)      991 2023-05-27 02:52:52.531360 FreeTVG-karjakak-3.2.9/setup.cfg
```

### Comparing `FreeTVG-karjakak-3.2.8rc1/FreeTVG_karjakak.egg-info/PKG-INFO` & `FreeTVG-karjakak-3.2.9/FreeTVG_karjakak.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.8rc1
+Version: 3.2.9
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.8rc1/LICENSE.txt` & `FreeTVG-karjakak-3.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.8rc1/PKG-INFO` & `FreeTVG-karjakak-3.2.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.8rc1
+Version: 3.2.9
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.8rc1/README.md` & `FreeTVG-karjakak-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.8rc1/TVG/FreeTVG.py` & `FreeTVG-karjakak-3.2.9/TVG/FreeTVG.py`

 * *Files 2% similar despite different names*

```diff
@@ -1746,14 +1746,17 @@
                 style = convhtml(
                     self._utilspdf(),
                     self.filename,
                     fon,
                     self.text.cget("background")[1:],
                     self.text.cget("foreground"),
                     preview=False,
+                    pdfpath=self.glop.joinpath(f"{self.filename}.pdf")
+                    if not self.plat.startswith("win")
+                    else None,
                 )
             del px, ck, sty, add, fon, style
 
     def spaces(self):
         """Mostly used by other functions to clear an obselete spaces.
         To appropriate the display better.
         """
@@ -2527,14 +2530,48 @@
                 i.destroy()
                 del i
             self.mdframe.destroy()
             self.__delattr__("mdb")
             self.__delattr__("mdframe")
             self.frb3.pack_forget()
 
+    def _compile_editor(self, rows: int):
+        self.store = tuple(i for i in self.text.get("0.0", END)[:-1].split("\n") if i)
+        ckc = {f"c{i}": f"child{i}" for i in range(1, 51)}
+        compiled = {}
+        et = rows
+        for i in self.store:
+            et += 1
+            if "s:" == i.lower()[:2]:
+                compiled[et] = ("space", "\n")
+            elif "p:" == i.lower()[:2]:
+                if i.partition(":")[2].isspace() or not bool(i.partition(":")[2]):
+                    raise Exception("Parent cannot be empty!")
+                else:
+                    compiled[et] = (
+                        "parent",
+                        i[2:].removeprefix(" "),
+                    )
+            elif i.lower().partition(":")[0] in list(ckc):
+                if i.partition(":")[2].isspace():
+                    compiled[et] = (
+                        ckc[i.partition(":")[0].lower()],
+                        i.partition(":")[2],
+                    )
+                elif bool(i.partition(":")[2]):
+                    compiled[et] = (
+                        ckc[i.partition(":")[0].lower()],
+                        i.partition(":")[2].removeprefix(" "),
+                    )
+        if len(self.store) != len(compiled):
+            raise Exception("Not Editable!")
+        self.store = None
+        del ckc
+        return compiled, et
+
     def editor(self):
         """This is direct editor on text window.
         FORMAT:
         "s:" for 'space'
         "p:" for 'parent'
         "c1:" - "c50:" for 'child1' to 'child50'
         """
@@ -2557,138 +2594,51 @@
                 self._mdbuttons()
                 if not self.plat.startswith("win"):
                     self.root.clipboard_clear()
                 del ckb
             else:
                 try:
                     if self.text.count("1.0", END, "chars")[0] > 1:
-                        self.store = self.text.get("1.0", END)
-                        if self.nonetype():
-                            if self.editorsel:
-                                stor = self.editorsel
-                                ed = tuple(i for i in self.store[:-1].split("\n") if i)
-                                ckc = {f"c{i}": f"child{i}" for i in range(1, 51)}
-                                et = stor[0]
-                                p2 = {}
-                                p1 = None
-                                p3 = None
-                                for i in ed:
-                                    et += 1
-                                    if "s:" == i.lower()[:2]:
-                                        p2[et] = ("space", "\n")
-                                    elif "p:" == i.lower()[:2]:
-                                        if i.partition(":")[2].isspace() or not bool(
-                                            i.partition(":")[2]
-                                        ):
-                                            raise Exception("Parent cannot be empty!")
-                                        else:
-                                            p2[et] = (
-                                                "parent",
-                                                i[2:].removeprefix(" "),
-                                            )
-                                    elif i.lower().partition(":")[0] in list(ckc):
-                                        if i.partition(":")[2].isspace():
-                                            p2[et] = (
-                                                ckc[i.partition(":")[0].lower()],
-                                                i.partition(":")[2],
-                                            )
-                                        elif bool(i.partition(":")[2]):
-                                            p2[et] = (
-                                                ckc[i.partition(":")[0].lower()],
-                                                i.partition(":")[2].removeprefix(" "),
-                                            )
-                                if len(ed) != len(p2):
-                                    raise Exception("Not Editable!")
-                                with tv(self.filename) as tvg:
-                                    p1 = islice(tvg.insighttree(), 0, stor[0])
-                                    if stor[1] < tvg.getdatanum() - 1:
-                                        p3 = islice(
-                                            tvg.insighttree(),
-                                            stor[1],
-                                            tvg.getdatanum(),
-                                        )
-                                    if p3:
-                                        p3 = tuple(v for v in dict(p3).values())
-                                        p3 = {et + j + 1: p3[j] for j in range(len(p3))}
-                                        combi = iter((dict(p1) | p2 | p3).values())
-                                    else:
-                                        combi = iter((dict(p1) | p2).values())
-                                    tvg.fileread(combi)
-                                del stor, tvg, p1, ed, ckc, et, p2, combi, p3
-                            else:
-                                et = self.listb.size()
-                                ed = tuple(i for i in self.store[:-1].split("\n") if i)
-                                ckc = {f"c{i}": f"child{i}" for i in range(1, 51)}
-                                p2 = {}
-                                for i in ed:
-                                    et += 1
-                                    if "s:" == i.lower()[:2]:
-                                        p2[et] = ("space", "\n")
-                                    elif "p:" == i.lower()[:2]:
-                                        if i.partition(":")[2].isspace() or not bool(
-                                            i.partition(":")[2]
-                                        ):
-                                            raise Exception("Parent cannot be empty!")
-                                        else:
-                                            p2[et] = (
-                                                "parent",
-                                                i[2:].removeprefix(" "),
-                                            )
-                                    elif i.lower().partition(":")[0] in list(ckc):
-                                        if i.partition(":")[2].isspace():
-                                            p2[et] = (
-                                                ckc[i.partition(":")[0].lower()],
-                                                i.partition(":")[2],
-                                            )
-                                        elif bool(i.partition(":")[2]):
-                                            p2[et] = (
-                                                ckc[i.partition(":")[0].lower()],
-                                                i.partition(":")[2].removeprefix(" "),
-                                            )
-                                if len(ed) != len(p2):
-                                    raise Exception("Not Editable!")
-                                with tv(self.filename) as tvg:
-                                    combi = iter(
-                                        (dict(tvg.insighttree()) | p2).values()
+                        stor = None
+                        if self.editorsel or (stor := self.listb.curselection()):
+                            stor = (
+                                self.editorsel if self.editorsel else (stor[0], stor[0])
+                            )
+                            p2 = self._compile_editor(stor[0])
+                            p1 = None
+                            p3 = None
+                            with tv(self.filename) as tvg:
+                                p1 = islice(tvg.insighttree(), 0, stor[0])
+                                if stor[1] <= tvg.getdatanum() - 1:
+                                    p3 = islice(
+                                        tvg.insighttree(),
+                                        stor[1],
+                                        tvg.getdatanum(),
                                     )
-                                    tvg.fileread(combi)
-                                del tvg, et, ed, ckc, p2, combi
+                                if p3:
+                                    p3 = tuple(v for v in dict(p3).values())
+                                    p3 = {p2[1] + j + 1: p3[j] for j in range(len(p3))}
+                                    combi = iter((dict(p1) | p2[0] | p3).values())
+                                else:
+                                    combi = iter((dict(p1) | p2[0]).values())
+                                tvg.fileread(combi)
+                            del tvg, p1, p2, combi, p3
                         else:
-                            ed = tuple(i for i in self.store[:-1].split("\n") if i)
-                            et = -1
-                            ckc = {f"c{i}": f"child{i}" for i in range(1, 51)}
-                            p2 = {}
-                            for i in ed:
-                                et += 1
-                                if "s:" == i.lower()[:2]:
-                                    p2[et] = ("space", "\n")
-                                elif "p:" == i.lower()[:2]:
-                                    if i.partition(":")[2].isspace() or not bool(
-                                        i.partition(":")[2]
-                                    ):
-                                        raise Exception("Parent cannot be empty!")
-                                    else:
-                                        p2[et] = ("parent", i[2:].removeprefix(" "))
-                                elif i.lower().partition(":")[0] in list(ckc):
-                                    if i.partition(":")[2].isspace():
-                                        p2[et] = (
-                                            ckc[i.partition(":")[0].lower()],
-                                            i.partition(":")[2],
-                                        )
-                                    elif bool(i.partition(":")[2]):
-                                        p2[et] = (
-                                            ckc[i.partition(":")[0].lower()],
-                                            i.partition(":")[2].removeprefix(" "),
-                                        )
-                            if len(ed) != len(p2):
-                                raise Exception("Not Editable!")
+                            p2 = self._compile_editor(self.listb.size())
                             with tv(self.filename) as tvg:
-                                tvg.fileread(iter(p2.values()))
-                            del tvg, ed, et, ckc, p2
-                        self.store = None
+                                if not self.nonetype():
+                                    tvg.fileread(iter(p2[0].values()))
+                                else:
+                                    combi = iter(
+                                        (dict(tvg.insighttree()) | p2[0]).values()
+                                    )
+                                    tvg.fileread(combi)
+                                    del combi
+                            del tvg, p2
+                        del stor
                         self.text.config(state=DISABLED)
                         self.disab(dis=False)
                         self.spaces()
                         if self.editorsel:
                             self.text.see(f"{self.editorsel[0]}.0")
                             self.editorsel = None
                     else:
@@ -2697,15 +2647,14 @@
                         self.spaces()
                         if self.editorsel:
                             self.editorsel = None
                 except Exception as a:
                     messagebox.showerror("TreeViewGui", f"{a}", parent=self.root)
                 if self.text.cget("state") == DISABLED:
                     self._mdbuttons()
-            self.store = None
             self.text.edit_reset()
             self.infobar()
 
     def tvgexit(self, event=None):
         """Exit mode for TVG and setting everything back to default"""
 
         if self.FREEZE is False:
```

### Comparing `FreeTVG-karjakak-3.2.8rc1/TVG/structure/frame_layouts.py` & `FreeTVG-karjakak-3.2.9/TVG/structure/frame_layouts.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from excptr import DEFAULTDIR, DEFAULTFILE, DIRPATH, excpcls
 
 DEFAULTDIR = os.path.join(DIRPATH, "FreeTVG_TRACE")
 if not os.path.exists(DEFAULTDIR):
     os.mkdir(DEFAULTDIR)
 DEFAULTFILE = os.path.join(DEFAULTDIR, Path(DEFAULTFILE).name)
 
+__all__ = [""]
+
 
 @excpcls(m=2, filenm=DEFAULTFILE)
 class Lay1(ttk.Frame):
     def __init__(self, root):
         super().__init__()
         self.pack(side=TOP, fill="x")
         self.label = ttk.Label(self, text="Words")
```

### Comparing `FreeTVG-karjakak-3.2.8rc1/TVG/utility/RegMail.py` & `FreeTVG-karjakak-3.2.9/TVG/utility/RegMail.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.8rc1/setup.cfg` & `FreeTVG-karjakak-3.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FreeTVG-karjakak
-version = 3.2.8rc1
+version = 3.2.9
 author = karjakak
 author_email = kakkarja.github@gmail.com
 description = Tree View Gui for outline treeview note.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kakkarja/FreeTVG#latest-notice
 license = MIT License
@@ -26,14 +26,15 @@
 	pymdown-extensions>=9.0
 	treeview-karjakak>=1.8.1
 	excptr-karjakak>=0.1.0
 	demoji>=1.1.0
 	tomlkit>=0.11.6
 	darkdetect>=0.8.0
 	pywebview>=4.1
+	pdfkit>=1.0.0
 
 [options.package_data]
 * = *.pdf
 
 [options.entry_points]
 gui_scripts = 
 	TVG = TVG:main
```

