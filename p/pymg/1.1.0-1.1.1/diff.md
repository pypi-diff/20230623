# Comparing `tmp/pymg-1.1.0.tar.gz` & `tmp/pymg-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymg-1.1.0.tar", last modified: Fri Jun  2 06:50:26 2023, max compression
+gzip compressed data, was "pymg-1.1.1.tar", last modified: Thu Jun 22 23:49:31 2023, max compression
```

## Comparing `pymg-1.1.0.tar` & `pymg-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-06-02 06:50:26.393669 pymg-1.1.0/
--rw-r--r--   0 mimseyedi   (501) staff       (20)    35129 2023-05-03 19:17:09.000000 pymg-1.1.0/LICENSE
--rw-r--r--   0 mimseyedi   (501) staff       (20)     2213 2023-06-02 06:50:26.393559 pymg-1.1.0/PKG-INFO
--rw-r--r--   0 mimseyedi   (501) staff       (20)     1542 2023-06-02 06:41:12.000000 pymg-1.1.0/README.md
-drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-06-02 06:50:26.392724 pymg-1.1.0/pymg/
--rw-r--r--   0 mimseyedi   (501) staff       (20)        0 2023-05-03 19:21:55.000000 pymg-1.1.0/pymg/__init__.py
--rw-r--r--   0 mimseyedi   (501) staff       (20)      178 2023-06-02 06:26:19.000000 pymg-1.1.0/pymg/mirror.py
--rw-r--r--   0 mimseyedi   (501) staff       (20)    44500 2023-06-02 06:46:53.000000 pymg-1.1.0/pymg/pymg.py
-drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-06-02 06:50:26.393410 pymg-1.1.0/pymg.egg-info/
--rw-r--r--   0 mimseyedi   (501) staff       (20)     2213 2023-06-02 06:50:26.000000 pymg-1.1.0/pymg.egg-info/PKG-INFO
--rw-r--r--   0 mimseyedi   (501) staff       (20)      241 2023-06-02 06:50:26.000000 pymg-1.1.0/pymg.egg-info/SOURCES.txt
--rw-r--r--   0 mimseyedi   (501) staff       (20)       20 2023-06-02 06:50:26.000000 pymg-1.1.0/pymg.egg-info/dependency_links.txt
--rw-r--r--   0 mimseyedi   (501) staff       (20)       40 2023-06-02 06:50:26.000000 pymg-1.1.0/pymg.egg-info/entry_points.txt
--rw-r--r--   0 mimseyedi   (501) staff       (20)       20 2023-06-02 06:50:26.000000 pymg-1.1.0/pymg.egg-info/requires.txt
--rw-r--r--   0 mimseyedi   (501) staff       (20)        5 2023-06-02 06:50:26.000000 pymg-1.1.0/pymg.egg-info/top_level.txt
--rw-r--r--   0 mimseyedi   (501) staff       (20)       38 2023-06-02 06:50:26.393707 pymg-1.1.0/setup.cfg
--rw-r--r--   0 mimseyedi   (501) staff       (20)     1193 2023-06-02 06:45:49.000000 pymg-1.1.0/setup.py
+drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-06-22 23:49:31.185590 pymg-1.1.1/
+-rw-r--r--   0 mimseyedi   (501) staff       (20)    35129 2023-05-03 19:17:09.000000 pymg-1.1.1/LICENSE
+-rw-r--r--   0 mimseyedi   (501) staff       (20)    24458 2023-06-22 23:49:31.185459 pymg-1.1.1/PKG-INFO
+-rw-r--r--   0 mimseyedi   (501) staff       (20)    23838 2023-06-22 23:44:37.000000 pymg-1.1.1/README.md
+drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-06-22 23:49:31.184510 pymg-1.1.1/pymg/
+-rw-r--r--   0 mimseyedi   (501) staff       (20)        0 2023-05-03 19:21:55.000000 pymg-1.1.1/pymg/__init__.py
+-rw-r--r--   0 mimseyedi   (501) staff       (20)    44638 2023-06-22 23:32:31.000000 pymg-1.1.1/pymg/pymg.py
+drwxr-xr-x   0 mimseyedi   (501) staff       (20)        0 2023-06-22 23:49:31.185280 pymg-1.1.1/pymg.egg-info/
+-rw-r--r--   0 mimseyedi   (501) staff       (20)    24458 2023-06-22 23:49:31.000000 pymg-1.1.1/pymg.egg-info/PKG-INFO
+-rw-r--r--   0 mimseyedi   (501) staff       (20)      226 2023-06-22 23:49:31.000000 pymg-1.1.1/pymg.egg-info/SOURCES.txt
+-rw-r--r--   0 mimseyedi   (501) staff       (20)       20 2023-06-22 23:49:31.000000 pymg-1.1.1/pymg.egg-info/dependency_links.txt
+-rw-r--r--   0 mimseyedi   (501) staff       (20)       40 2023-06-22 23:49:31.000000 pymg-1.1.1/pymg.egg-info/entry_points.txt
+-rw-r--r--   0 mimseyedi   (501) staff       (20)       20 2023-06-22 23:49:31.000000 pymg-1.1.1/pymg.egg-info/requires.txt
+-rw-r--r--   0 mimseyedi   (501) staff       (20)        5 2023-06-22 23:49:31.000000 pymg-1.1.1/pymg.egg-info/top_level.txt
+-rw-r--r--   0 mimseyedi   (501) staff       (20)       38 2023-06-22 23:49:31.185626 pymg-1.1.1/setup.cfg
+-rw-r--r--   0 mimseyedi   (501) staff       (20)     1161 2023-06-22 23:36:18.000000 pymg-1.1.1/setup.py
```

### Comparing `pymg-1.1.0/LICENSE` & `pymg-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymg-1.1.0/pymg/pymg.py` & `pymg-1.1.1/pymg/pymg.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 https://github.com/mimseyedi/pymg/blob/master/docs/guide/how_to_use_pymg.md
 
 pymg Github repository:
 https://github.com/mimseyedi/pymg
 """
 
 
+
 import os
 import re
 import sys
 import click
 import pickle
 import requests
 import traceback
@@ -39,16 +40,14 @@
 from pathlib import Path
 from types import TracebackType, ModuleType
 try:
     from rich.panel import Panel
     from rich.console import Group
     from rich.syntax import Syntax
     from rich import print as cprint
-except ModuleNotFoundError:
-    subprocess.run([sys.executable, "-m", "pip", "install", "rich"], stdout=subprocess.DEVNULL)
 except ImportError:
     subprocess.run([sys.executable, "-m", "pip", "install", "rich"], stdout=subprocess.DEVNULL)
 finally:
     from rich.panel import Panel
     from rich.console import Group
     from rich.syntax import Syntax
     from rich import print as cprint
@@ -142,15 +141,15 @@
 
     if source_info_file.exists():
         with open(file=source_info_file, mode='rb') as source_info_file_:
             source_information: list = pickle.load(source_info_file_)
 
         return source_information
 
-    return list()
+    return []
 
 
 def write_source_info(source_info_file: Path, source_info: tuple) -> None:
     """
     The task of this function is to write the information of the main file (source) in a file.
 
     -Note: This is done so that the information of the original file (source) is replaced by the
@@ -193,34 +192,45 @@
     """
 
     syntax_err: str = subprocess.run(
         [python_interpreter, '-m', 'py_compile', source_file.__str__()],
         capture_output=True
     ).stderr.decode()
 
-    return (True, 'INTACT') if not syntax_err else (False, syntax_err)
+    return (False, syntax_err) if syntax_err else (True, 'INTACT')
 
 
 def display_syntax_error(source_file: Path, syntax_err: str) -> None:
     """
     The task of this function is to create and finally display
     the error template that shows the syntax error message.
 
     :param source_file: The path of the python file that the user introduced to pymg.
     :param syntax_err: The syntax error message generated by the Python interpreter.
     :return: None
     """
 
-    if not syntax_err.startswith("Sorry: IndentationError:"):
+    extract_digits = lambda string: int(''.join([char for char in string if char.isdigit()]))
+
+    if syntax_err.startswith("Sorry: TabError:"):
+        title: str = "TabError"
+        splitted_message: list = syntax_err.split("(")
+        lineno: int = extract_digits(splitted_message[-1].split(",")[-1])
+        code: str = read_source(source_file=source_file)[lineno - 1].strip()
+        pointer, message = "    ^", splitted_message[0][16:].strip()
+
+    elif not syntax_err.startswith("Sorry: IndentationError:"):
+        title: str = "SyntaxError"
         splitted_message: list = syntax_err[syntax_err.index(',') + 2:].split('\n')
-        lineno, code = int(splitted_message[0].split()[-1]), splitted_message[1].strip()
+        lineno, code = extract_digits(splitted_message[0].split()[-1]), splitted_message[1].strip()
         pointer, message = splitted_message[2], splitted_message[3][13:]
 
     else:
-        lineno: int = int(syntax_err.split(',')[-1][:-1].split()[-1])
+        title: str = "IndentationError"
+        lineno: int = extract_digits(syntax_err.split(',')[-1][:-1].split()[-1])
         code: str = read_source(source_file=source_file)[lineno - 1].strip()
         pointer, message = "    ^", syntax_err.split(":")[2].split("(")[0].strip()
 
     main_group = Group(
         Syntax(code=code, lexer='python', line_numbers=True,
                start_line=lineno, highlight_lines={lineno},
                indent_guides=True, background_color='default', theme='gruvbox-dark'),
@@ -228,16 +238,15 @@
         pointer if len(str(lineno)) < 2 else " " * (len(str(lineno)) - 1) + pointer,
 
         '\n' + f'Message: [default]{message.capitalize()}[/]'
     )
 
     cprint(Panel(
         main_group,
-        title='SyntaxError' if not syntax_err.startswith("Sorry: IndentationError:")
-        else 'IndentationError',
+        title=title,
         style='red',
         padding=(1, 1, 1, 1),
         highlight=False
     ))
 
 
 def gen_type(**exc_info: type|Exception|TracebackType) -> list:
@@ -724,19 +733,26 @@
             item.get('title'): item.get('link')
             for item in response.json().get('items')
             if item.get('is_answered')
         }
 
         search_box = Panel(
             Group(
-                '\n'.join([f'[bold]{title}[/]\n[underline color(33)]{link}[/]\n'
-                for title, link in posts.items()])
-            )
-        , title=f'[bold]Search Result[/]', title_align='center',
-        padding=(1, 1, 0, 1), style='color(29)')
+                '\n'.join(
+                    [
+                        f'[bold]{title}[/]\n[underline color(33)]{link}[/]\n'
+                        for title, link in posts.items()
+                    ]
+                )
+            ),
+            title='[bold]Search Result[/]',
+            title_align='center',
+            padding=(1, 1, 0, 1),
+            style='color(29)',
+        )
 
         cprint(search_box)
 
 
 def get_output(python_interpreter: str, mirror_file: Path, args: list, output_file: Path) -> None:
     """
     The task of this function is to write the output generated by pymg in a text file.
@@ -810,24 +826,21 @@
 
     search_status: bool = False
 
     if 'search' in recipe:
         search_status = True
         recipe.remove('search')
 
-    template: list = [
-        list_ for func in recipe
+    if template := [
+        list_
+        for func in recipe
         for list_ in funcs[func](
-            exc_type=exc_type,
-            exc_message=exc_message,
-            traceback_=traceback_
+            exc_type=exc_type, exc_message=exc_message, traceback_=traceback_
         )
-    ]
-
-    if template:
+    ]:
         cprint(
             Panel(
                 Group(*template),
                 title='Exception',
                 style='red',
                 padding=(0, 1, 0, 1),
                 highlight=False
@@ -875,17 +888,16 @@
             if gen_trace_with_locals not in prioritized_options:
                 prioritized_options.append(option)
 
         elif option == 'inner':
             if gen_inner_with_locals not in prioritized_options:
                 prioritized_options.append(option)
 
-        else:
-            if option != 'search':
-                draft_options.append(option)
+        elif option != 'search':
+            draft_options.append(option)
 
     if not prioritized_options:
         prioritized_options.extend(draft_options)
 
     if 'search' in available_options:
         prioritized_options.append('search')
 
@@ -941,15 +953,15 @@
 def get_version() -> str:
     """
     The task of this function is to return the current version of 'pymg'.
 
     :return: str
     """
 
-    return '1.1.0'
+    return '1.1.1'
 
 
 @click.command(context_settings={'help_option_names': ['-h', '--help']})
 @click.argument('python_file', required=False, nargs=-1)
 @click.option('-x', '--syntax', is_flag=True, help="It checks the syntax of the selected Python file. If there is a syntax problem, an error message will be displayed, otherwise 'INTACT' will be displayed.")
 @click.option('-t', '--type', is_flag=True, help="The type of exception that occurred will be displayed.")
 @click.option('-m', '--message', is_flag=True, help="The message of exception that occurred will be displayed.")
@@ -977,91 +989,90 @@
             python_interpreter=sys.executable,
             mirror_file=MIRROR_FILE,
             args=get_source_info(source_info_file=SOURCE_INFO)[1:],
             source_info_file=SOURCE_INFO,
             recipe_file=RECIPE_FILE
         )
 
-    else:
-        if not options['python_file']:
-            click.echo("Usage: pymg [OPTIONS] [PYTHON_FILE]...\nTry 'pymg --help' for help.\n\nError: Missing argument 'PYTHON_FILE...'.")
-
+    elif options['python_file']:
+        if options['version'] or options['recent']:
+            click.echo(
+                "Usage: pymg [OPTIONS] [PYTHON_FILE]...\nTry 'pymg --help' for help.\n\nError: Two options --version and --recent cannot be used at this stage.")
         else:
-            if options['version'] or options['recent']:
-                click.echo(
-                    "Usage: pymg [OPTIONS] [PYTHON_FILE]...\nTry 'pymg --help' for help.\n\nError: Two options --version and --recent cannot be used at this stage.")
-            else:
-                response, file_error_message = pyfile_path_validator(py_file=Path(options['python_file'][0]))
+            response, file_error_message = pyfile_path_validator(py_file=Path(options['python_file'][0]))
 
-                if response:
-                    if options['syntax']:
-                        response, content = check_syntax(
-                            source_file=options['python_file'][0],
-                            python_interpreter=sys.executable
-                        )
+            if response:
+                if options['syntax']:
+                    response, content = check_syntax(
+                        source_file=options['python_file'][0],
+                        python_interpreter=sys.executable
+                    )
 
-                        cprint(f'[bold green]{content}[/]') if response \
-                            else display_syntax_error(
-                            source_file=options['python_file'][0],
-                            syntax_err=content
-                        )
+                    cprint(f'[bold green]{content}[/]') if response \
+                        else display_syntax_error(
+                        source_file=options['python_file'][0],
+                        syntax_err=content
+                    )
 
-                    else:
-                        response, syntax_err = check_syntax(
-                            source_file=options['python_file'][0],
-                            python_interpreter=sys.executable
-                        )
+                else:
+                    response, syntax_err = check_syntax(
+                        source_file=options['python_file'][0],
+                        python_interpreter=sys.executable
+                    )
 
-                        if response:
-                            filtered_options: dict = {
-                                option: value
-                                for option, value in options.items()
-                                if option not in [
-                                    'python_file', 'syntax', 'output', 'version', 'recent'
-                                ]
-                            }
-
-                            recipe: list = prioritizing_options(options=filtered_options)
-
-                            if recipe:
-                                write_recipe(recipe_file=RECIPE_FILE, recipe_data=recipe)
-                            else:
-                                write_recipe(recipe_file=RECIPE_FILE, recipe_data=['inner_with_locals'])
+                    if response:
+                        filtered_options: dict = {
+                            option: value
+                            for option, value in options.items()
+                            if option not in [
+                                'python_file', 'syntax', 'output', 'version', 'recent'
+                            ]
+                        }
+
+                        if recipe := prioritizing_options(
+                            options=filtered_options
+                        ):
+                            write_recipe(recipe_file=RECIPE_FILE, recipe_data=recipe)
+                        else:
+                            write_recipe(recipe_file=RECIPE_FILE, recipe_data=['inner_with_locals'])
 
-                            source_info: tuple = (
-                                Path(os.getcwd(), options['python_file'][0]), *options['python_file'][1:]
-                            )
+                        source_info: tuple = (
+                            Path(os.getcwd(), options['python_file'][0]), *options['python_file'][1:]
+                        )
 
-                            write_source_info(source_info_file=SOURCE_INFO, source_info=source_info)
+                        write_source_info(source_info_file=SOURCE_INFO, source_info=source_info)
 
-                            mk_mirror_file(
+                        mk_mirror_file(
+                            mirror_file=MIRROR_FILE,
+                            source=read_source(Path(options['python_file'][0])),
+                            header=gen_mirror_header()
+                        )
+
+                        if options['output'] is not None:
+                            output_file: Path = Path(options['output'])
+                            get_output(
+                                python_interpreter=sys.executable,
                                 mirror_file=MIRROR_FILE,
-                                source=read_source(Path(options['python_file'][0])),
-                                header=gen_mirror_header()
+                                args=options['python_file'][1:],
+                                output_file=output_file
                             )
 
-                            if options['output'] is not None:
-                                output_file: Path = Path(options['output'])
-                                get_output(
-                                    python_interpreter=sys.executable,
-                                    mirror_file=MIRROR_FILE,
-                                    args=options['python_file'][1:],
-                                    output_file=output_file
-                                )
-
-                            else:
-                                interpret(
-                                    python_interpreter=sys.executable,
-                                    mirror_file=MIRROR_FILE,
-                                    args=options['python_file'][1:]
-                                )
                         else:
-                            display_syntax_error(
-                                source_file=options['python_file'][0],
-                                syntax_err=syntax_err
+                            interpret(
+                                python_interpreter=sys.executable,
+                                mirror_file=MIRROR_FILE,
+                                args=options['python_file'][1:]
                             )
-                else:
-                    cprint(file_error_message)
+                    else:
+                        display_syntax_error(
+                            source_file=options['python_file'][0],
+                            syntax_err=syntax_err
+                        )
+            else:
+                cprint(file_error_message)
+
+    else:
+        click.echo("Usage: pymg [OPTIONS] [PYTHON_FILE]...\nTry 'pymg --help' for help.\n\nError: Missing argument 'PYTHON_FILE...'.")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pymg-1.1.0/setup.py` & `pymg-1.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 install_requires = ['rich', 'click', 'requests']
 dependency_links = ['rich', 'click', 'requests']
 
 
 setup (
  name = 'pymg',
  description = 'pymg is a CLI tool that can interpret Python files by the Python interpreter and display the error message in a more readable way if an exception occurs.',
- version = '1.1.0',
+ version = '1.1.1',
  packages = find_packages(),
  install_requires = install_requires,
  python_requires='>=3.11',
  entry_points='''
         [console_scripts]
         pymg=pymg.pymg:main
     ''',
  author="mimseyedi",
- keyword="pymg, debugger, CLI, Python, command-line",
+ keyword=["pymg", "debugger", "CLI", "Python", "bug", "debugger-tool"],
  long_description=README,
  long_description_content_type="text/markdown",
  license='GNU General Public License v3 (GPLv3)',
  url='https://github.com/mimseyedi/pymg',
  dependency_links=dependency_links,
  author_email='mim.seyedi@gmail.com',
  classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ]
 )
```

