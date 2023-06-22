# Comparing `tmp/econdata-1.0.4.tar.gz` & `tmp/econdata-1.0.5.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econdata-1.0.4.tar", last modified: Thu Jun  8 06:51:51 2023, max compression
+gzip compressed data, was "econdata-1.0.5.post0.tar", last modified: Thu Jun 22 23:08:58 2023, max compression
```

## Comparing `econdata-1.0.4.tar` & `econdata-1.0.5.post0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 06:51:51.660580 econdata-1.0.4/
--rw-rw-rw-   0        0        0     2251 2023-06-08 06:51:51.660580 econdata-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1779 2023-06-08 06:49:59.000000 econdata-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 06:51:51.661593 econdata-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-06-08 06:49:43.000000 econdata-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 06:51:51.641646 econdata-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 06:51:51.651313 econdata-1.0.4/src/econdata/
--rw-rw-rw-   0        0        0     6314 2023-06-08 06:47:58.000000 econdata-1.0.4/src/econdata/BCRP.py
--rw-rw-rw-   0        0        0     2820 2023-06-08 06:47:12.000000 econdata-1.0.4/src/econdata/BM.py
--rw-rw-rw-   0        0        0     4008 2023-06-08 06:47:12.000000 econdata-1.0.4/src/econdata/FRED.py
--rw-rw-rw-   0        0        0     2112 2023-06-08 06:47:12.000000 econdata-1.0.4/src/econdata/OECD.py
--rw-rw-rw-   0        0        0     3592 2023-06-08 06:47:12.000000 econdata-1.0.4/src/econdata/YFinance.py
--rw-rw-rw-   0        0        0        0 2023-06-08 06:47:12.000000 econdata-1.0.4/src/econdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 06:51:51.659580 econdata-1.0.4/src/econdata.egg-info/
--rw-rw-rw-   0        0        0     2251 2023-06-08 06:51:51.000000 econdata-1.0.4/src/econdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-06-08 06:51:51.000000 econdata-1.0.4/src/econdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 06:51:51.000000 econdata-1.0.4/src/econdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-08 06:51:51.000000 econdata-1.0.4/src/econdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-08 06:51:51.000000 econdata-1.0.4/src/econdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 23:08:58.515198 econdata-1.0.5.post0/
+-rw-rw-rw-   0        0        0     2358 2023-06-22 23:08:58.514201 econdata-1.0.5.post0/PKG-INFO
+-rw-rw-rw-   0        0        0     1880 2023-06-22 22:56:18.000000 econdata-1.0.5.post0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 23:08:58.515198 econdata-1.0.5.post0/setup.cfg
+-rw-rw-rw-   0        0        0      910 2023-06-22 22:56:20.000000 econdata-1.0.5.post0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:08:58.500238 econdata-1.0.5.post0/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 23:08:58.508216 econdata-1.0.5.post0/src/econdata/
+-rw-rw-rw-   0        0        0     6390 2023-06-22 22:25:48.000000 econdata-1.0.5.post0/src/econdata/BCRP.py
+-rw-rw-rw-   0        0        0     4034 2023-06-22 22:24:06.000000 econdata-1.0.5.post0/src/econdata/FRED.py
+-rw-rw-rw-   0        0        0     4272 2023-06-22 23:04:50.000000 econdata-1.0.5.post0/src/econdata/IMF.py
+-rw-rw-rw-   0        0        0     2154 2023-06-22 22:24:57.000000 econdata-1.0.5.post0/src/econdata/OECD.py
+-rw-rw-rw-   0        0        0     2826 2023-06-22 22:17:31.000000 econdata-1.0.5.post0/src/econdata/WB.py
+-rw-rw-rw-   0        0        0     3599 2023-06-22 22:17:39.000000 econdata-1.0.5.post0/src/econdata/YFinance.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 22:17:31.000000 econdata-1.0.5.post0/src/econdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:08:58.513204 econdata-1.0.5.post0/src/econdata.egg-info/
+-rw-rw-rw-   0        0        0     2358 2023-06-22 23:08:58.000000 econdata-1.0.5.post0/src/econdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-06-22 23:08:58.000000 econdata-1.0.5.post0/src/econdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 23:08:58.000000 econdata-1.0.5.post0/src/econdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-22 23:08:58.000000 econdata-1.0.5.post0/src/econdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 23:08:58.000000 econdata-1.0.5.post0/src/econdata.egg-info/top_level.txt
```

### Comparing `econdata-1.0.4/PKG-INFO` & `econdata-1.0.5.post0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,30 @@
-Metadata-Version: 2.1
-Name: econdata
-Version: 1.0.4
-Summary: Extracción de series de tiempo de las principales instituciones económicas para el Perú
-Home-page: https://github.com/mauricioalvaradoo/econdata
-Author: Mauricio Alvarado, Andrei Romero
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # Econdata
 Extracción de series de tiempo de las principales instituciones económicas para el Perú:
 1. Banco Central de Reserva del Perú (BCRP)
-2. Yahoo Finance
+2. Yahoo Finance (YFinance)
 3. Federal Reserve Economic Data (FRED)
-4. World Bank
-5. Organización para la Cooperación y el Desarrollo Económicos (OCDE)
+4. World Bank (WB)
+5. Organization for Economic Cooperation and Development (OECD)
+6. International Monetary Fund (IMF)
 
 ```
 # Instalación mediante PyPI
-!pip install econdata==1.0.4
+!pip install econdata==1.0.5-r
 
 # o simplemente:
 !pip install econdata
 ```
 El anuncio fue realizado en Linkedin, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
 
-## Versión 1.0.4
-* Para el `BCRP`, `Yahoo Finance`, `FRED` y el `World Bank`, se cuenta con ambos métodos: `get_data()` y `search()`.
-* Para la `OCDE`, se cuenta únicamente con el método `get_data()`.
-* En la versión 1.0.4, (i) se corrigió el formato de las fechas para `BCRP` y `FRED`, y (ii) se añadió el filtro de frecuencia en `search()` para `FRED`.
+## Versión 1.0.5-r
+* Para el `BCRP`, `YFinance`, `FRED`, `IMF` y el `WB`, se cuenta con ambos métodos: `get_data()` y `search()`.
+* Para la `OECD`, se cuenta únicamente con el método `get_data()`.
+* En la versión 1.0.5-r, se incluyó el `IMF`.
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
 get_data()
 ```
@@ -48,11 +37,16 @@
 
 
 ## Test !
 El código guía para usar las funciones está disponible [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/test.py).
 El video del anuncio de la librería y la demo está disponible [aquí](https://www.youtube.com/watch?v=etaqHMDfvtE).
 
 
+## Macroeconomic Dataset
+Se elaboró un dataset de series macroeconómicas [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/macro-dataset.py).
+
+
+
 ## Créditos
 * [Mauricio Alvarado](https://github.com/mauricioalvaradoo)
 * [Andrei Romero](https://github.com/Ixtalia)
```

### Comparing `econdata-1.0.4/README.md` & `econdata-1.0.5.post0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,42 @@
+Metadata-Version: 2.1
+Name: econdata
+Version: 1.0.5.post0
+Summary: Extracción de series de tiempo de las principales instituciones económicas para el Perú
+Home-page: https://github.com/mauricioalvaradoo/econdata
+Author: Mauricio Alvarado, Andrei Romero
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # Econdata
 Extracción de series de tiempo de las principales instituciones económicas para el Perú:
 1. Banco Central de Reserva del Perú (BCRP)
-2. Yahoo Finance
+2. Yahoo Finance (YFinance)
 3. Federal Reserve Economic Data (FRED)
-4. World Bank
-5. Organización para la Cooperación y el Desarrollo Económicos (OCDE)
+4. World Bank (WB)
+5. Organization for Economic Cooperation and Development (OECD)
+6. International Monetary Fund (IMF)
 
 ```
 # Instalación mediante PyPI
-!pip install econdata==1.0.4
+!pip install econdata==1.0.5-r
 
 # o simplemente:
 !pip install econdata
 ```
 El anuncio fue realizado en Linkedin, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
 
-## Versión 1.0.4
-* Para el `BCRP`, `Yahoo Finance`, `FRED` y el `World Bank`, se cuenta con ambos métodos: `get_data()` y `search()`.
-* Para la `OCDE`, se cuenta únicamente con el método `get_data()`.
-* En la versión 1.0.4, (i) se corrigió el formato de las fechas para `BCRP` y `FRED`, y (ii) se añadió el filtro de frecuencia en `search()` para `FRED`.
+## Versión 1.0.5-r
+* Para el `BCRP`, `YFinance`, `FRED`, `IMF` y el `WB`, se cuenta con ambos métodos: `get_data()` y `search()`.
+* Para la `OECD`, se cuenta únicamente con el método `get_data()`.
+* En la versión 1.0.5-r, se incluyó el `IMF`.
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
 get_data()
 ```
@@ -36,11 +49,16 @@
 
 
 ## Test !
 El código guía para usar las funciones está disponible [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/test.py).
 El video del anuncio de la librería y la demo está disponible [aquí](https://www.youtube.com/watch?v=etaqHMDfvtE).
 
 
+## Macroeconomic Dataset
+Se elaboró un dataset de series macroeconómicas [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/macro-dataset.py).
+
+
+
 ## Créditos
 * [Mauricio Alvarado](https://github.com/mauricioalvaradoo)
 * [Andrei Romero](https://github.com/Ixtalia)
```

### Comparing `econdata-1.0.4/setup.py` & `econdata-1.0.5.post0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='econdata',
-    version = '1.0.4',
+    version = '1.0.5-r',
     author = 'Mauricio Alvarado, Andrei Romero',
     description = 'Extracción de series de tiempo de las principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mauricioalvaradoo/econdata',
     classifiers = [
         'Programming Language :: Python :: 3',
```

### Comparing `econdata-1.0.4/src/econdata/BCRP.py` & `econdata-1.0.5.post0/src/econdata/BCRP.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import pandas as pd
 import requests
 
 
 
 def get_data(series, fechaini, fechafin):
 
-    """ Importar multiples series de la API del BCRP
-    Considerar que las series deben ser de la misma frecuencia
+    ''' Importar multiples series de la API del BCRP.
+    Considerar que las series deben ser de la misma frecuencia.
     
     Parámetros
     ----------
     series: dict
-        Diccionario de los códigos y nombres de las series
+        Diccionario de los códigos y nombres de las series.
     fechaini: datetime
-        Fecha de inicio de la serie:
+        Fecha de inicio de la serie.
     fechafin: datetime
-        Fecha de fin de la serie
+        Fecha de fin de la serie.
         
     Retorno
     ----------
     df: pd.DataFrame
-        Series consultadas
+        Series consultadas.
     
     Ejemplo
     ----------
     Formatos para fechas:
     >>> Diario: yyyy-mm-dd
     >>> Mensual: yyyy-mm
     >>> Trimestral: yyyyQq
@@ -49,176 +49,178 @@
     Documentación
     ----------
     https://estadisticas.bcrp.gob.pe/estadisticas/series/ayuda/api
     
 
     @author: Mauricio Alvarado
     
-    """
+    '''
 
     keys = list(series.keys())
     
     
     df = pd.DataFrame()
-    base = "https://estadisticas.bcrp.gob.pe/estadisticas/series/api"
+    base = 'https://estadisticas.bcrp.gob.pe/estadisticas/series/api'
         
 
     for i in keys:
-        url = f"{base}/{i}/json/{fechaini}/{fechafin}/ing"
+        url = f'{base}/{i}/json/{fechaini}/{fechafin}/ing'
 
         r = requests.get(url)
         
         if r.status_code == 200:
             pass
         else:
-            print("Vinculacion inválida!")
+            print('Vinculacion inválida!')
             break
         
-        response = r.json().get("periods")
+        response = r.json().get('periods')
         
         list_values = []
         list_time = []
                 
         for j in response:
-            list_values.append(float(j["values"][0]))    
-            list_time.append(j["name"])
+            list_values.append(float(j['values'][0]))    
+            list_time.append(j['name'])
 
         # Merge
-        dic = pd.DataFrame({"time": list_time, f"{i}": list_values})                      
-        df = pd.concat([df, dic]) if df.empty is True else pd.merge(df, dic, how="outer")
+        dic = pd.DataFrame({'time': list_time, f'{i}': list_values})                      
+        df = pd.concat([df, dic]) if df.empty is True else pd.merge(df, dic, how='outer')
         
-    df.set_index("time", inplace=True)
+    df.set_index('time', inplace=True)
     df.rename(series, axis=1, inplace=True)
 
 
     # Formatos de fechas
     if keys[0][-1] == 'D':
         df.index = df.index.str.replace('Set', 'Sep')
-        df.index = pd.to_datetime(df.index, format="%d.%b.%y")
+        df.index = pd.to_datetime(df.index, format='%d.%b.%y')
     if keys[0][-1] == 'M':
         df.index = df.index.str.replace('Set', 'Sep')
-        df.index = pd.to_datetime(df.index, format="%b.%Y")
+        df.index = pd.to_datetime(df.index, format='%b.%Y')
     if keys[0][-1] == 'Q':
         try:
-            df.index = pd.period_range(fechaini, fechafin, freq="Q")
+            df.index = pd.period_range(fechaini, fechafin, freq='Q')
         except: 
             try: # Hasta fecha fin Q4
-                df.index = pd.period_range(fechaini, fechafin[:4]+'Q4', freq="Q")
+                df.index = pd.period_range(fechaini, fechafin[:4]+'Q4', freq='Q')
             except: # Aumentando un año para series en var. %
                 try:
                     newanio = str( int(fechaini[:4])+1 )
-                    df.index = pd.period_range(newanio+fechaini[4:], fechafin, freq="Q")
+                    df.index = pd.period_range(newanio+fechaini[4:], fechafin, freq='Q')
                 except:  
                     try: # Aumentando un año para series en var. % y hasta fechafin Q4 
                         newanio = str( int(fechaini[:4])+1 )
-                        df.index = pd.period_range(newanio+fechaini[4:], fechafin[:4]+'Q4', freq="Q")
+                        df.index = pd.period_range(newanio+fechaini[4:], fechafin[:4]+'Q4', freq='Q')
                     except:
                         pass
+    
+    df.sort_index(inplace=True) # Ordenamiento de fechas
 
     return df
 
 
 
 def metadatos():
 
-    metadatos = "https://raw.githubusercontent.com/mauricioalvaradoo/econdata/master/src/econdata/metadata/BCRPData-metadata.csv"
+    metadatos = 'https://raw.githubusercontent.com/mauricioalvaradoo/econdata/master/src/econdata/metadata/BCRPData-metadata.csv'
     df = pd.read_csv(metadatos, index_col=0, sep=";", encoding="latin-1").reset_index()
-    df = df[["Código de serie", "Grupo de serie", "Nombre de serie", "Frecuencia", "Fecha de inicio", "Fecha de fin"]]
+    df = df[['Código de serie', 'Grupo de serie', 'Nombre de serie', 'Frecuencia', 'Fecha de inicio', 'Fecha de fin']]
 
     return df
 
 
 
 def search(consulta, grupo=None, frecuencia=None):
 
-    """ Extraer código de la consulta
+    ''' Extraer código de la consulta.
     
     Parámetros
     ----------
     consulta: list
-        Palabras claves de las series
+        Palabras claves de las series.
     grupo: list
-        Palabras claves de los grupos. Default: None
+        Palabras claves de los grupos. Default: None.
     frecuencia: str
         Frecuencia de la serie consultada. Default: None.
-        >>> "Diaria"
-        >>> "Mensual"
-        >>> "Trimestral"
-        >>> "Anual"
+        >>> 'Diaria'
+        >>> 'Mensual'
+        >>> 'Trimestral'
+        >>> 'Anual'
 
     Retorno
     ----------
     df: pd.DataFrame
-        Metadatos de las series consultadas
+        Metadatos de las series consultadas.
     
     Documentación
     ----------
     https://estadisticas.bcrp.gob.pe/estadisticas/series/ayuda/metadatos
     
     
     @author: Mauricio Alvarado
     
-    """
+    '''
     
     df = metadatos()
     consulta = [x.lower() for x in consulta]
 
     # Frecuencia
     if frecuencia is not None:
         try:
-            df = df[df["Frecuencia"] == str(frecuencia)]
+            df = df[df['Frecuencia'] == str(frecuencia)]
         except:
             pass
     
     # Grupo
     if grupo is not None:
         grupo = [x.lower() for x in grupo]
         
         for i in grupo:
             try:
-                filter = df["Grupo de serie"].str.lower().str.contains(i)
+                filter = df['Grupo de serie'].str.lower().str.contains(i)
                 df = df[filter]
             except:
                 pass
 
     # Series
     for i in consulta:           
         try:
-            filter = df["Nombre de serie"].str.lower().str.contains(i)
+            filter = df['Nombre de serie'].str.lower().str.contains(i)
             df = df[filter]
         except:
-            df = print("Consulta no encontrada!")
+            df = print('Consulta no encontrada!')
     
-    df.set_index("Código de serie", inplace=True)
+    df.set_index('Código de serie', inplace=True)
     return df
 
 
 
 def documentation(code):
     
-    """ Extraer microdatos del código de la serie
+    ''' Extraer microdatos del código de la serie.
     
     Parámetros
     ----------
     code: str
-        Código base de la serie
+        Código base de la serie.
 
     Retorno
     ----------
     df: pd.DataFrame
-        Metadatos de las series consultadas
+        Metadatos de las series consultadas.
       
     Documentación
     ----------
     https://estadisticas.bcrp.gob.pe/estadisticas/series/ayuda/metadatos
     
     
     @author: Mauricio Alvarado
     
-    """
+    '''
 
     df = metadatos()
-    df = df[df["Código de serie"] == str(code)]
+    df = df[df['Código de serie'] == str(code)]
 
     return df
```

### Comparing `econdata-1.0.4/src/econdata/BM.py` & `econdata-1.0.5.post0/src/econdata/WB.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,115 +1,115 @@
 import pandas as pd
 import requests 
 
 
 
 def get_data(countries, indicator, fechaini, fechafin):
     
-    """ Importar múltiples series de la API del Banco Mundial
+    ''' Importar múltiples series de la API del Banco Mundial.
     
     Parámetros
     ----------
     countries: dict
-        Diccionario de los códigos y nombres de los países
-        >>>  countries = {"PE": "Perú"}   
+        Diccionario de los códigos y nombres de los países.
+        >>>  countries = {'PE': 'Perú'}   
     indicator: str
-        Código del indicador o serie
-        Se obtiene de: "https://datos.bancomundial.org/indicator/"        
+        Código del indicador o serie.
+        Se obtiene de: 'https://datos.bancomundial.org/indicator/'       
     fechaini: str
-        Fecha de inicio de la serie
+        Fecha de inicio de la serie.
         >>> Anual: yyyy
     fechafin: str
-        Fecha de fin de la serie
+        Fecha de fin de la serie.
         >>> Anual: yyyy
         
     Retorno
     ----------
     df: pd.DataFrame
         Países con las series consultadas.    
     
     Documentación
     ----------
     https://datahelpdesk.worldbank.org/knowledgebase/articles/898581-api-basic-call-structure
     
     
     @authors: Mauricio Alvarado, Norbert Andrei Romero Escobedo
 
-    """
+    '''
 
 
     keys = list(countries.keys())
     df = pd.DataFrame()
     
 
     for i in keys:
-        url = f"http://api.worldbank.org/v2/country/{i}/indicator/{indicator}?format=json"
+        url = f'http://api.worldbank.org/v2/country/{i}/indicator/{indicator}?format=json'
          
         r = requests.get(url) 
                 
         if r.status_code == 200:
             pass
         else:
-            print("Revisa los datos ingresados")
+            print('Revisa los datos ingresados')
             break
     
         response = r.json()[1]
     
         values_list = []
         time_list = []
     
         for j in response: 
-            values_list.append(j["value"])
-            time_list.append(j["date"])
+            values_list.append(j['value'])
+            time_list.append(j['date'])
         
         # Merge
-        dictio = pd.DataFrame({"time": time_list, f"{i}": values_list})
-        df = pd.concat([df, dictio]) if df.empty is True else pd.merge(df, dictio, how = "outer")
+        dictio = pd.DataFrame({'time': time_list, f'{i}': values_list})
+        df = pd.concat([df, dictio]) if df.empty is True else pd.merge(df, dictio, how = 'outer')
     
-    df.set_index("time", inplace = True)
+    df.set_index('time', inplace = True)
     df.sort_index(ascending=True, inplace=True)
     df.rename(countries, axis=1, inplace=True)
 
     df = df.loc[fechaini: fechafin]
     
     return df
       
           
       
       
 def search(consulta):
         
-    """ Extraer metadatos
+    ''' Extraer metadatos.
     
     Parámetros
     ----------
     consulta: list
-        Dos palabras clave de la consulta
+        Dos palabras clave de la consulta.
         
     Retorno: 
     ---------
     df: pd.DataFrame
-       Series consultadas
+       Series consultadas.
     
     @authors: Mauricio Alvarado, Norbert Andrei Romero Escobedo  
 
-    """
+    '''
 
 
-    formato = "%20".join(consulta)
+    formato = '%20'.join(consulta)
     formato = formato.lower()
    
-    url = f"http://api.worldbank.org/v2/sources/2/search/{formato}?format=json"
+    url = f'http://api.worldbank.org/v2/sources/2/search/{formato}?format=json'
     r = requests.get(url) 
-    response = r.json()["source"][0]["concept"][1]["variable"]
+    response = r.json()['source'][0]['concept'][1]['variable']
     
 
     list_id= []
     list_names= []
     
     for i in response: 
-        list_id.append(i["id"])
-        list_names.append(i["name"])
+        list_id.append(i['id'])
+        list_names.append(i['name'])
         
-    df= pd.DataFrame({ "id": list_id, "title": list_names})
+    df= pd.DataFrame({'id': list_id, 'title': list_names})
 
     return df
```

### Comparing `econdata-1.0.4/src/econdata/FRED.py` & `econdata-1.0.5.post0/src/econdata/FRED.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 
 import warnings
 warnings.simplefilter('ignore')
 
 
 def get_data(series, api_key, fechaini, fechafin):
     
-    """ Importar múltiples series de la API del FRED
+    ''' Importar múltiples series de la API del FRED.
     
     Parámetros
     ----------
     series: dict
-        Diccionario de los códigos y nombres de las series
+        Diccionario de los códigos y nombres de las series.
     api_key: str
         API Key del desarrollador: https://fred.stlouisfed.org/docs/api/api_key.html
     fechaini: str
-        Fecha de inicio de la serie  
+        Fecha de inicio de la serie.
     fechfin: str
-        Fecha de fin de la serie
+        Fecha de fin de la serie.
  
     Retorno 
     ----------
     df: pd.DataFrame
-       Series consultadas
+       Series consultadas.
     
     Ejemplo
     ----------
     Formatos para fechas:
     >>> Diario: yyyy-mm-dd
     >>> Mensual: yyyy-mm
     >>> Anual: yyyy   
@@ -36,99 +36,100 @@
     Documentación
     ----------
     https://fred.stlouisfed.org/docs/api/fred/
     
 
     @authors: Norbert Andrei Romero Escobedo, Mauricio Alvarado
     
-    """
+    '''
     
     
     keys = list(series.keys())
 
     df = pd.DataFrame()
     
     for i in keys:
-        url = f"https://api.stlouisfed.org/fred/series/observations?series_id={i}&api_key={api_key}&file_type=json"
+        url = f'https://api.stlouisfed.org/fred/series/observations?series_id={i}&api_key={api_key}&file_type=json'
     
         r = requests.get(url)
         
         if r.status_code == 200:
             pass
         else:
-            print("Porfavor, revisa los datos ingresados.")
+            print('Por favor, revisa los datos ingresados.')
             break
     
-        observations = r.json().get("observations")
+        observations = r.json().get('observations')
     
         list_values = []
         list_time = []
         
         for j in observations:
-            list_values.append(j["value"])
-            list_time.append(j["date"])
+            list_values.append(j['value'])
+            list_time.append(j['date'])
 
 
-        dictio = pd.DataFrame({"time": list_time, f"{i}": list_values})
-        df = dictio if df.empty is True else pd.merge(df, dictio, how = "outer")
+        dictio = pd.DataFrame({'time': list_time, f'{i}': list_values})
+        df = dictio if df.empty is True else pd.merge(df, dictio, how='outer')
 
-    df.set_index("time", inplace=True)
-    df.rename (series, axis = 1, inplace = True)
+    df.set_index('time', inplace=True)
+    df.rename(series, axis = 1, inplace = True)
     df = df.loc[fechaini: fechafin]
     
     # Corrigiendo '.' for missing values   
     for i in df.columns:
         try:
             df.loc[df[i] == '.', i] = np.nan
             df[i] = df[i].astype('float')
         except:
             pass
     
     # index to datetime
     df.index = pd.to_datetime(df.index)
+    df.sort_index(inplace=True)
 
     return df
 
 
 
 
 def search(consulta, api_key, frecuencia=None):
     
-    """ Extraer metadatos de las consultas
+    ''' Extraer metadatos de las .
 
     Parámetros
     ----------
     consulta: list
-        Palabras claves de las consultas  
+        Palabras claves de las consultas.
     api_key: str
         API Key del desarrollador: https://fred.stlouisfed.org/docs/api/api_key.html
     frecuencia: str
         Frecuencia de la serie consultada. Default: None.
         >>> "Daily"
         >>> "Monthly"
         >>> "Quarterly"
         >>> "Annual"
             
     Retorno
     ----------
     df: pd.DataFrame
-       Series consultadas
+       Series consultadas.
     
 
     @authors: Norbert Andrei Romero Escobedo, Mauricio Alvarado
     
-    """
+    '''
     
-    formato = "+".join(consulta)
+    formato = '+'.join(consulta)
     formato = formato.lower()
 
-    url = f"https://api.stlouisfed.org/fred/series/search?search_text={formato}&api_key={api_key}&file_type=json"
+    url = f'https://api.stlouisfed.org/fred/series/search?search_text={formato}&api_key={api_key}&file_type=json'
     r = requests.get(url) 
 
-    response = r.json()["seriess"]
+    response = r.json()['seriess']
 
     list_id = []
     list_title = []
     list_start = []
     list_end = []
     list_frequency = []
     list_seasonal_adjusment = []
@@ -138,25 +139,25 @@
         list_title.append(i['title'])
         list_start.append(i['observation_start'])
         list_end.append(i['observation_end'])
         list_frequency.append(i['frequency'])
         list_seasonal_adjusment.append(i['seasonal_adjustment'])
 
     df = pd.DataFrame({
-        "id": list_id,
-        "title": list_title,
-        "start": list_start,
-        "end": list_end,
-        "frequency": list_frequency,
-        "seasonal_adjusment": list_seasonal_adjusment
+        'id': list_id,
+        'title': list_title,
+        'start': list_start,
+        'end': list_end,
+        'frequency': list_frequency,
+        'seasonal_adjusment': list_seasonal_adjusment
     })
 
     if frecuencia is not None:
         try:
-            df = df[df["frequency"] == str(frecuencia)]
+            df = df[df['frequency'] == str(frecuencia)]
         except:
             pass
 
-    df.set_index("id", inplace=True) 
+    df.set_index('id', inplace=True) 
 
     return df
```

### Comparing `econdata-1.0.4/src/econdata/OECD.py` & `econdata-1.0.5.post0/src/econdata/OECD.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 import pandas as pd
 import requests 
 
 
 
 def get_data(identifier, countries, serie, fechaini, fechafin, periodicidad):
     
-    """ Importar multiples series de la API de la OCDE
+    ''' Importar multiples series de la API de la OCDE.
     
     Parámetros
     ----------
     identifier: str
-        Código identificador de la base de datos
+        Código identificador de la base de datos.
     countries: dict
-        Códigos y nombres de los países (keys, values)
+        Códigos y nombres de los países (keys, values).
     serie: str
-        Código de la serie
+        Código de la serie.
     fechaini: str
-        Fecha de inicio (yyyy-qq) 
+        Fecha de inicio (yyyy-qq) .
     fechafin: str
-        Fecha de fin (yyyy-qq) 
+        Fecha de fin (yyyy-qq).
     periodicidad: str
-        Frecuencia de los datos: "Q", "Y"    
+        Frecuencia de los datos: 'Q', 'Y'.  
     
     Retorno
     -------
     df: pd.DataFrame
-        Series consultadas
+        Series consultadas.
     
     Documentación
     -------
     https://stats.oecd.org/
     
     
     @authors: Nobert Andrei Romero Escobedo, Mauricio Alvarado
     
-    """
+    '''
 
 
-    filters = "+".join(countries.keys())
+    filters = '+'.join(countries.keys())
     nombres = list(countries.values())
     cantidad_paises = len(countries.keys())
     
-    url = f"https://stats.oecd.org/SDMX-JSON/data/{identifier}/{filters}.{serie}/all?startTime={fechaini}&endTime={fechafin}"
+    url = f'https://stats.oecd.org/SDMX-JSON/data/{identifier}/{filters}.{serie}/all?startTime={fechaini}&endTime={fechafin}'
 
     r = requests.get(url)
     if r.status_code == 200:
         pass
     else:
-        print("Por favor, revisa los datos ingresados.")
+        print('Por favor, revisa los datos ingresados.')
         return
 
 
-    series = r.json()["dataSets"][0]["series"]    
+    series = r.json()['dataSets'][0]['series']    
     
     df = pd.DataFrame()
     j = 0
 
     for i in range(0, cantidad_paises):
-        fechas = list(list(series.values())[i]["observations"].keys())    # Índices con fechas
-        valores = list(list(series.values())[i]["observations"].values()) # Valores en bruto
+        fechas = list(list(series.values())[i]['observations'].keys())    # Índices con fechas
+        valores = list(list(series.values())[i]['observations'].values()) # Valores en bruto
         
         # Extraer los valores limpios
         nv = []
         for i in range(0, len(fechas)):
             nv.append(valores[i][0])
 
         if df.empty == True:
-            df = pd.DataFrame({"fechas": fechas, nombres[j]: nv})
+            df = pd.DataFrame({'fechas': fechas, nombres[j]: nv})
         else:
-            df2 = pd.DataFrame({"fechas": fechas, nombres[j]: nv})
-            df = df.merge(df2, how="inner")
+            df2 = pd.DataFrame({'fechas': fechas, nombres[j]: nv})
+            df = df.merge(df2, how='inner')
         j += 1    
       
-    df = df.set_index("fechas")
+    df = df.set_index('fechas')
     df.index = pd.period_range(fechaini, fechafin, freq=periodicidad)
-
+    df.sort_index(inplace=True)
+    
     return df
```

### Comparing `econdata-1.0.4/src/econdata/YFinance.py` & `econdata-1.0.5.post0/src/econdata/YFinance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 import pandas as pd
 import yfinance as yf
 
 
 
-def get_data(series, tipo="Close", fechaini=None, fechafin=None):
+def get_data(series, tipo='Close', fechaini=None, fechafin=None):
 
-    """ Importar multiples series de la API de Yahoo Finance
+    ''' Importar multiples series de la API de Yahoo Finance.
     
     Parámetros
     ----------
     series: dict
-        Lista de los codigos de las series y nombres
+        Lista de los codigos de las series y nombres.
     tipo: str
         Serie consultada.
         >>> Close: Default
         >>> Open
         >>> High
         >>> Low
         >>> AdjClose
         >>> Volume
     fechaini: datetime
-        Fecha de inicio de la serie 
+        Fecha de inicio de la serie.
     fechafin: datetime
-        Fecha de fin de la serie
+        Fecha de fin de la serie.
 
     Retorno
     ----------
     df: pd.DataFrame
-        Series consultadas
+        Series consultadas.
     
     Documentación
     ----------
     https://pypi.org/project/yfinance/
 
 
     @author: Mauricio Alvarado
     
-    """
+    '''
     
     
     keys = list(series.keys())
     df = pd.DataFrame()
     
     for key in keys:
         data = yf.Ticker(key)
         
         if (fechaini == None) or (fechafin == None):
-            data = data.history(period="max")
+            data = data.history(period='max')
         else:
             data = data.history(start=fechaini, end=fechafin)
         
         data.reset_index(inplace=True)
         data[key] = data[tipo]
 
         try: 
             # Quitar zona horaria
             data['Date'] = data['Date'].dt.tz_localize(None)
         except:
             pass
     
         # Merge
-        df = pd.concat([df, data[["Date", key]]]) if df.empty is True else pd.merge(df, data[["Date", key]], how="outer")
+        df = pd.concat([df, data[['Date', key]]]) if df.empty is True else pd.merge(df, data[['Date', key]], how='outer')
 
-    df.set_index("Date", inplace=True)
-    df.index = df.index.strftime("%Y-%m-%d")
+    df.set_index('Date', inplace=True)
+    df.index = df.index.strftime('%Y-%m-%d')
     df.sort_index(inplace=True)
     df = df.rename(series, axis = 1)
 
 
     return df
 
 
 
 def search(consulta):
     
-    """ Extraer código de la consulta
+    ''' Extraer código de la consulta.
     
     Parámetros
     ----------
     consulta: list
-        Palabras claves de las series
+        Palabras claves de las series.
 
     Retorno
     ----------
     df: pd.DataFrame
-        Metadatos de las series consultadas
+        Metadatos de las series consultadas.
     
     Documentación
     ----------
     https://www.nasdaq.com/market-activity/stocks/screener
     
         
     Ejemplos
@@ -122,30 +122,30 @@
     >>> SPOT: Spotify
     >>> TCEHY: Tencent Holdings Limited
     >>> TSLA: Tesla
     
     
     @author: Mauricio Alvarado
     
-    """
+    '''
     
     df = pd.read_csv(
-        "https://raw.githubusercontent.com/mauricioalvaradoo/econdata/master/src/econdata/metadata/Yahoo-Tickers.csv",
+        'https://raw.githubusercontent.com/mauricioalvaradoo/econdata/master/src/econdata/metadata/Yahoo-Tickers.csv',
         index_col=0
     ).reset_index()
-    df = df[["Symbol", "Name", "Country", "IPO Year", "Sector", "Industry"]]
-    df.set_index("Symbol", inplace=True)
+    df = df[['Symbol', 'Name', 'Country', 'IPO Year', 'Sector', 'Industry']]
+    df.set_index('Symbol', inplace=True)
     
     consulta = [x.lower() for x in consulta]
     
     for i in consulta:           
         try:
-            filter = df["Name"].str.lower().str.contains(i)
+            filter = df['Name'].str.lower().str.contains(i)
             df = df[filter]
         except:
-            df = print("Consulta no encontrada!")
+            df = print('Consulta no encontrada!')
             return
     
     return df
```

### Comparing `econdata-1.0.4/src/econdata.egg-info/PKG-INFO` & `econdata-1.0.5.post0/src/econdata.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: econdata
-Version: 1.0.4
+Version: 1.0.5.post0
 Summary: Extracción de series de tiempo de las principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/econdata
 Author: Mauricio Alvarado, Andrei Romero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Econdata
 Extracción de series de tiempo de las principales instituciones económicas para el Perú:
 1. Banco Central de Reserva del Perú (BCRP)
-2. Yahoo Finance
+2. Yahoo Finance (YFinance)
 3. Federal Reserve Economic Data (FRED)
-4. World Bank
-5. Organización para la Cooperación y el Desarrollo Económicos (OCDE)
+4. World Bank (WB)
+5. Organization for Economic Cooperation and Development (OECD)
+6. International Monetary Fund (IMF)
 
 ```
 # Instalación mediante PyPI
-!pip install econdata==1.0.4
+!pip install econdata==1.0.5-r
 
 # o simplemente:
 !pip install econdata
 ```
 El anuncio fue realizado en Linkedin, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
 
-## Versión 1.0.4
-* Para el `BCRP`, `Yahoo Finance`, `FRED` y el `World Bank`, se cuenta con ambos métodos: `get_data()` y `search()`.
-* Para la `OCDE`, se cuenta únicamente con el método `get_data()`.
-* En la versión 1.0.4, (i) se corrigió el formato de las fechas para `BCRP` y `FRED`, y (ii) se añadió el filtro de frecuencia en `search()` para `FRED`.
+## Versión 1.0.5-r
+* Para el `BCRP`, `YFinance`, `FRED`, `IMF` y el `WB`, se cuenta con ambos métodos: `get_data()` y `search()`.
+* Para la `OECD`, se cuenta únicamente con el método `get_data()`.
+* En la versión 1.0.5-r, se incluyó el `IMF`.
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```
 get_data()
 ```
@@ -48,11 +49,16 @@
 
 
 ## Test !
 El código guía para usar las funciones está disponible [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/test.py).
 El video del anuncio de la librería y la demo está disponible [aquí](https://www.youtube.com/watch?v=etaqHMDfvtE).
 
 
+## Macroeconomic Dataset
+Se elaboró un dataset de series macroeconómicas [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/macro-dataset.py).
+
+
+
 ## Créditos
 * [Mauricio Alvarado](https://github.com/mauricioalvaradoo)
 * [Andrei Romero](https://github.com/Ixtalia)
```

