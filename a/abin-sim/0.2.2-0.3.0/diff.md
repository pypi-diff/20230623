# Comparing `tmp/abin_sim-0.2.2.tar.gz` & `tmp/abin_sim-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abin_sim-0.2.2.tar", max compression
+gzip compressed data, was "abin_sim-0.3.0.tar", max compression
```

## Comparing `abin_sim-0.2.2.tar` & `abin_sim-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      260 2023-06-22 13:51:02.599520 abin_sim-0.2.2/LICENSE
--rw-r--r--   0        0        0     7252 2023-06-22 13:51:02.599520 abin_sim-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-06-22 13:51:02.599520 abin_sim-0.2.2/abin_sim/__init__.py
--rw-r--r--   0        0        0     5331 2023-06-22 13:51:02.599520 abin_sim-0.2.2/abin_sim/cli.py
--rw-r--r--   0        0        0      194 2023-06-22 13:51:02.599520 abin_sim-0.2.2/abin_sim/config.py
--rw-r--r--   0        0        0      783 2023-06-22 13:51:02.599520 abin_sim-0.2.2/abin_sim/core/file_manager.py
--rw-r--r--   0        0        0     3224 2023-06-22 13:51:02.599520 abin_sim-0.2.2/abin_sim/core/functions.py
--rw-r--r--   0        0        0     1190 2023-06-22 13:51:02.599520 abin_sim-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     8141 1970-01-01 00:00:00.000000 abin_sim-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-06-23 12:59:01.261627 abin_sim-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7485 2023-06-23 12:59:01.261627 abin_sim-0.3.0/README.md
+-rw-r--r--   0        0        0       21 2023-06-23 12:59:01.261627 abin_sim-0.3.0/abin_sim/__init__.py
+-rw-r--r--   0        0        0     6693 2023-06-23 12:59:01.261627 abin_sim-0.3.0/abin_sim/cli.py
+-rw-r--r--   0        0        0      194 2023-06-23 12:59:01.261627 abin_sim-0.3.0/abin_sim/config.py
+-rw-r--r--   0        0        0      783 2023-06-23 12:59:01.261627 abin_sim-0.3.0/abin_sim/core/file_manager.py
+-rw-r--r--   0        0        0     3224 2023-06-23 12:59:01.261627 abin_sim-0.3.0/abin_sim/core/functions.py
+-rw-r--r--   0        0        0     1190 2023-06-23 12:59:01.261627 abin_sim-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8374 1970-01-01 00:00:00.000000 abin_sim-0.3.0/PKG-INFO
```

### Comparing `abin_sim-0.2.2/README.md` & `abin_sim-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# ABIN
+[![CI](https://github.com/SIM-Rede/abin-sim/actions/workflows/pipeline.yaml/badge.svg)](https://github.com/SIM-Rede/abin-sim/actions/workflows/pipeline.yaml)
+[![PyPI version](https://badge.fury.io/py/abin-sim.svg)](https://badge.fury.io/py/abin-sim)
+
 ## Instalação
 
 ```
 sudo apt install pipx
 pipx install abin_sim
 
 ```
@@ -25,21 +29,24 @@
 Com o arquivo em mãos, altere o valor de **vault_token** para o seu token, o valor deverá focar entre " "
 
 *vault_token* -> Seu token de autenticação no Vault
 
 Para ter acesso seu token basta autenticar no Web UI do Vault.
 Acesse no seu navegador o endereço https://aspirina.simtech.solutions
 *PS*: O acesso devera ser solicitado ao time de SRE da SIMTech
+
 Na tela de login:
-    * Mude **Method** para ***Username***
-    * Entre com o seu usuário em **Username**
-    * Entre com a sua senha em **Password**
-    * Clique em **More Options**
-    * Em **Mount Path** digite ***simtech***
-    * Clique em **Sign in**
+
+* Mude **Method** para ***Username***
+* Entre com o seu usuário em **Username**
+* Entre com a sua senha em **Password**
+* Clique em **More Options**
+* Em **Mount Path** digite ***simtech***
+* Clique em **Sign in**
+
 Após o login clique no boneco localizao no canto superior direito e, após, clique em **Copy Token**
 
 **Importante:** O Token é válido por 30 dias, portanto lembre de renová-lo.
 
 ## Funções
     
 ### GET
@@ -52,15 +59,15 @@
     │    --file    --no-file          Cria um arquivo para cada path cadastrada no secrets. [default: file]                                                │
     │    --help                       Show this message and exit.                                                                                          │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
     For example:
     * Imprime os dados no StdOut (Tela)
         abin get --app api-auth --env dev --proj simlabs --no-file
-    * Imprime os dados em arquivo (Com base no arquivo $HOME/abin_sim/settings.toml)
+    * Imprime os dados em arquivo (Com base no arquivo $HOME/abin/settings.toml)
         abin get --app api-auth --env dev --proj simlabs
 
 ### UPDATE
     Usage: abin update [OPTIONS] 
                                                
     ╭─ Options─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app         TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None]  [required]                                        │
```

### Comparing `abin_sim-0.2.2/abin_sim/cli.py` & `abin_sim-0.3.0/abin_sim/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,73 @@
-import pkg_resources
 from rich.console import Console
 from rich.table import Table
-from typer import Option, Typer
+from typer import Context, Exit, Option, Typer
+
+from abin_sim import __version__
 
 from .config import settings
 from .core.file_manager import make_return
 from .core.functions import (
     convert_to_json,
     get_metadata,
     get_secret,
     make_conf,
     update_secret,
 )
 
 console = Console()
 app = Typer()
 
-@app.command('version')
-def version():
-    console.print(pkg_resources.get_distribution('abin-sim').version)
-
-@app.command('make-conf')
-def conf():
-    configuration = make_conf()
-    if configuration['Status']:
-        console.print(configuration['Message'])
-    else:
-        console.print(configuration['Message'])
+
+def version_func(flag):
+    if flag:
+        print(__version__)
+        raise Exit(code=0)
+
+def conf_func(flag):
+    if flag:
+        configuration = make_conf()
+        if configuration['Status']:
+            console.print(configuration['Message'])
+        else:
+            console.print(configuration['Message'])
+        raise Exit(code=0)
+    
+
+@app.callback(invoke_without_command=True)
+def main(
+    ctx: Context,
+    version: bool = Option(False, callback=version_func, is_flag=True),
+    configure: bool = Option(False, callback=conf_func, is_flag=True),
+):
+    message = """
+[b]ABIN[/] - SIM Tech Solutions
+
+Forma de uso: [b]abin [SUBCOMANDO] [ARGUMENTOS][/]
+
+Existem 3 subcomandos disponíveis para essa aplicação
+
+- [b]get[/]: Fornece os secrets cadastrados em uma aplicação. Este retorno pode ser em tela ou arquivo
+- [b]update[/]: Envia uma nova coleção de ENV para uma determinada aplicação [red](Uso restrito, somente TL e SRE)[/]
+- [b]compare[/]: Compara o ENV de uma aplicação em 2 ambientes
+
+[b]Exemplos de uso:[/]
+[green][b]abin[/][/] [b]get[/] --app api-auth --env dev --proj simlabs [magenta](para retorno em tela use [green][b]--no-file[/][/])[/]
+
+[green][b]abin[/][/] [b]update[/] --app api-auth --env dev --proj simlabs --file .env
+
+[green][b]abin[/][/] [b]compare[/] --app api-auth --env qa,dev --proj simlabs
+
+[b]Para mais informações[/]: [green][b]abin[/][/] --help
+[b]Para ver a versão instalada[/]: [green][b]abin[/][/] --version
+[b]Para informações detalhadas: [blue][link=https://github.com/SIM-Rede/abin-sim]Repo no GIT SIM[/]
+"""
+    if ctx.invoked_subcommand:
+        return
+    console.print(message)
 
 @app.command('get')
 def get(
     app: str = Option(
         ...,
         help='Nome da aplicação que deseja recuperar os secrets.',
     ),
```

### Comparing `abin_sim-0.2.2/abin_sim/core/file_manager.py` & `abin_sim-0.3.0/abin_sim/core/file_manager.py`

 * *Files identical despite different names*

### Comparing `abin_sim-0.2.2/abin_sim/core/functions.py` & `abin_sim-0.3.0/abin_sim/core/functions.py`

 * *Files identical despite different names*

### Comparing `abin_sim-0.2.2/pyproject.toml` & `abin_sim-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abin-sim"
-version = "0.2.2"
+version = "0.3.0"
 description = "ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech"
 license = "BeerWare"
 authors = ["Bonatto <andrebonatto@gmail.com>"]
 readme = "README.md"
 packages = [{include = "abin_sim"}]
 classifiers = [
     "Topic :: Utilities",
```

### Comparing `abin_sim-0.2.2/PKG-INFO` & `abin_sim-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abin-sim
-Version: 0.2.2
+Version: 0.3.0
 Summary: ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech
 License: Beerware
 Author: Bonatto
 Author-email: andrebonatto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -17,14 +17,18 @@
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: pathlib3x (>=2.0.2.1,<3.0.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
+# ABIN
+[![CI](https://github.com/SIM-Rede/abin-sim/actions/workflows/pipeline.yaml/badge.svg)](https://github.com/SIM-Rede/abin-sim/actions/workflows/pipeline.yaml)
+[![PyPI version](https://badge.fury.io/py/abin-sim.svg)](https://badge.fury.io/py/abin-sim)
+
 ## Instalação
 
 ```
 sudo apt install pipx
 pipx install abin_sim
 
 ```
@@ -48,21 +52,24 @@
 Com o arquivo em mãos, altere o valor de **vault_token** para o seu token, o valor deverá focar entre " "
 
 *vault_token* -> Seu token de autenticação no Vault
 
 Para ter acesso seu token basta autenticar no Web UI do Vault.
 Acesse no seu navegador o endereço https://aspirina.simtech.solutions
 *PS*: O acesso devera ser solicitado ao time de SRE da SIMTech
+
 Na tela de login:
-    * Mude **Method** para ***Username***
-    * Entre com o seu usuário em **Username**
-    * Entre com a sua senha em **Password**
-    * Clique em **More Options**
-    * Em **Mount Path** digite ***simtech***
-    * Clique em **Sign in**
+
+* Mude **Method** para ***Username***
+* Entre com o seu usuário em **Username**
+* Entre com a sua senha em **Password**
+* Clique em **More Options**
+* Em **Mount Path** digite ***simtech***
+* Clique em **Sign in**
+
 Após o login clique no boneco localizao no canto superior direito e, após, clique em **Copy Token**
 
 **Importante:** O Token é válido por 30 dias, portanto lembre de renová-lo.
 
 ## Funções
     
 ### GET
@@ -75,15 +82,15 @@
     │    --file    --no-file          Cria um arquivo para cada path cadastrada no secrets. [default: file]                                                │
     │    --help                       Show this message and exit.                                                                                          │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
     For example:
     * Imprime os dados no StdOut (Tela)
         abin get --app api-auth --env dev --proj simlabs --no-file
-    * Imprime os dados em arquivo (Com base no arquivo $HOME/abin_sim/settings.toml)
+    * Imprime os dados em arquivo (Com base no arquivo $HOME/abin/settings.toml)
         abin get --app api-auth --env dev --proj simlabs
 
 ### UPDATE
     Usage: abin update [OPTIONS] 
                                                
     ╭─ Options─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ *  --app         TEXT  Nome da aplicação que deseja recuperar os secrets. [default: None]  [required]                                        │
```

