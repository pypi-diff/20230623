# Comparing `tmp/cloud_radar-0.8.1a1.tar.gz` & `tmp/cloud_radar-0.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_radar-0.8.1a1.tar", max compression
+gzip compressed data, was "cloud_radar-0.9.0a0.tar", max compression
```

## Comparing `cloud_radar-0.8.1a1.tar` & `cloud_radar-0.9.0a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/LICENSE.txt
--rw-r--r--   0        0        0    13927 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/README.md
--rw-r--r--   0        0        0     1435 2023-06-16 23:18:56.368052 cloud_radar-0.8.1a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/cf/__init__.py
--rw-r--r--   0        0        0       48 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/cf/e2e/__init__.py
--rw-r--r--   0        0        0     1677 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/cf/e2e/_stack.py
--rw-r--r--   0        0        0       57 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/__init__.py
--rw-r--r--   0        0        0      711 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_condition.py
--rw-r--r--   0        0        0     1822 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_output.py
--rw-r--r--   0        0        0     3199 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_parameter.py
--rw-r--r--   0        0        0     3872 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_resource.py
--rw-r--r--   0        0        0     5230 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_stack.py
--rw-r--r--   0        0        0    20352 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_template.py
--rw-r--r--   0        0        0    24791 2023-06-16 23:18:41.235859 cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/functions.py
--rw-r--r--   0        0        0    15083 1970-01-01 00:00:00.000000 cloud_radar-0.8.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/LICENSE.txt
+-rw-r--r--   0        0        0    14071 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/README.md
+-rw-r--r--   0        0        0     1435 2023-06-23 18:35:02.126889 cloud_radar-0.9.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/cf/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/cf/e2e/__init__.py
+-rw-r--r--   0        0        0     1677 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/cf/e2e/_stack.py
+-rw-r--r--   0        0        0       57 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_condition.py
+-rw-r--r--   0        0        0     1822 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_output.py
+-rw-r--r--   0        0        0     3199 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_parameter.py
+-rw-r--r--   0        0        0     3872 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_resource.py
+-rw-r--r--   0        0        0     5230 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_stack.py
+-rw-r--r--   0        0        0    23707 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_template.py
+-rw-r--r--   0        0        0    24791 2023-06-23 18:34:48.686524 cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/functions.py
+-rw-r--r--   0        0        0    15227 1970-01-01 00:00:00.000000 cloud_radar-0.9.0a0/PKG-INFO
```

### Comparing `cloud_radar-0.8.1a1/LICENSE.txt` & `cloud_radar-0.9.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.1a1/README.md` & `cloud_radar-0.9.0a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -337,14 +337,15 @@
 Levi - [@shady_cuz](https://twitter.com/shady_cuz)
 
 <!-- ACKNOWLEDGEMENTS -->
 ## Acknowledgements
 * [Taskcat](https://aws-quickstart.github.io/taskcat/)
 * [Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/)
 * [Best-README-Template](https://github.com/othneildrew/Best-README-Template)
+* @dhutchison - He was the first contributor to this project and finished the last couple of features to make this project complete. Thank you!
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [python-shield]: https://img.shields.io/pypi/pyversions/cloud-radar?style=for-the-badge
 [version-shield]: https://img.shields.io/pypi/v/cloud-radar?label=latest&style=for-the-badge
 [pypi-url]: https://pypi.org/project/cloud-radar/
 [test-shield]: https://img.shields.io/github/actions/workflow/status/DontShaveTheYak/cloud-radar/test.yml?label=Tests&style=for-the-badge
```

#### html2text {}

```diff
@@ -130,20 +130,22 @@
 Changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git
 push origin feature/AmazingFeature`) 5. Open a Pull Request ## License
 Distributed under the Apache-2.0 License. See [LICENSE.txt](./LICENSE.txt) for
 more information. ## Contact Levi - [@shady_cuz](https://twitter.com/shady_cuz)
 ## Acknowledgements * [Taskcat](https://aws-quickstart.github.io/taskcat/) *
 [Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-
 setup/) * [Best-README-Template](https://github.com/othneildrew/Best-README-
-Template)   [python-shield]: https://img.shields.io/pypi/pyversions/cloud-
-radar?style=for-the-badge [version-shield]: https://img.shields.io/pypi/v/
-cloud-radar?label=latest&style=for-the-badge [pypi-url]: https://pypi.org/
-project/cloud-radar/ [test-shield]: https://img.shields.io/github/actions/
-workflow/status/DontShaveTheYak/cloud-radar/test.yml?label=Tests&style=for-the-
-badge [test-url]: https://github.com/DontShaveTheYak/cloud-radar/
+Template) * @dhutchison - He was the first contributor to this project and
+finished the last couple of features to make this project complete. Thank you!
+[python-shield]: https://img.shields.io/pypi/pyversions/cloud-radar?style=for-
+the-badge [version-shield]: https://img.shields.io/pypi/v/cloud-
+radar?label=latest&style=for-the-badge [pypi-url]: https://pypi.org/project/
+cloud-radar/ [test-shield]: https://img.shields.io/github/actions/workflow/
+status/DontShaveTheYak/cloud-radar/test.yml?label=Tests&style=for-the-badge
+[test-url]: https://github.com/DontShaveTheYak/cloud-radar/
 actions?query=workflow%3ATests+branch%3Amaster [codecov-shield]: https://
 img.shields.io/codecov/c/gh/DontShaveTheYak/cloud-radar?color=green&style=for-
 the-badge&token=NE5C92139X [codecov-url]: https://codecov.io/gh/
 DontShaveTheYak/cloud-radar [contributors-shield]: https://img.shields.io/
 github/contributors/DontShaveTheYak/cloud-radar.svg?style=for-the-badge
 [contributors-url]: https://github.com/DontShaveTheYak/cloud-radar/graphs/
 contributors [forks-shield]: https://img.shields.io/github/forks/
```

### Comparing `cloud_radar-0.8.1a1/pyproject.toml` & `cloud_radar-0.9.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-radar"
-version = "0.8.1a1"
+version = "0.9.0a0"
 description = "Run functional tests on cloudformation stacks."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/DontShaveTheYak/cloud-radar"
 keywords = ["aws", "cloudformation", "cloud-radar", "testing", "taskcat", "cloud", "radar"]
 classifiers = [
```

### Comparing `cloud_radar-0.8.1a1/src/cloud_radar/cf/e2e/_stack.py` & `cloud_radar-0.9.0a0/src/cloud_radar/cf/e2e/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_condition.py` & `cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_condition.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_output.py` & `cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_output.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_parameter.py` & `cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_parameter.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_resource.py` & `cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_resource.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_stack.py` & `cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/_template.py` & `cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/_template.py`

 * *Files 11% similar despite different names*

```diff
@@ -399,14 +399,15 @@
     are not met.
     Args:
         parameter_name (str): The name of the parameter being validated
         parameter_definition (Dict): The parameter definition being validated
                                     against
         parameter_value (str): The supplied parameter value being validated
     """
+
     if parameter_definition["Type"] == "String":
         validate_string_parameter_constraints(
             parameter_name, parameter_definition, parameter_value
         )
     elif parameter_definition["Type"] == "CommaDelimitedList":
         # When applied to a parameter of type CommaDelimitedList,
         # each value in the list must meet the String type criteria
@@ -414,24 +415,94 @@
             validate_string_parameter_constraints(
                 parameter_name, parameter_definition, part.strip()
             )
     elif parameter_definition["Type"] == "Number":
         validate_number_parameter_constraints(
             parameter_name, parameter_definition, parameter_value
         )
-    elif parameter_definition["Type"] == "List<Number>":
-        # The docs are not as clear here but I think it will be
-        # the same as CommaDelimitedList - run the number parameter
-        # constraints for each item in the list
+    elif parameter_definition["Type"].startswith("AWS::"):
+        validate_aws_parameter_constraints(
+            parameter_name, parameter_definition["Type"], parameter_value
+        )
+    elif parameter_definition["Type"].startswith("List<"):
+        # All list types runs the single value validation for all items
+        trimmed_type = parameter_definition["Type"][5:-1]
+
+        # There are a couple though that are not supported
+        if trimmed_type == "AWS::EC2::KeyPair::KeyName" or trimmed_type == "String":
+            # this is a type that isn't valid as a list, but is
+            # as a single item
+            raise ValueError(f"Type {trimmed_type} is not valid in a List<>")
+
+        # Iterate over each item and call this method again with an
+        # updated definition for the non-list type
+        updated_defintion = parameter_definition.copy()
+        updated_defintion["Type"] = trimmed_type
+
         for part in parameter_value.split(","):
-            validate_number_parameter_constraints(
-                parameter_name, parameter_definition, part.strip()
+            validate_parameter_constraints(
+                parameter_name, updated_defintion, part.strip()
             )
 
 
+def validate_aws_parameter_constraints(
+    parameter_name: str, parameter_type: str, parameter_value: str
+):
+    """
+    Validate that the parameter value matches any constraints
+    that are applicable for an AWS type parameter
+
+    This method will raise a ValueError if any validation constraints
+    are not met.
+    Args:
+        parameter_name (str): The name of the parameter being validated
+        parameter_type (str): The AWS type of the parameter being validated
+                                    against
+        parameter_value (str): The supplied parameter value being validated
+    """
+
+    parameter_type_regexes = {
+        # Reference for this was
+        # https://gist.github.com/rams3sh/4858d5150acba5383dd697fda54dda2c
+        "AWS::EC2::AvailabilityZone::Name": (
+            "^(af|ap|ca|eu|me|sa|us)-(central|north|(north(?:east|west))|"
+            "south|south(?:east|west)|east|west)-[0-9]+[a-z]{1}$"
+        ),
+        # Reference for the next few are
+        # https://blog.skeddly.com/2016/01/long-ec2-instance-ids-are-fully-supported.html
+        "AWS::EC2::Image::Id": "^ami-[a-f0-9]{8}([a-f0-9]{9})?$",
+        "AWS::EC2::Instance::Id": "^i-[a-f0-9]{8}([a-f0-9]{9})?$",
+        "AWS::EC2::SecurityGroup::Id": "^sg-[a-f0-9]{8}([a-f0-9]{9})?$",
+        "AWS::EC2::Subnet::Id": "^subnet-[a-f0-9]{8}([a-f0-9]{9})?$",
+        "AWS::EC2::VPC::Id": "^vpc-[a-f0-9]{8}([a-f0-9]{9})?$",
+        "AWS::EC2::Volume::Id": "^vol-[a-f0-9]{8}([a-f0-9]{9})?$",
+        # Reference for this was
+        # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-security-group.html#cfn-ec2-securitygroup-groupname
+        "AWS::EC2::SecurityGroup::GroupName": r"^[a-zA-Z0-9 ._\-:\/()#,@\[\]+=&;{}!$*]{1,255}$",
+        # Bit of a guess this one, not sure what the minimum bound should be
+        # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-route53-recordset.html#cfn-route53-recordset-hostedzoneid
+        "AWS::Route53::HostedZone::Id": "^[A-Z0-9]{,32}$",
+        # All the docs say for this type is up to 255 ascii characters
+        "AWS::EC2::KeyPair::KeyName": "^[ -~]{1,255}$",
+    }
+    param_regex = parameter_type_regexes.get(parameter_type)
+
+    if param_regex is None:
+        # If a regex is defined, we know the regex to validate the parameter
+        raise KeyError(f"Unsupported parameter type {parameter_type}")
+
+    if not re.match(param_regex, parameter_value):
+        raise ValueError(
+            (
+                f"Value {parameter_value} does not match the expected pattern "
+                f"for parameter {parameter_name} and type {parameter_type}"
+            )
+        )
+
+
 def validate_number_parameter_constraints(
     parameter_name: str, parameter_definition: dict, parameter_value: str
 ):
     """
     Validate that the parameter value matches any constraints
     that are applicable for Number value parameters
     (min/max value)
```

### Comparing `cloud_radar-0.8.1a1/src/cloud_radar/cf/unit/functions.py` & `cloud_radar-0.9.0a0/src/cloud_radar/cf/unit/functions.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.8.1a1/PKG-INFO` & `cloud_radar-0.9.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-radar
-Version: 0.8.1a1
+Version: 0.9.0a0
 Summary: Run functional tests on cloudformation stacks.
 Home-page: https://github.com/DontShaveTheYak/cloud-radar
 License: Apache-2.0
 Keywords: aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -364,14 +364,15 @@
 Levi - [@shady_cuz](https://twitter.com/shady_cuz)
 
 <!-- ACKNOWLEDGEMENTS -->
 ## Acknowledgements
 * [Taskcat](https://aws-quickstart.github.io/taskcat/)
 * [Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-setup/)
 * [Best-README-Template](https://github.com/othneildrew/Best-README-Template)
+* @dhutchison - He was the first contributor to this project and finished the last couple of features to make this project complete. Thank you!
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [python-shield]: https://img.shields.io/pypi/pyversions/cloud-radar?style=for-the-badge
 [version-shield]: https://img.shields.io/pypi/v/cloud-radar?label=latest&style=for-the-badge
 [pypi-url]: https://pypi.org/project/cloud-radar/
 [test-shield]: https://img.shields.io/github/actions/workflow/status/DontShaveTheYak/cloud-radar/test.yml?label=Tests&style=for-the-badge
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-radar Version: 0.8.1a1 Summary: Run
+Metadata-Version: 2.1 Name: cloud-radar Version: 0.9.0a0 Summary: Run
 functional tests on cloudformation stacks. Home-page: https://github.com/
 DontShaveTheYak/cloud-radar License: Apache-2.0 Keywords:
 aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar Author: Levi Blaney
 Author-email: shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
@@ -146,20 +146,22 @@
 Changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git
 push origin feature/AmazingFeature`) 5. Open a Pull Request ## License
 Distributed under the Apache-2.0 License. See [LICENSE.txt](./LICENSE.txt) for
 more information. ## Contact Levi - [@shady_cuz](https://twitter.com/shady_cuz)
 ## Acknowledgements * [Taskcat](https://aws-quickstart.github.io/taskcat/) *
 [Hypermodern Python](https://cjolowicz.github.io/posts/hypermodern-python-01-
 setup/) * [Best-README-Template](https://github.com/othneildrew/Best-README-
-Template)   [python-shield]: https://img.shields.io/pypi/pyversions/cloud-
-radar?style=for-the-badge [version-shield]: https://img.shields.io/pypi/v/
-cloud-radar?label=latest&style=for-the-badge [pypi-url]: https://pypi.org/
-project/cloud-radar/ [test-shield]: https://img.shields.io/github/actions/
-workflow/status/DontShaveTheYak/cloud-radar/test.yml?label=Tests&style=for-the-
-badge [test-url]: https://github.com/DontShaveTheYak/cloud-radar/
+Template) * @dhutchison - He was the first contributor to this project and
+finished the last couple of features to make this project complete. Thank you!
+[python-shield]: https://img.shields.io/pypi/pyversions/cloud-radar?style=for-
+the-badge [version-shield]: https://img.shields.io/pypi/v/cloud-
+radar?label=latest&style=for-the-badge [pypi-url]: https://pypi.org/project/
+cloud-radar/ [test-shield]: https://img.shields.io/github/actions/workflow/
+status/DontShaveTheYak/cloud-radar/test.yml?label=Tests&style=for-the-badge
+[test-url]: https://github.com/DontShaveTheYak/cloud-radar/
 actions?query=workflow%3ATests+branch%3Amaster [codecov-shield]: https://
 img.shields.io/codecov/c/gh/DontShaveTheYak/cloud-radar?color=green&style=for-
 the-badge&token=NE5C92139X [codecov-url]: https://codecov.io/gh/
 DontShaveTheYak/cloud-radar [contributors-shield]: https://img.shields.io/
 github/contributors/DontShaveTheYak/cloud-radar.svg?style=for-the-badge
 [contributors-url]: https://github.com/DontShaveTheYak/cloud-radar/graphs/
 contributors [forks-shield]: https://img.shields.io/github/forks/
```

