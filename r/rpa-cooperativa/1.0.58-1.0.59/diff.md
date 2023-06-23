# Comparing `tmp/rpa_cooperativa-1.0.58.tar.gz` & `tmp/rpa_cooperativa-1.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.58.tar", last modified: Fri Jun 23 12:07:39 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.59.tar", last modified: Fri Jun 23 12:23:13 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.58.tar` & `rpa_cooperativa-1.0.59.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 12:07:39.332205 rpa_cooperativa-1.0.58/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.58/LICENSE
--rw-rw-rw-   0        0        0     6875 2023-06-23 12:07:39.327649 rpa_cooperativa-1.0.58/PKG-INFO
--rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.58/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 12:07:39.086718 rpa_cooperativa-1.0.58/rpa_coop/
--rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.58/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 12:07:39.229758 rpa_cooperativa-1.0.58/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.58/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.58/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.58/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.58/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.58/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.58/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.58/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.58/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.58/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.58/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.58/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    88098 2023-06-23 12:06:39.000000 rpa_cooperativa-1.0.58/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-06-23 12:07:39.315554 rpa_cooperativa-1.0.58/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6875 2023-06-23 12:07:38.000000 rpa_cooperativa-1.0.58/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-06-23 12:07:38.000000 rpa_cooperativa-1.0.58/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 12:07:38.000000 rpa_cooperativa-1.0.58/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 12:07:38.000000 rpa_cooperativa-1.0.58/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      567 2023-06-23 12:07:38.000000 rpa_cooperativa-1.0.58/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 12:07:38.000000 rpa_cooperativa-1.0.58/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 12:07:39.334205 rpa_cooperativa-1.0.58/setup.cfg
--rw-rw-rw-   0        0        0     2336 2023-06-23 12:07:14.000000 rpa_cooperativa-1.0.58/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:23:13.763791 rpa_cooperativa-1.0.59/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.59/LICENSE
+-rw-rw-rw-   0        0        0     6875 2023-06-23 12:23:13.757853 rpa_cooperativa-1.0.59/PKG-INFO
+-rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.59/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 12:23:13.550107 rpa_cooperativa-1.0.59/rpa_coop/
+-rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.59/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:23:13.665992 rpa_cooperativa-1.0.59/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.59/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.59/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.59/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.59/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.59/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.59/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.59/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.59/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.59/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.59/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.59/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    88164 2023-06-23 12:22:08.000000 rpa_cooperativa-1.0.59/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:23:13.748857 rpa_cooperativa-1.0.59/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6875 2023-06-23 12:23:13.000000 rpa_cooperativa-1.0.59/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-06-23 12:23:13.000000 rpa_cooperativa-1.0.59/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 12:23:13.000000 rpa_cooperativa-1.0.59/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-23 12:23:13.000000 rpa_cooperativa-1.0.59/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      567 2023-06-23 12:23:13.000000 rpa_cooperativa-1.0.59/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 12:23:13.000000 rpa_cooperativa-1.0.59/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 12:23:13.764838 rpa_cooperativa-1.0.59/setup.cfg
+-rw-rw-rw-   0        0        0     2336 2023-06-23 12:22:54.000000 rpa_cooperativa-1.0.59/setup.py
```

### Comparing `rpa_cooperativa-1.0.58/LICENSE` & `rpa_cooperativa-1.0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.58/PKG-INFO` & `rpa_cooperativa-1.0.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.58
+Version: 1.0.59
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.58/README.md` & `rpa_cooperativa-1.0.59/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.58/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.59/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.58/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.59/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.58/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.59/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.58/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.59/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.58/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.59/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.58/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.59/rpa_coop/rpa_coop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1282,52 +1282,54 @@
         self.janela_siat = janela
         self.janela_siac = janela
         
         opcoes = [x.upper() for x in opcoes]
         
         for menu in opcoes:
             janela.activate()
-            time.sleep(1)
             self.p.press('pgdn')
             time.sleep(1)
             
             if menu == 'SACG':
                 # Abrir SACG
                 try:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_branco.png', confidence=0.9, grayscale=True)
                 except:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_verde.png', confidence=0.9, grayscale=True)
                 self.p.doubleClick(posicao)
                 time.sleep(7)
                 self.janela_sacg = self.p.getWindowsWithTitle('teoff-exe')[num_menu]
                 self.janelas.append(self.janela_sacg)
                 print('clicou no menu: sacg')
+                time.sleep(3)
                 # self.janela_sacg.activate()
             elif menu == 'SIAT':
                 # Abrir SIAT
                 try:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siat_amarelo.png', confidence=0.9, grayscale=True)
                 except:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siat_branco.png', confidence=0.9, grayscale=True)
                 self.p.doubleClick(posicao)
                 time.sleep(7)
                 self.janela_siat = self.p.getWindowsWithTitle('teoff-exe')[num_menu] 
                 self.janelas.append(self.janela_siat)
                 print('clicou no menu: siat')
+                time.sleep(3)
                 # self.janela_siat.activate()
             elif menu == 'SIAC':
                 try:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siac_branco.png', confidence=0.9, grayscale=True)
                 except:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siac_amarelo.png', confidence=0.9, grayscale=True)
                 self.p.doubleClick(posicao)
                 time.sleep(7)
                 self.janela_siac = self.p.getWindowsWithTitle('teoff-exe')[num_menu]
                 self.janelas.append(self.janela_siac)
                 print('clicou no menu: siac')
+                time.sleep(3)
                 # self.janela_siac.activate()
             time.sleep(1)
         return self.janelas
 
              
     def select_menu_letras(self, letras, nome_janela=None):
         '''acc.select_menu_letras(letras) \n
```

### Comparing `rpa_cooperativa-1.0.58/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.59/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.58
+Version: 1.0.59
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.58/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.59/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.58/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.59/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.58/setup.py` & `rpa_cooperativa-1.0.59/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.58",
+    version="1.0.59",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

