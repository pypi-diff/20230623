# Comparing `tmp/mathpub-0.1.2.tar.gz` & `tmp/mathpub-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathpub-0.1.2.tar", last modified: Fri Jun 23 19:38:57 2023, max compression
+gzip compressed data, was "mathpub-0.1.3.tar", last modified: Fri Jun 23 20:32:04 2023, max compression
```

## Comparing `mathpub-0.1.2.tar` & `mathpub-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 19:38:57.310004 mathpub-0.1.2/
--rw-rw-rw-   0        0        0      200 2023-06-23 19:38:57.310997 mathpub-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-23 19:38:57.261999 mathpub-0.1.2/mathpub/
--rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.1.2/mathpub/__init__.py
--rw-rw-rw-   0        0        0     3091 2023-06-23 19:38:53.000000 mathpub-0.1.2/mathpub/page.py
--rw-rw-rw-   0        0        0     3321 2023-06-23 18:29:55.000000 mathpub-0.1.2/mathpub/text_processing.py
--rw-rw-rw-   0        0        0     1590 2023-06-22 23:10:58.000000 mathpub-0.1.2/mathpub/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:38:57.308000 mathpub-0.1.2/mathpub.egg-info/
--rw-rw-rw-   0        0        0      200 2023-06-23 19:38:56.000000 mathpub-0.1.2/mathpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-23 19:38:57.000000 mathpub-0.1.2/mathpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 19:38:56.000000 mathpub-0.1.2/mathpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 18:44:47.000000 mathpub-0.1.2/mathpub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-06-23 19:38:57.000000 mathpub-0.1.2/mathpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 19:38:57.311997 mathpub-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      295 2023-06-23 19:38:53.000000 mathpub-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:32:04.460312 mathpub-0.1.3/
+-rw-rw-rw-   0        0        0      200 2023-06-23 20:32:04.460312 mathpub-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-23 20:32:04.448293 mathpub-0.1.3/mathpub/
+-rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.1.3/mathpub/__init__.py
+-rw-rw-rw-   0        0        0     3199 2023-06-23 20:31:57.000000 mathpub-0.1.3/mathpub/page.py
+-rw-rw-rw-   0        0        0     3321 2023-06-23 18:29:55.000000 mathpub-0.1.3/mathpub/text_processing.py
+-rw-rw-rw-   0        0        0     1592 2023-06-23 20:31:57.000000 mathpub-0.1.3/mathpub/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:32:04.458270 mathpub-0.1.3/mathpub.egg-info/
+-rw-rw-rw-   0        0        0      200 2023-06-23 20:32:03.000000 mathpub-0.1.3/mathpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-23 20:32:03.000000 mathpub-0.1.3/mathpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 20:32:03.000000 mathpub-0.1.3/mathpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-23 18:44:47.000000 mathpub-0.1.3/mathpub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-23 20:32:03.000000 mathpub-0.1.3/mathpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 20:32:04.461713 mathpub-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      295 2023-06-23 20:31:57.000000 mathpub-0.1.3/setup.py
```

### Comparing `mathpub-0.1.2/mathpub/page.py` & `mathpub-0.1.3/mathpub/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,22 @@
     def repr_latex(self):
         return repr(self.str_latex())
 
     def _display_unchanged(self):
         display(Latex(self.str_latex()))
 
     def _display_changed(self):
+        class ReprString(str):
+            def __repr__(self):
+                return self
+
         before_checkpoint = ''.join(x.latex() for x in self.lines[:self._last_length])
         if before_checkpoint:
             display(Latex("$" + before_checkpoint + "$"))
-        display("-------Checkpoint-------")
+        display(ReprString("-------Checkpoint-------"))
         after_checkpoint = "$" + ''.join(x.latex() for x in self.lines[self._last_length:]) + "$"
         display(Latex(after_checkpoint))
 
         if self.interactive_buttons:
             checkpoint_button = Button(description="Checkpoint")
             checkpoint_button.style.button_color = "lightgreen"
             checkpoint_button.on_click(lambda b: (self.checkpoint(), clear_output(), self._display_unchanged()))
```

### Comparing `mathpub-0.1.2/mathpub/text_processing.py` & `mathpub-0.1.3/mathpub/text_processing.py`

 * *Files identical despite different names*

### Comparing `mathpub-0.1.2/mathpub/utils.py` & `mathpub-0.1.3/mathpub/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     return f"\\overline{br(ins)}"
 
 
 def lower_index(ind):
     return f"_{br(ind)}"
 
 
-def upper_ind(ind):
+def upper_index(ind):
     return f"^{br(ind)}"
 
 
 def lr(ins, left, right):
     """Wraps \\left and \\right (with delimiters left and right respectively) around ins """
     return f"\\left {left} {ins} \\right {right}"
```

