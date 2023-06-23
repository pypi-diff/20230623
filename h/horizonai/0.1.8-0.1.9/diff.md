# Comparing `tmp/horizonai-0.1.8.tar.gz` & `tmp/horizonai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horizonai-0.1.8.tar", last modified: Fri May  5 01:15:27 2023, max compression
+gzip compressed data, was "horizonai-0.1.9.tar", last modified: Thu May 18 22:55:25 2023, max compression
```

## Comparing `horizonai-0.1.8.tar` & `horizonai-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-05 01:15:27.373497 horizonai-0.1.8/
--rw-r--r--   0 linatawfik   (501) staff       (20)     1070 2023-05-05 01:04:58.000000 horizonai-0.1.8/LICENSE
--rw-r--r--   0 linatawfik   (501) staff       (20)     2344 2023-05-05 01:15:27.373576 horizonai-0.1.8/PKG-INFO
--rw-r--r--   0 linatawfik   (501) staff       (20)     1612 2023-05-05 01:04:58.000000 horizonai-0.1.8/README.md
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-05 01:15:27.372637 horizonai-0.1.8/horizonai/
--rw-r--r--   0 linatawfik   (501) staff       (20)      216 2023-05-05 01:04:58.000000 horizonai-0.1.8/horizonai/__init__.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     1351 2023-05-05 01:04:58.000000 horizonai-0.1.8/horizonai/base.py
--rw-r--r--   0 linatawfik   (501) staff       (20)    14613 2023-05-05 01:04:58.000000 horizonai-0.1.8/horizonai/cli.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     1227 2023-05-05 01:04:58.000000 horizonai-0.1.8/horizonai/project.py
--rw-r--r--   0 linatawfik   (501) staff       (20)     3560 2023-05-05 01:04:58.000000 horizonai-0.1.8/horizonai/task.py
--rw-r--r--   0 linatawfik   (501) staff       (20)      355 2023-05-05 01:04:58.000000 horizonai-0.1.8/horizonai/user.py
-drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-05 01:15:27.373396 horizonai-0.1.8/horizonai.egg-info/
--rw-r--r--   0 linatawfik   (501) staff       (20)     2344 2023-05-05 01:15:27.000000 horizonai-0.1.8/horizonai.egg-info/PKG-INFO
--rw-r--r--   0 linatawfik   (501) staff       (20)      350 2023-05-05 01:15:27.000000 horizonai-0.1.8/horizonai.egg-info/SOURCES.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)        1 2023-05-05 01:15:27.000000 horizonai-0.1.8/horizonai.egg-info/dependency_links.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       48 2023-05-05 01:15:27.000000 horizonai-0.1.8/horizonai.egg-info/entry_points.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       15 2023-05-05 01:15:27.000000 horizonai-0.1.8/horizonai.egg-info/requires.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       10 2023-05-05 01:15:27.000000 horizonai-0.1.8/horizonai.egg-info/top_level.txt
--rw-r--r--   0 linatawfik   (501) staff       (20)       79 2023-05-05 01:15:27.373800 horizonai-0.1.8/setup.cfg
--rw-r--r--   0 linatawfik   (501) staff       (20)     1282 2023-05-05 01:14:36.000000 horizonai-0.1.8/setup.py
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-18 22:55:25.604415 horizonai-0.1.9/
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1070 2023-05-18 22:52:32.000000 horizonai-0.1.9/LICENSE
+-rw-r--r--   0 linatawfik   (501) staff       (20)     2344 2023-05-18 22:55:25.604478 horizonai-0.1.9/PKG-INFO
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1612 2023-05-18 22:52:32.000000 horizonai-0.1.9/README.md
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-18 22:55:25.603522 horizonai-0.1.9/horizonai/
+-rw-r--r--   0 linatawfik   (501) staff       (20)      216 2023-05-18 22:52:32.000000 horizonai-0.1.9/horizonai/__init__.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1351 2023-05-18 22:52:32.000000 horizonai-0.1.9/horizonai/base.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)    15657 2023-05-18 22:52:32.000000 horizonai-0.1.9/horizonai/cli.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1227 2023-05-18 22:52:32.000000 horizonai-0.1.9/horizonai/project.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)     4367 2023-05-18 22:52:32.000000 horizonai-0.1.9/horizonai/task.py
+-rw-r--r--   0 linatawfik   (501) staff       (20)      355 2023-05-18 22:52:32.000000 horizonai-0.1.9/horizonai/user.py
+drwxr-xr-x   0 linatawfik   (501) staff       (20)        0 2023-05-18 22:55:25.604285 horizonai-0.1.9/horizonai.egg-info/
+-rw-r--r--   0 linatawfik   (501) staff       (20)     2344 2023-05-18 22:55:25.000000 horizonai-0.1.9/horizonai.egg-info/PKG-INFO
+-rw-r--r--   0 linatawfik   (501) staff       (20)      350 2023-05-18 22:55:25.000000 horizonai-0.1.9/horizonai.egg-info/SOURCES.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)        1 2023-05-18 22:55:25.000000 horizonai-0.1.9/horizonai.egg-info/dependency_links.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       48 2023-05-18 22:55:25.000000 horizonai-0.1.9/horizonai.egg-info/entry_points.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       15 2023-05-18 22:55:25.000000 horizonai-0.1.9/horizonai.egg-info/requires.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       10 2023-05-18 22:55:25.000000 horizonai-0.1.9/horizonai.egg-info/top_level.txt
+-rw-r--r--   0 linatawfik   (501) staff       (20)       79 2023-05-18 22:55:25.604676 horizonai-0.1.9/setup.cfg
+-rw-r--r--   0 linatawfik   (501) staff       (20)     1231 2023-05-18 22:54:04.000000 horizonai-0.1.9/setup.py
```

### Comparing `horizonai-0.1.8/LICENSE` & `horizonai-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.8/PKG-INFO` & `horizonai-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: horizonai
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package and command line interface to access the Horizon AI API
 Home-page: https://www.gethorizon.ai
-Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.8.tar.gz
+Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.9.tar.gz
 Author: Horizon Team
 Author-email: team@gethorizon.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `horizonai-0.1.8/README.md` & `horizonai-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.8/horizonai/base.py` & `horizonai-0.1.9/horizonai/base.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.8/horizonai/cli.py` & `horizonai-0.1.9/horizonai/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,50 +8,45 @@
 
 config = configparser.ConfigParser()
 config.read(os.path.expanduser("~/.horizonai.cfg"))
 
 
 @click.group()
 def cli():
+    """Command line interface for Horizon AI API."""
     pass
 
 
 @click.group()
 def user():
+    """Manage your User account."""
     pass
 
 
 @click.group()
 def project():
+    """Manage your Projects."""
     pass
 
 
 @click.group()
 def task():
-    pass
-
-
-@click.group()
-def evaluation_dataset():
-    pass
-
-
-@click.group()
-def prompt():
+    """Manage your Tasks."""
     pass
 
 
 # User-related methods
-# Generate new Horizon API key for user
+# Generate new HorizonAI API key for user
 @click.command(name="api-key")
 @click.option("--email", prompt="Email", help="The email for the user.")
 @click.password_option(
     "--password", prompt="Password", help="The password for the user."
 )
 def generate_new_api_key(email, password):
+    """Generate a new HorizonAI API key."""
     try:
         result = horizonai.user.generate_new_api_key(email, password)
         formatted_output = json.dumps(result, indent=4)
         click.echo(formatted_output)
     except Exception as e:
         click.echo(str(e))
 
@@ -63,14 +58,15 @@
     "--horizonai_api_key",
     default=os.environ.get("HORIZONAI_API_KEY"),
     prompt="HorizonAI API Key" if not os.environ.get("HORIZONAI_API_KEY") else False,
     help="The HorizonAI API key for the user.",
     hide_input=True,
 )
 def list_projects(horizonai_api_key):
+    """View a list of all your Projects."""
     horizonai.api_key = horizonai_api_key
     try:
         result = horizonai.project.list_projects()
         formatted_output = json.dumps(result, indent=4)
         click.echo(formatted_output)
     except Exception as e:
         click.echo(str(e))
@@ -85,14 +81,15 @@
     help="The HorizonAI API key for the user.",
     hide_input=True,
 )
 @click.option(
     "--name", prompt="Project name", help="The name of the project to create."
 )
 def create_project(name, horizonai_api_key):
+    """Create a new Project."""
     horizonai.api_key = horizonai_api_key
     try:
         result = horizonai.project.create_project(name)
         formatted_output = json.dumps(result, indent=4)
         click.echo(formatted_output)
     except Exception as e:
         click.echo(str(e))
@@ -107,60 +104,38 @@
     help="The HorizonAI API key for the user.",
     hide_input=True,
 )
 @click.option(
     "--project_id", prompt="Project ID", help="The ID of the project to retrieve."
 )
 def get_project(project_id, horizonai_api_key):
+    """Get details about a specific Project."""
     horizonai.api_key = horizonai_api_key
     try:
         result = horizonai.project.get_project(project_id)
         formatted_output = json.dumps(result, indent=4)
         click.echo(formatted_output)
     except Exception as e:
         click.echo(str(e))
 
 
-# Update Project
-@click.command(name="update")
-@click.option(
-    "--horizonai_api_key",
-    default=os.environ.get("HORIZONAI_API_KEY"),
-    prompt="HorizonAI API Key" if not os.environ.get("HORIZONAI_API_KEY") else False,
-    help="The HorizonAI API key for the user.",
-    hide_input=True,
-)
-@click.option(
-    "--project_id", prompt="Project ID", help="The ID of the project to update."
-)
-@click.option("--description", help="The new description for the project.")
-@click.option("--status", help="The new status for the project.")
-def update_project(project_id, horizonai_api_key, description=None, status=None):
-    horizonai.api_key = horizonai_api_key
-    try:
-        result = horizonai.project.update_project(project_id, description, status)
-        formatted_output = json.dumps(result, indent=4)
-        click.echo(formatted_output)
-    except Exception as e:
-        click.echo(str(e))
-
-
 # Delete Project
 @click.command(name="delete")
 @click.option(
     "--horizonai_api_key",
     default=os.environ.get("HORIZONAI_API_KEY"),
     prompt="HorizonAI API Key" if not os.environ.get("HORIZONAI_API_KEY") else False,
     help="The HorizonAI API key for the user.",
     hide_input=True,
 )
 @click.option(
     "--project_id", prompt="Project ID", help="The ID of the project to delete."
 )
 def delete_project(project_id, horizonai_api_key):
+    """Delete an existing Project."""
     horizonai.api_key = horizonai_api_key
     try:
         result = horizonai.project.delete_project(project_id)
         formatted_output = json.dumps(result, indent=4)
         click.echo(formatted_output)
     except Exception as e:
         click.echo(str(e))
@@ -173,61 +148,56 @@
     "--horizonai_api_key",
     default=os.environ.get("HORIZONAI_API_KEY"),
     prompt="HorizonAI API Key" if not os.environ.get("HORIZONAI_API_KEY") else False,
     help="The HorizonAI API key for the user.",
     hide_input=True,
 )
 def list_tasks(horizonai_api_key):
+    """View a list of all your Tasks."""
     horizonai.api_key = horizonai_api_key
     try:
         result = horizonai.task.list_tasks()
         formatted_output = json.dumps(result, indent=4)
         click.echo(formatted_output)
     except Exception as e:
         click.echo(str(e))
 
 
 # Create Task record and generate prompt for it
 @click.command(name="generate")
-@click.option(
-    "--horizonai_api_key",
-    default=os.environ.get("HORIZONAI_API_KEY"),
-    prompt="HorizonAI API Key" if not os.environ.get("HORIZONAI_API_KEY") else False,
-    help="The HorizonAI API key for the user.",
-    hide_input=True,
-)
-@click.option("--name", prompt="Task name", help="The name of the task to create.")
-@click.option(
-    "--project_id",
-    prompt="Associated project ID",
-    help="The ID of the project that the task belongs to.",
-)
-# @click.option('--task_type', prompt='Task type', help='The type of the task to create.')
-@click.option(
-    "--task_type", default="text_generation", help="The type of the task to create."
-)
-@click.option(
-    "--objective",
-    prompt="Task objective",
-    help="The objective of the task to generate.",
-)
-@click.option(
-    "--file_path",
-    prompt="Evaluation data file path",
-    help="The path to the file containing the evaluation datasets to upload.",
-)
-def generate_task(
-    name,
-    project_id,
-    task_type,
-    objective,
-    file_path,
-    horizonai_api_key,
-):
-    horizonai.api_key = horizonai_api_key
+def generate_task():
+    """Create a new Task with the optimal prompt-model configuration."""
+    click.echo("### Step 1 - Task Overview ###")
+    # Get HorizonAI API key
+    if os.environ.get("HORIZONAI_API_KEY"):
+        horizonai.api_key = os.environ.get("HORIZONAI_API_KEY")
+    else:
+        horizonai.api_key = click.prompt(
+            text="HorizonAI API key (text hidden)", hide_input=True
+        )
+
+    # Get project ID
+    project_id = click.prompt("Project ID")
+
+    # Get task name
+    task_name = click.prompt("Task name")
+
+    # Get objective
+    objective = click.prompt("Task objective")
+
+    # Get evaluation dataset
+    dataset_file_path = click.prompt("Evaluation dataset file path (.csv)")
+
+    # Get output schema, if applicable
+    output_schema_file_path = None
+    if click.confirm("Add JSON schema for LLM output?"):
+        output_schema_file_path = click.prompt(text="Output schema file path (.json)")
+
+    click.echo("")
+    click.echo("### Step 2 - Model Selection ###")
 
     # Ask user which models they'd like to include
     allowed_models = []
     if click.confirm("Include [OpenAI]-[gpt-3.5-turbo]?"):
         allowed_models.append("gpt-3.5-turbo")
     if click.confirm("Include [OpenAI]-[text-davinci-003]?"):
         allowed_models.append("text-davinci-003")
@@ -250,39 +220,52 @@
         if os.environ.get("ANTHROPIC_API_KEY"):
             horizonai.anthropic_api_key = os.environ.get("ANTHROPIC_API_KEY")
         else:
             horizonai.anthropic_api_key = click.prompt(
                 text="Anthropic API Key (text hidden)", hide_input=True
             )
 
-    click.echo(f"Evaluating the following models for task generation: {allowed_models}")
-
     # Create task record
     try:
         task_creation_response = horizonai.task.create_task(
-            name, task_type, project_id, allowed_models
+            name=task_name,
+            project_id=project_id,
+            allowed_models=allowed_models,
         )
         task_id = task_creation_response["task"]["id"]
     except Exception as e:
         click.echo("Failed in task creation")
         click.echo(str(e))
         return
 
     # Upload evaluation dataset
     try:
         upload_dataset_response = horizonai.task.upload_evaluation_dataset(
-            task_id, file_path
+            task_id,
+            dataset_file_path,
         )
     except Exception as e:
         # If uploading evaluation dataset fails, then delete previously created task
         horizonai.task.delete_task(task_id)
         click.echo("Failed in dataset upload")
         click.echo(str(e))
         return
 
+    # Upload output schema, if applicable
+    if output_schema_file_path:
+        try:
+            upload_output_schema_response = horizonai.task.upload_output_schema(
+                task_id, output_schema_file_path
+            )
+        except Exception as e:
+            horizonai.task.delete_task(task_id)
+            click.echo("Failed in output schema upload")
+            click.echo(str(e))
+            return
+
     # Confirm key details of task creation (e.g., estimated cost) with user before proceeding
     try:
         task_confirmation_details_response = (
             horizonai.task.get_task_confirmation_details(task_id)
         )
         task_confirmation_details = task_confirmation_details_response[
             "task_confirmation_details"
@@ -290,69 +273,69 @@
     except Exception as e:
         # If error with getting task confirmation details, then clean up task record and evaluation dataset before raising exception
         horizonai.task.delete_task(task_id)
         click.echo("Failed in task confirmation details")
         click.echo(str(e))
         return
 
-    click.echo("=====")
+    click.echo("")
+    click.echo("### Step 3 - Task confirmation ###")
     click.echo(
         "Please confirm the following parameters for your task creation request:"
     )
     click.echo("")
     click.echo(f"1) Task objective: {objective}")
     click.echo("")
     click.echo(f"2) Input variables: {task_confirmation_details['input_variables']}")
     click.echo(
         "* Inferred based on the headers of all but the right-most column in your evaluation dataset."
     )
     click.echo("")
+    click.echo(f"3) Models considered: {allowed_models}")
+    click.echo("")
     click.echo(
-        f"3) Estimated LLM provider cost: ${task_confirmation_details['cost_estimate']['total_cost']['low']}-{task_confirmation_details['cost_estimate']['total_cost']['high']}"
+        f"4) Estimated LLM provider cost: ${task_confirmation_details['cost_estimate']['total_cost']['low']}-{task_confirmation_details['cost_estimate']['total_cost']['high']}"
     )
     click.echo(
         "* This is entirely the LLM provider cost and not a Horizon charge. Actual cost may vary."
     )
-    click.echo("=====")
+    click.echo("")
 
     # Cancel task creation if user does not give confirmation
-    if not click.confirm("Proceed with task creation?"):
+    if not click.confirm("Proceed?"):
         # Delete task and evaluation dataset, and abort operation
         horizonai.task.delete_task(task_id)
         click.echo("Cancelled task creation.")
         return
 
     # Given user's confirmation, continue with task creation
     try:
-        click.echo("Proceeding with task creation...")
         generate_response = horizonai.task.generate_task(task_id, objective)
+        formatted_output = json.dumps(generate_response, indent=4)
+        click.echo(formatted_output)
     except Exception as e:
-        # If error with generating task, then clean up task record and evaluation dataset before raising exception
+        # If error with generating task, then clean up task record before raising exception
         horizonai.task.delete_task(task_id)
         click.echo("Failed in task generation")
         click.echo(str(e))
         return
 
-    # Print task generation response
-    click.echo("=====")
-    formatted_output = json.dumps(generate_response, indent=4)
-    click.echo(formatted_output)
-
 
 # Get Task
 @click.command(name="get")
 @click.option(
     "--horizonai_api_key",
     default=os.environ.get("HORIZONAI_API_KEY"),
     prompt="HorizonAI API Key" if not os.environ.get("HORIZONAI_API_KEY") else False,
     help="The HorizonAI API key for the user.",
     hide_input=True,
 )
 @click.option("--task_id", prompt="Task ID", help="The ID of the task to retrieve.")
 def get_task(task_id, horizonai_api_key):
+    """Get details about a specific Task."""
     horizonai.api_key = horizonai_api_key
     try:
         result = horizonai.task.get_task(task_id)
         formatted_output = json.dumps(result, indent=4)
         click.echo(formatted_output)
     except Exception as e:
         click.echo(str(e))
@@ -365,14 +348,15 @@
     default=os.environ.get("HORIZONAI_API_KEY"),
     prompt="HorizonAI API Key" if not os.environ.get("HORIZONAI_API_KEY") else False,
     help="The HorizonAI API key for the user.",
     hide_input=True,
 )
 @click.option("--task_id", prompt="Task ID", help="The ID of the task to delete.")
 def delete_task(task_id, horizonai_api_key):
+    """Delete an existing Task."""
     horizonai.api_key = horizonai_api_key
     try:
         result = horizonai.task.delete_task(task_id)
         formatted_output = json.dumps(result, indent=4)
         click.echo(formatted_output)
     except HTTPError as e:
         click.echo(f"Error deleting task (HTTP Error): {str(e)}")
@@ -389,39 +373,74 @@
     help="The HorizonAI API key for the user.",
     hide_input=True,
 )
 @click.option("--task_id", prompt="Task ID", help="The ID of the task to deploy.")
 @click.option(
     "--inputs", prompt="Inputs", help="The inputs to the task in JSON format."
 )
+def deploy_task(horizonai_api_key, task_id, inputs):
+    """Deploy a Task based on provided input values."""
+    horizonai.api_key = horizonai_api_key
+
+    # Determine model provider for selected task
+    try:
+        task_details_response = horizonai.task.get_task(task_id)
+        task_details = task_details_response["task"]
+        model_name = task_details["prompts"][0]["model_name"]
+    except Exception as e:
+        click.echo(str(e))
+        return
+
+    # Get appropriate LLM provider API key
+    if model_name in ["gpt-3.5-turbo", "text-davinci-003"]:
+        if os.environ.get("OPENAI_API_KEY"):
+            horizonai.openai_api_key = os.environ.get("OPENAI_API_KEY")
+        else:
+            horizonai.openai_api_key = click.prompt(
+                text="OpenAI API Key (text hidden)", hide_input=True
+            )
+    elif model_name in ["claude-instant-v1", "claude-v1"]:
+        if os.environ.get("ANTHROPIC_API_KEY"):
+            horizonai.anthropic_api_key = os.environ.get("ANTHROPIC_API_KEY")
+        else:
+            horizonai.anthropic_api_key = click.prompt(
+                text="Anthropic API Key (text hidden)", hide_input=True
+            )
+
+    log_deployment = False
+    if click.confirm("Log deployment?"):
+        log_deployment = True
+    try:
+        inputs_dict = json.loads(inputs, strict=False)
+        result = horizonai.task.deploy_task(task_id, inputs_dict, log_deployment)
+        formatted_output = json.dumps(result, indent=4)
+        click.echo(formatted_output)
+    except Exception as e:
+        click.echo(str(e))
+
+
+# Download task deployment logs
+@click.command(name="view-logs")
 @click.option(
-    "--openai_api_key",
-    default=os.environ.get("OPENAI_API_KEY"),
-    prompt="OpenAI API Key (text hidden; type 'skip' if you're not using OpenAI)"
-    if not os.environ.get("OPENAI_API_KEY")
-    else False,
-    help="The OpenAI API key for the user.",
+    "--horizonai_api_key",
+    default=os.environ.get("HORIZONAI_API_KEY"),
+    prompt="HorizonAI API Key" if not os.environ.get("HORIZONAI_API_KEY") else False,
+    help="The HorizonAI API key for the user.",
     hide_input=True,
 )
 @click.option(
-    "--anthropic_api_key",
-    default=os.environ.get("ANTHROPIC_API_KEY"),
-    prompt="Anthropic API Key (text hidden; type 'skip' if you're not using Anthropic)"
-    if not os.environ.get("ANTHROPIC_API_KEY")
-    else False,
-    help="The Anthropic API key for the user.",
-    hide_input=True,
+    "--task_id",
+    prompt="Task ID",
+    help="The ID of the task to view logs for.",
 )
-def deploy_task(task_id, inputs, horizonai_api_key, openai_api_key, anthropic_api_key):
+def view_deployment_logs(horizonai_api_key, task_id):
+    """View Task deployment logs."""
     horizonai.api_key = horizonai_api_key
-    horizonai.openai_api_key = openai_api_key
-    horizonai.anthropic_api_key = anthropic_api_key
     try:
-        inputs_dict = json.loads(inputs)
-        result = horizonai.task.deploy_task(task_id, inputs_dict)
+        result = horizonai.task.view_deployment_logs(task_id)
         formatted_output = json.dumps(result, indent=4)
         click.echo(formatted_output)
     except Exception as e:
         click.echo(str(e))
 
 
 # Add CLI commands to their respective groups
@@ -440,14 +459,15 @@
 
 # Task-related commands
 task.add_command(list_tasks)
 task.add_command(generate_task)
 task.add_command(get_task)
 task.add_command(delete_task)
 task.add_command(deploy_task)
+task.add_command(view_deployment_logs)
 
 # Enable auto-completion
 try:
     import click_completion
 
     click_completion.init()
 except ImportError:
```

### Comparing `horizonai-0.1.8/horizonai/project.py` & `horizonai-0.1.9/horizonai/project.py`

 * *Files identical despite different names*

### Comparing `horizonai-0.1.8/horizonai/task.py` & `horizonai-0.1.9/horizonai/task.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     headers = {"X-Api-Key": horizonai.api_key}
     response = base._get(endpoint="/api/tasks", headers=headers)
     return response
 
 
 def create_task(
     name: str,
-    task_type: str,
     project_id: int,
     allowed_models: list,
+    task_type: str = "text_generation",
 ):
     if horizonai.api_key == None:
         raise Exception("Must set Horizon API key.")
     if type(allowed_models) != list or len(allowed_models) == 0:
         raise Exception("Must provide list with at least one allowed model.")
     headers = {"Content-Type": "application/json", "X-Api-Key": horizonai.api_key}
     payload = {
@@ -72,25 +72,26 @@
         "openai_api_key": horizonai.openai_api_key,
         "anthropic_api_key": horizonai.anthropic_api_key,
     }
     response = base._post(endpoint="/api/tasks/generate", json=payload, headers=headers)
     return response
 
 
-def deploy_task(task_id, inputs):
+def deploy_task(task_id, inputs, log_deployment=False):
     if horizonai.api_key == None:
         raise Exception("Must set Horizon API key.")
-    if horizonai.openai_api_key == None or horizonai.anthropic_api_key == None:
+    if horizonai.openai_api_key == None and horizonai.anthropic_api_key == None:
         raise Exception("Must set LLM provider API key.")
     headers = {"Content-Type": "application/json", "X-Api-Key": horizonai.api_key}
     payload = {
         "task_id": task_id,
         "inputs": inputs,
         "openai_api_key": horizonai.openai_api_key,
         "anthropic_api_key": horizonai.anthropic_api_key,
+        "log_deployment": log_deployment,
     }
     response = base._post(endpoint="/api/tasks/deploy", json=payload, headers=headers)
     return response
 
 
 def upload_evaluation_dataset(task_id, file_path):
     if horizonai.api_key == None:
@@ -99,7 +100,30 @@
     with open(file_path, "rb") as f:
         response = base._post(
             endpoint=f"/api/tasks/{task_id}/upload_evaluation_dataset",
             files={"evaluation_dataset": f},
             headers=headers,
         )
         return response
+
+
+def upload_output_schema(task_id, file_path):
+    if horizonai.api_key == None:
+        raise Exception("Must set Horizon API key.")
+    headers = {"X-Api-Key": horizonai.api_key}
+    with open(file_path, "rb") as f:
+        response = base._post(
+            endpoint=f"/api/tasks/{task_id}/upload_output_schema",
+            files={"output_schema": f},
+            headers=headers,
+        )
+        return response
+
+
+def view_deployment_logs(task_id):
+    if horizonai.api_key == None:
+        raise Exception("Must set Horizon API key.")
+    headers = {"X-Api-Key": horizonai.api_key}
+    response = base._get(
+        endpoint=f"/api/tasks/{task_id}/view_deployment_logs", headers=headers
+    )
+    return response
```

### Comparing `horizonai-0.1.8/horizonai.egg-info/PKG-INFO` & `horizonai-0.1.9/horizonai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: horizonai
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package and command line interface to access the Horizon AI API
 Home-page: https://www.gethorizon.ai
-Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.8.tar.gz
+Download-URL: https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.9.tar.gz
 Author: Horizon Team
 Author-email: team@gethorizon.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `horizonai-0.1.8/setup.py` & `horizonai-0.1.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from setuptools import setup, find_packages
 import os
 
 
 def read(file_name):
-    with open(os.path.join(os.path.dirname(__file__), file_name), "r", encoding="utf-8") as f:
+    with open(
+        os.path.join(os.path.dirname(__file__), file_name), "r", encoding="utf-8"
+    ) as f:
         return f.read()
 
 
 setup(
     name="horizonai",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     package_data={"": ["__init__.py"]},
     install_requires=[
         "requests",
         "click",
     ],
     entry_points={"console_scripts": ["horizonai=horizonai.cli:cli"]},
     author="Horizon Team",
     author_email="team@gethorizon.ai",
     license="MIT",
     description="Python package and command line interface to access the Horizon AI API",
-    long_description=read("README.md"),  # Include README.md content
-    long_description_content_type="text/markdown",  # Specify content type as Markdown
+    long_description=read("README.md"),
+    long_description_content_type="text/markdown",
     url="https://www.gethorizon.ai",
-    download_url="https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.8.tar.gz",
+    download_url="https://github.com/gethorizon-ai/horizonai-python/archive/refs/tags/v0.1.9.tar.gz",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

