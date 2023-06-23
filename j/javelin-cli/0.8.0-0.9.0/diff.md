# Comparing `tmp/javelin-cli-0.8.0.tar.gz` & `tmp/javelin-cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "javelin-cli-0.8.0.tar", max compression
+gzip compressed data, was "javelin-cli-0.9.0.tar", max compression
```

## Comparing `javelin-cli-0.8.0.tar` & `javelin-cli-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      812 2023-06-14 04:57:05.265432 javelin-cli-0.8.0/README.md
--rw-r--r--   0        0        0       22 2023-06-14 04:42:13.306827 javelin-cli-0.8.0/javelin/__init__.py
--rw-r--r--   0        0        0     6250 2023-06-14 04:42:13.157618 javelin-cli-0.8.0/javelin/__main__.py
--rw-r--r--   0        0        0        0 2022-06-20 23:44:18.476590 javelin-cli-0.8.0/javelin/utils/__init__.py
--rw-r--r--   0        0        0     1716 2022-07-15 05:36:25.525384 javelin-cli-0.8.0/javelin/utils/aws.py
--rw-r--r--   0        0        0     4494 2023-06-14 04:42:13.158776 javelin-cli-0.8.0/javelin/utils/github.py
--rw-r--r--   0        0        0     4391 2023-06-14 04:42:13.159443 javelin-cli-0.8.0/javelin/utils/slack.py
--rw-r--r--   0        0        0      633 2023-06-14 04:42:13.307351 javelin-cli-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1703 2023-06-14 05:02:33.949024 javelin-cli-0.8.0/setup.py
--rw-r--r--   0        0        0     1613 2023-06-14 05:02:33.949329 javelin-cli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      899 2023-06-14 05:06:16.318545 javelin-cli-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-23 00:28:57.642147 javelin-cli-0.9.0/javelin/__init__.py
+-rw-r--r--   0        0        0     6429 2023-06-23 00:29:54.151220 javelin-cli-0.9.0/javelin/__main__.py
+-rw-r--r--   0        0        0        0 2022-06-20 23:44:18.476590 javelin-cli-0.9.0/javelin/utils/__init__.py
+-rw-r--r--   0        0        0     1716 2022-07-15 05:36:25.525384 javelin-cli-0.9.0/javelin/utils/aws.py
+-rw-r--r--   0        0        0     4494 2023-06-23 00:20:12.089499 javelin-cli-0.9.0/javelin/utils/github.py
+-rw-r--r--   0        0        0     4391 2023-06-14 04:42:13.159443 javelin-cli-0.9.0/javelin/utils/slack.py
+-rw-r--r--   0        0        0      633 2023-06-23 00:29:09.825821 javelin-cli-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1794 2023-06-23 00:31:25.906753 javelin-cli-0.9.0/setup.py
+-rw-r--r--   0        0        0     1700 2023-06-23 00:31:25.907038 javelin-cli-0.9.0/PKG-INFO
```

### Comparing `javelin-cli-0.8.0/README.md` & `javelin-cli-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 
 ## Contribution
 ### Run lint
 ```sh
 pylint javelin
 ```
 
+### Increase version number in these files
+- `pyproject.toml`
+- `javelin/__init__.py`
+
 ### Create and push release commit
 ```sh
 git commit -m v1.2.3
 git tag v1.2.3
 git push
 git push --tags
 ```
```

### Comparing `javelin-cli-0.8.0/javelin/__main__.py` & `javelin-cli-0.9.0/javelin/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     match command:
         case 'pre-release':
             _prerelease()
         case 'release':
             _release()
         case '':
             print("javelin: missing command")
-            sys.exit(2)
+            sys.exit(1)
         case _:
             print(f"javelin: invalid command '{command}'")
             sys.exit(2)
 
     duration = time.time() - start_time
     print(f'Finished in {duration:0.2f} seconds')
 
@@ -69,48 +69,48 @@
     global project_name
     global bump_level
 
     try:
         opts, args = getopt.gnu_getopt(argv, 'hvP:l:p:', ['help', 'version', 'project=', 'bump-level=', 'pull-request='])
     except getopt.GetoptError:
         print(help_message)
-        sys.exit(2)
+        sys.exit(3)
 
     if len(args) > 0:
         command = args[0]
 
     for opt, arg in opts:
         if opt in ('-h', '--help'):
             print(help_message)
-            sys.exit()
+            sys.exit(4)
         if opt in ('-v', '--version'):
             print(__version__)
-            sys.exit()
+            sys.exit(5)
         elif opt in ('-P', '--project'):
             project_name = arg
         elif opt in ('-l', '--bump-level'):
             bump_level = arg
         elif opt in ('-p', '--pull-request'):
             pr_numbers.append(arg)
 
     pr_numbers.sort()
 
     if not project_name:
         print("\njavelin: missing project")
-        sys.exit(2)
+        sys.exit(6)
 
     if command != 'pre-release':
         return
 
     if not bump_level:
         print("\njavelin: missing bump level")
-        sys.exit(2)
+        sys.exit(7)
     elif bump_level not in ('major', 'minor', 'patch'):
         print("\njavelin: invalid bump level")
-        sys.exit(2)
+        sys.exit(8)
 
 def _prerelease():
     global start_time
 
     try:
         repo_name = _get_project_repo_name()
         repo = github.get_repo(repo_name)
@@ -123,15 +123,19 @@
             pull = github.fetch_pull_request(repo_name, pr_number)
             pulls.append(pull)
 
             print(f'      #{pull.number}: {pull.title} ({pull.head.ref})')
 
             if not pull.mergeable or pull.mergeable_state != 'clean':
                 print(f"\njavelin: pull request can't be merged ({pull.mergeable_state})")
-                sys.exit(2)
+                sys.exit(9)
+
+            if pull.base.ref != repo.default_branch:
+                print("\njavelin: pull request's base branch is different from the repo's")
+                sys.exit(10)
 
         print(f'\n  2. Create a new GitHub Release with version {prerelease_version}')
         print(f'\n  3. Deploy the "{repo.default_branch}" branch to Staging 🚀\n')
 
         print('\n\033[1mDo you want to continue?\033[0m')
         print('  Only "yes" will be accepted.\n')
 
@@ -156,15 +160,15 @@
     try:
         repo_name = _get_project_repo_name()
         repo = github.get_repo(repo_name)
         latest_prerelease = github.get_latest_prerelease(repo)
 
         if not latest_prerelease:
             print("javelin: repository doesn't have any pre-releases")
-            sys.exit(2)
+            sys.exit(11)
 
         release_version = latest_prerelease.title
 
         print('The following actions will be performed:\n')
         print(f'\n  1. Deploy version {release_version} to Production 🚀\n')
         print('\n\033[1mDo you want to continue?\033[0m')
         print('  Only "yes" will be accepted.\n')
@@ -186,11 +190,11 @@
     with open('./config/projects.yml', 'r', encoding='utf-8') as stream:
         try:
             config = yaml.safe_load(stream)
 
             return config[project_name]['repo_full_names']
         except (KeyError, yaml.YAMLError):
             print("\njavelin: invalid project name")
-            sys.exit(2)
+            sys.exit(12)
 
 if __name__ == '__main__':
     main(sys.argv[1:])
```

### Comparing `javelin-cli-0.8.0/javelin/utils/aws.py` & `javelin-cli-0.9.0/javelin/utils/aws.py`

 * *Files identical despite different names*

### Comparing `javelin-cli-0.8.0/javelin/utils/github.py` & `javelin-cli-0.9.0/javelin/utils/github.py`

 * *Files identical despite different names*

### Comparing `javelin-cli-0.8.0/javelin/utils/slack.py` & `javelin-cli-0.9.0/javelin/utils/slack.py`

 * *Files identical despite different names*

### Comparing `javelin-cli-0.8.0/pyproject.toml` & `javelin-cli-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "javelin-cli"
-version = "0.8.0"
+version = "0.9.0"
 description = "CLI tool for managing Spearly deployments."
 authors = ["David Grilli <dj@unimal.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/unimal-jp/javelin"
 packages = [
     { include = "javelin" }
```

### Comparing `javelin-cli-0.8.0/setup.py` & `javelin-cli-0.9.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'packaging>=21.3,<22.0',
  'python-dotenv>=0.20.0,<0.21.0',
  'python-semantic-release>=7.29.2,<8.0.0',
  'slack-sdk>=3.17.2,<4.0.0']
 
 setup_kwargs = {
     'name': 'javelin-cli',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'CLI tool for managing Spearly deployments.',
-    'long_description': '# Javelin\n\nCLI tool for managing Spearly deployments.\n\n## Requirements\n- Python 3.10+\n- `GITHUB_ACCESS_TOKEN` environment variable set to a **GitHub Personal Access Token** with `repo` scope ([Ref](https://github.com/settings/tokens))\n- **AWS IAM User** with `codepipeline:StartPipelineExecution` permission to the required resources ([Ref](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html#configuration))\n\n## Installation\n```sh\nbrew install pyenv\npyenv install 3.10:latest\n[pyenv exec] pip install javelin-cli\n```\n\n## Usage\n```sh\npython -m javelin --help\n```\n\n## Contribution\n### Run lint\n```sh\npylint javelin\n```\n\n### Create and push release commit\n```sh\ngit commit -m v1.2.3\ngit tag v1.2.3\ngit push\ngit push --tags\n```\n\n### Build and publish\n```sh\npoetry build\npoetry publish\n```\n',
+    'long_description': '# Javelin\n\nCLI tool for managing Spearly deployments.\n\n## Requirements\n- Python 3.10+\n- `GITHUB_ACCESS_TOKEN` environment variable set to a **GitHub Personal Access Token** with `repo` scope ([Ref](https://github.com/settings/tokens))\n- **AWS IAM User** with `codepipeline:StartPipelineExecution` permission to the required resources ([Ref](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html#configuration))\n\n## Installation\n```sh\nbrew install pyenv\npyenv install 3.10:latest\n[pyenv exec] pip install javelin-cli\n```\n\n## Usage\n```sh\npython -m javelin --help\n```\n\n## Contribution\n### Run lint\n```sh\npylint javelin\n```\n\n### Increase version number in these files\n- `pyproject.toml`\n- `javelin/__init__.py`\n\n### Create and push release commit\n```sh\ngit commit -m v1.2.3\ngit tag v1.2.3\ngit push\ngit push --tags\n```\n\n### Build and publish\n```sh\npoetry build\npoetry publish\n```\n',
     'author': 'David Grilli',
     'author_email': 'dj@unimal.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/unimal-jp/javelin',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `javelin-cli-0.8.0/PKG-INFO` & `javelin-cli-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: javelin-cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: CLI tool for managing Spearly deployments.
 Home-page: https://github.com/unimal-jp/javelin
 License: MIT
 Author: David Grilli
 Author-email: dj@unimal.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -43,14 +43,18 @@
 
 ## Contribution
 ### Run lint
 ```sh
 pylint javelin
 ```
 
+### Increase version number in these files
+- `pyproject.toml`
+- `javelin/__init__.py`
+
 ### Create and push release commit
 ```sh
 git commit -m v1.2.3
 git tag v1.2.3
 git push
 git push --tags
 ```
```

