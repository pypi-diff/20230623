# Comparing `tmp/CTkTable-0.3.tar.gz` & `tmp/CTkTable-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkTable-0.3.tar", last modified: Thu Jun 22 11:05:05 2023, max compression
+gzip compressed data, was "CTkTable-0.4.tar", last modified: Fri Jun 23 15:42:40 2023, max compression
```

## Comparing `CTkTable-0.3.tar` & `CTkTable-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 11:05:05.796499 CTkTable-0.3/
-drwxrwxrwx   0        0        0        0 2023-06-22 11:05:05.756533 CTkTable-0.3/CTkTable/
--rw-rw-rw-   0        0        0      227 2023-06-22 10:58:22.000000 CTkTable-0.3/CTkTable/__init__.py
--rw-rw-rw-   0        0        0    11112 2023-06-22 10:59:10.000000 CTkTable-0.3/CTkTable/ctktable.py
-drwxrwxrwx   0        0        0        0 2023-06-22 11:05:05.786351 CTkTable-0.3/CTkTable.egg-info/
--rw-rw-rw-   0        0        0     3348 2023-06-22 11:05:05.000000 CTkTable-0.3/CTkTable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-22 11:05:05.000000 CTkTable-0.3/CTkTable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2023-06-22 11:05:05.000000 CTkTable-0.3/CTkTable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-22 11:05:05.000000 CTkTable-0.3/CTkTable.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 11:05:05.000000 CTkTable-0.3/CTkTable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkTable-0.3/LICENSE
--rw-rw-rw-   0        0        0     3348 2023-06-22 11:05:05.796499 CTkTable-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2762 2023-06-22 11:03:43.000000 CTkTable-0.3/README.md
--rw-rw-rw-   0        0        0      519 2023-06-22 11:05:05.796499 CTkTable-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1036 2023-06-22 11:04:09.000000 CTkTable-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 15:42:40.037660 CTkTable-0.4/
+drwxrwxrwx   0        0        0        0 2023-06-23 15:42:40.013694 CTkTable-0.4/CTkTable/
+-rw-rw-rw-   0        0        0      227 2023-06-23 15:30:21.000000 CTkTable-0.4/CTkTable/__init__.py
+-rw-rw-rw-   0        0        0    12702 2023-06-23 15:40:44.000000 CTkTable-0.4/CTkTable/ctktable.py
+drwxrwxrwx   0        0        0        0 2023-06-23 15:42:40.035697 CTkTable-0.4/CTkTable.egg-info/
+-rw-rw-rw-   0        0        0     3348 2023-06-23 15:42:39.000000 CTkTable-0.4/CTkTable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-23 15:42:39.000000 CTkTable-0.4/CTkTable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-06-23 15:42:39.000000 CTkTable-0.4/CTkTable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-23 15:42:39.000000 CTkTable-0.4/CTkTable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 15:42:39.000000 CTkTable-0.4/CTkTable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1067 2023-06-21 11:17:36.000000 CTkTable-0.4/LICENSE
+-rw-rw-rw-   0        0        0     3348 2023-06-23 15:42:40.038086 CTkTable-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2762 2023-06-22 11:03:43.000000 CTkTable-0.4/README.md
+-rw-rw-rw-   0        0        0      519 2023-06-23 15:42:40.043083 CTkTable-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2023-06-23 15:41:59.000000 CTkTable-0.4/setup.py
```

### Comparing `CTkTable-0.3/CTkTable/ctktable.py` & `CTkTable-0.4/CTkTable/ctktable.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,20 +12,28 @@
         master: any,
         row: int = None,
         column: int = None,
         padx: int = 1, 
         pady: int = 0,
         values: list = [[None]],
         colors: list = [None, None],
+        orientation: str = "horizontal",
         color_phase: str = "horizontal",
+        border_width: int = 0,
+        text_color: str = None,
+        border_color: str = None,
+        font: tuple = None,
         header_color: str = None,
         corner_radius: int = 25,
-        hover_color: str = None,
         write: str = False,
         command = None,
+        anchor = "c",
+        hover_color = None,
+        hover = False,
+        justify = "center",
         **kwargs):
         
         super().__init__(master, fg_color="transparent")
 
         self.master = master # parent widget
         self.rows = row if row else len(values) # number of default rows
         self.columns = column if column else len(values[0])# number of default columns
@@ -33,16 +41,28 @@
         self.pady = pady
         self.command = command
         self.values = values # the default values of the table
         self.colors = colors # colors of the table if required
         self.header_color = header_color # specify the topmost row color
         self.phase = color_phase
         self.corner = corner_radius
-        self.hover_color = hover_color
         self.write = write
+        self.justify = justify
+        if self.write:
+            border_width = border_width=+1
+        if hover_color:
+            hover=True
+        self.anchor = anchor
+        self.hover = hover
+        self.border_width = border_width
+        self.hover_color = customtkinter.ThemeManager.theme["CTkButton"]["hover_color"] if hover_color is None else hover_color
+        self.orient = orientation
+        self.border_color = customtkinter.ThemeManager.theme["CTkButton"]["border_color"] if border_color is None else border_color
+        self.text_color = customtkinter.ThemeManager.theme["CTkButton"]["text_color"] if text_color is None else text_color
+        self.font = font
         # if colors are None then use the default frame colors:
         self.data = {}
         self.fg_color = customtkinter.ThemeManager.theme["CTkFrame"]["fg_color"] if not self.colors[0] else self.colors[0]
         self.fg_color2 = customtkinter.ThemeManager.theme["CTkFrame"]["top_fg_color"] if not self.colors[1] else self.colors[1]
 
         if self.colors[0] is None and self.colors[1] is None:
             if self.fg_color==self.master.cget("fg_color"):
@@ -50,15 +70,15 @@
             if self.fg_color2==self.master.cget("fg_color"):
                 self.fg_color2 = customtkinter.ThemeManager.theme["CTk"]["fg_color"]
             
         self.frame = {}
         self.draw_table(**kwargs)
         
     def draw_table(self, **kwargs):
-
+        
         """ draw the table """
         for i in range(self.rows):
             for j in range(self.columns):
                 if self.phase=="horizontal":
                     if i%2==0:
                         fg = self.fg_color
                     else:
@@ -66,24 +86,21 @@
                 else:
                     if j%2==0:
                         fg = self.fg_color
                     else:
                         fg = self.fg_color2
                         
                 if self.header_color:
-                    if i==0:
-                        fg = self.header_color
-                        
-                if not self.hover_color:
-                    hover_color = fg
-                    hover = False
-                else:
-                    hover_color = self.hover_color
-                    hover = True
-                    
+                    if self.orient=="horizontal":
+                        if i==0:
+                            fg = self.header_color
+                    else:
+                        if j==0:
+                            fg = self.header_color
+
                 corner_radius = self.corner    
                 if i==0 and j==0:
                     corners = ["", fg, fg, fg]
                 elif i==self.rows-1 and j==self.columns-1:
                     corners = [fg ,fg, "", fg]
                 elif i==self.rows-1 and j==0:
                     corners = [fg ,fg, fg, ""]
@@ -91,47 +108,56 @@
                     corners = [fg , "", fg, fg]
                 else:
                     corners = [fg, fg, fg, fg]
                     corner_radius = 0
                     
                 if self.values:
                     try:
-                        value = self.values[i][j]
+                        if self.orient=="horizontal":
+                            value = self.values[i][j]
+                        else:
+                            value = self.values[j][i]
                     except IndexError: value = " "
                 else:
                     value = " "
 
                 if (i,j) in self.data.keys():
                     if self.data[i,j]["args"]: 
                         args = self.data[i,j]["args"]
                     else:
                         args = kwargs
                 else:
                     args = kwargs
-                    
+                
                 self.data[i,j] = {"row": i, "column" : j, "value" : value, "args": args }
               
                 args = self.data[i,j]["args"]
                 
                 if self.write:
                     if self.padx==1: self.padx=0
-                    self.frame[i,j] = customtkinter.CTkEntry(self,
+                    self.frame[i,j] = customtkinter.CTkEntry(self, border_width=self.border_width,
+                                                             text_color=self.text_color,
+                                                             border_color=self.border_color,
+                                                             font=self.font, justify=self.justify,
                                                              corner_radius=0,
                                                              fg_color=fg, **args)
                     self.frame[i,j].insert("0", value)
                     self.frame[i,j].bind("<Key>", lambda e, row=i, column=j, data=self.data: self.after(100, lambda: self.manipulate_data(row, column)))
                     self.frame[i,j].grid(column=j, row=i, padx=self.padx, pady=self.pady, sticky="nsew")
                     if self.header_color:
                         if i==0:
                             self.frame[i,j].configure(state="readonly")
     
                 else:
                     self.frame[i,j] = customtkinter.CTkButton(self, background_corner_colors=corners,
-                                                              corner_radius=corner_radius, hover=hover,
-                                                              fg_color=fg, hover_color=hover_color, text=value,
+                                                              text_color=self.text_color, anchor=self.anchor,
+                                                              border_color=self.border_color,
+                                                              font=self.font, border_width=self.border_width,
+                                                              corner_radius=corner_radius, hover=self.hover,
+                                                              fg_color=fg, text=value, hover_color=self.hover_color,
                                                               command=(lambda e=self.data[i,j]: self.command(e)) if self.command else None, **args)
                     self.frame[i,j].grid(column=j, row=i, padx=self.padx, pady=self.pady, sticky="nsew")
                 
                 self.rowconfigure(i, weight=1)
                 self.columnconfigure(j, weight=1)
                 
     def manipulate_data(self, row, column):
@@ -185,15 +211,15 @@
         self.frame = {}
         if index is None:
             index = len(self.values)      
         try:
             self.values.insert(index, values)
             self.rows+=1
         except IndexError: pass
-    
+ 
         self.draw_table(**kwargs)
         self.update_data()
         
     def add_column(self, values, index=None, **kwargs):
         """ add a new column """
         for i in self.frame.values():
             i.destroy()
```

### Comparing `CTkTable-0.3/CTkTable.egg-info/PKG-INFO` & `CTkTable-0.4/CTkTable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkTable
-Version: 0.3
+Version: 0.4
 Summary: Customtkinter Table widget
 Home-page: https://github.com/Akascape/CTkTable
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,table-widget,table,ctktable,tabular-data,customtkinter-table
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkTable-0.3/LICENSE` & `CTkTable-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkTable-0.3/PKG-INFO` & `CTkTable-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkTable
-Version: 0.3
+Version: 0.4
 Summary: Customtkinter Table widget
 Home-page: https://github.com/Akascape/CTkTable
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,table-widget,table,ctktable,tabular-data,customtkinter-table
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CTkTable-0.3/README.md` & `CTkTable-0.4/README.md`

 * *Files identical despite different names*

### Comparing `CTkTable-0.3/setup.cfg` & `CTkTable-0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 5461 626c 650d 0a76 6572   = CTkTable..ver
-00000020: 7369 6f6e 203d 2030 2e33 0d0a 6465 7363  sion = 0.3..desc
+00000020: 7369 6f6e 203d 2030 2e34 0d0a 6465 7363  sion = 0.4..desc
 00000030: 7269 7074 696f 6e20 3d20 4375 7374 6f6d  ription = Custom
 00000040: 746b 696e 7465 7220 5461 626c 6520 7769  tkinter Table wi
 00000050: 6467 6574 0d0a 6c6f 6e67 5f64 6573 6372  dget..long_descr
 00000060: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000070: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000080: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
 00000090: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
```

### Comparing `CTkTable-0.3/setup.py` & `CTkTable-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkTable',
-    version = '0.3',
+    version = '0.4',
     description = "Customtkinter Table widget",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkTable",
```

