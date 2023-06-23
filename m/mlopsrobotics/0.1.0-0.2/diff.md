# Comparing `tmp/mlopsrobotics-0.1.0.tar.gz` & `tmp/mlopsrobotics-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlopsrobotics-0.1.0.tar", max compression
+gzip compressed data, was "mlopsrobotics-0.2.tar", max compression
```

## Comparing `mlopsrobotics-0.1.0.tar` & `mlopsrobotics-0.2.tar`

### file list

```diff
@@ -1,6 +1,20 @@
--rw-r--r--   0        0        0     9793 2023-05-26 14:03:55.350450 mlopsrobotics-0.1.0/README.md
--rw-r--r--   0        0        0     1062 2023-05-26 14:03:55.352874 mlopsrobotics-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2987 2023-05-26 15:01:57.050486 mlopsrobotics-0.1.0/src/mlopsrobotics/azure/setup_data.py
--rw-r--r--   0        0        0     1080 2023-05-26 14:03:55.353171 mlopsrobotics-0.1.0/src/mlopsrobotics/azure/setup_trainingjob.py
--rw-r--r--   0        0        0        0 2023-05-26 15:03:49.925054 mlopsrobotics-0.1.0/src/mlopsrobotics/pypi.py
--rw-r--r--   0        0        0    11445 1970-01-01 00:00:00.000000 mlopsrobotics-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13505 2023-06-23 13:53:01.726138 mlopsrobotics-0.2/README.md
+-rw-r--r--   0        0        0     1626 2023-06-23 14:12:03.355434 mlopsrobotics-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2977 2023-06-22 13:36:44.192678 mlopsrobotics-0.2/src/mlopsrobotics/azure/API_use.py
+-rw-r--r--   0        0        0     2711 2023-06-23 13:53:01.726689 mlopsrobotics-0.2/src/mlopsrobotics/azure/LOC_hyperparametingtuning.py
+-rw-r--r--   0        0        0     3785 2023-06-23 07:27:22.859555 mlopsrobotics-0.2/src/mlopsrobotics/azure/PipelineScheduler.py
+-rw-r--r--   0        0        0     1096 2023-06-07 12:50:08.414016 mlopsrobotics-0.2/src/mlopsrobotics/azure/__pycache__/component_train_loc.cpython-38.pyc
+-rw-r--r--   0        0        0     2782 2023-06-23 08:25:46.598902 mlopsrobotics-0.2/src/mlopsrobotics/azure/endpoint_inference_LOC.py
+-rw-r--r--   0        0        0     3251 2023-06-23 08:25:46.599243 mlopsrobotics-0.2/src/mlopsrobotics/azure/endpoint_inference_YOLO.py
+-rw-r--r--   0        0        0     4342 2023-06-22 13:36:20.293094 mlopsrobotics-0.2/src/mlopsrobotics/azure/pipeline_inference.py
+-rw-r--r--   0        0        0     5429 2023-06-22 14:03:27.100844 mlopsrobotics-0.2/src/mlopsrobotics/azure/pipeline_train_loc.py
+-rw-r--r--   0        0        0     5962 2023-06-23 08:25:46.599990 mlopsrobotics-0.2/src/mlopsrobotics/azure/pipeline_train_loc_scheduler.py
+-rw-r--r--   0        0        0     6943 2023-06-23 13:53:01.727917 mlopsrobotics-0.2/src/mlopsrobotics/azure/pipeline_train_yolo.py
+-rw-r--r--   0        0        0     7381 2023-06-23 08:25:46.600322 mlopsrobotics-0.2/src/mlopsrobotics/azure/pipeline_train_yolo_scheduler.py
+-rw-r--r--   0        0        0     4553 2023-06-23 13:53:01.729645 mlopsrobotics-0.2/src/mlopsrobotics/azure/register_model.py
+-rw-r--r--   0        0        0     3287 2023-06-22 11:31:20.391259 mlopsrobotics-0.2/src/mlopsrobotics/azure/setup_data.py
+-rw-r--r--   0        0        0     1684 2023-06-22 11:31:20.391945 mlopsrobotics-0.2/src/mlopsrobotics/azure/setup_trainingjob.py
+-rw-r--r--   0        0        0     5612 2023-06-22 20:24:38.246087 mlopsrobotics-0.2/src/mlopsrobotics/azure/traincostanalysis.py
+-rw-r--r--   0        0        0     3249 2023-06-20 10:03:27.558410 mlopsrobotics-0.2/src/mlopsrobotics/logs/inference.log
+-rw-r--r--   0        0        0      488 2023-06-22 11:31:20.392583 mlopsrobotics-0.2/src/mlopsrobotics/pypi.py
+-rw-r--r--   0        0        0    15697 1970-01-01 00:00:00.000000 mlopsrobotics-0.2/PKG-INFO
```

### Comparing `mlopsrobotics-0.1.0/PKG-INFO` & `mlopsrobotics-0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 Metadata-Version: 2.1
 Name: mlopsrobotics
-Version: 0.1.0
+Version: 0.2
 Summary: 
 Author: MichaelNed
 Author-email: 213566@buas.nl
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansimarkup (>=1.5.0,<2.0.0)
+Requires-Dist: autopep8 (>=2.0.2,<3.0.0)
 Requires-Dist: azure-ai-ml (>=1.7.2,<2.0.0)
 Requires-Dist: azure-identity (>=1.13.0,<2.0.0)
+Requires-Dist: azure-keyvault-secrets (>=4.7.0,<5.0.0)
 Requires-Dist: azureml (>=0.2.7,<0.3.0)
 Requires-Dist: azureml-core (>=1.51.0,<2.0.0)
+Requires-Dist: azureml-dataset-runtime (>=1.51.0,<2.0.0)
+Requires-Dist: azureml-mlflow (>=1.51.0,<2.0.0)
+Requires-Dist: black (>=23.3.0,<24.0.0)
+Requires-Dist: fastapi (>=0.97.0,<0.98.0)
+Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: gym (>=0.26.2,<0.27.0)
 Requires-Dist: gymnasium (>=0.28.1,<0.29.0)
 Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: mldesigner (>=0.1.0b13,<0.2.0)
+Requires-Dist: mlflow (>=2.3.2,<3.0.0)
 Requires-Dist: mujoco (>=2.3.5,<3.0.0)
+Requires-Dist: mypy (>=1.4.0,<2.0.0)
 Requires-Dist: numpy (>=1.19.3,<2.0.0)
-Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
+Requires-Dist: opencv-python-headless (>=4.5.0.72,<5.0.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: poetry2conda (>=0.3.0,<0.4.0)
+Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
+Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: roboflow (>=1.0.8,<2.0.0)
 Requires-Dist: robosuite (>=1.4.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: setuptools (>=67.8.0,<68.0.0)
 Requires-Dist: sphinx (>=4.3.0,<5.0.0)
@@ -38,14 +51,15 @@
 Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0)
 Requires-Dist: termcolor (>=2.3.0,<3.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: torchaudio (>=2.0.2,<3.0.0)
 Requires-Dist: torchvision (>=0.15.1,<0.16.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: ultralytics (>=8.0.101,<9.0.0)
+Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: wandb (>=0.15.3,<0.16.0)
 Description-Content-Type: text/markdown
 
 # Object Detection, Localization, and Pose Prediction for Robotic Manipulation
 
 The **Object Detection, Localization, and Pose Prediction** project is a Python package specifically designed for robotic manipulation tasks. The package leverages the latest advancements in computer vision and deep learning techniques to enable robust object detection, accurate localization, and precise pose prediction in a robotic environment.
 The system is built upon a proof-of-concept (PoC), which includes notebooks and scripts. It aims to provide a modular and platform-agnostic solution, ensuring compatibility with various robotic platforms and environments.
@@ -85,49 +99,111 @@
 - [Ultralytics](https://github.com/ultralytics/yolov5) (version 8.0.101 or later)
 
 ## Requirements
 The required Python packages and their versions are listed in the `pyproject.toml` file:
 
 ```plaintext
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8.1,<4.0"
 pandas = "^2.0.1"
 torch = "^2.0.0"
-opencv-python = "^4.7.0.72"
 pillow = "^9.5.0"
 requests = "^2.30.0"
 psutil = "^5.9.5"
 torchvision = "^0.15.1"
 pyyaml = "^6.0"
 tqdm = "^4.65.0"
 matplotlib = "^3.7.1"
 seaborn = "^0.12.2"
-sphinx = "^1.6"
+sphinx = "^4.3.0"
 sphinx-autobuild = "^2021.3.14"
 sphinx-rtd-theme = "^1.2.0"
 roboflow = "^1.0.8"
 pytest = "^7.3.1"
-numpy = "^1.24.3"
+numpy = "^1.19.3"
 loguru = "^0.7.0"
 ansimarkup = "^1.5.0"
 ultralytics = "^8.0.101"
+robosuite = "^1.4.0"
+mujoco = "^2.3.5"
+gymnasium = "^0.28.1"
+termcolor = "^2.3.0"
+h5py = "^3.8.0"
+gym = "^0.26.2"
+azureml = "^0.2.7"
+azureml-core = "^1.51.0"
+setuptools = "^67.8.0"
+wandb = "^0.15.3"
+torchaudio = "^2.0.2"
+azure-ai-ml = "^1.7.2"
+azure-identity = "^1.13.0"
+poetry2conda = "^0.3.0"
+opencv-python-headless = "^4.5.0.72"
+mlflow = "^2.3.2"
+azureml-mlflow = "^1.51.0"
+pyarrow = "^8.0.0"
+azureml-dataset-runtime = "^1.51.0"
+mldesigner = "^0.1.0b13"
+python-multipart = "^0.0.6"
+fastapi = "^0.97.0"
+uvicorn = "^0.22.0"
+azure-keyvault-secrets = "^4.7.0"
+flake8 = "^6.0.0"
+autopep8 = "^2.0.2"
+black = "^23.3.0"
+pre-commit = "^3.3.3"
+mypy = "^1.4.0"
+
+[tool.poetry.dev-dependencies]
+ipython = "*"
+poethepoet = "^0.10.0"
+
+[tool.poetry.group.dev.dependencies]
+ipykernel = "^6.23.1"
+
+[tool.poetry2conda]
+name = "mark-processor"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.poe.tasks]
+force-cuda18 = "python -m pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118"
 ```
 
 Ensure you have these packages installed with the specified versions by using a package manager like [Poetry](https://python-poetry.org/) or by manually installing them using `pip`.
 
 Please refer to the respective documentation of each package for installation instructions specific to your operating system.
 
 ## Installation
-To install the **MLOpsRobotics** package from PyPI, follow these steps:
+To install the **MLOpsRobotics** package, follow these steps:
+
+**Recommended** installation:
+1. Make sure you have Poetry installed on your system. If you don't have it installed, you can follow the installation instructions for your operating system from the official Poetry documentation: https://python-poetry.org/docs/#installation
+2. Clone the [GitHub repository](https://github.com/BredaUniversityADSAI/2022-23d-fga2_p1-adsai-group-mlops_robotics/tree/main).
+   ```
+   git clone https://github.com/BredaUniversityADSAI/2022-23d-fga2_p1-adsai-group-mlops_robotics.git
+   ```
+3. Once you have Poetry installed, navigate to the project directory that contains the existing Poetry environment.
+   ```
+   cd 2022-23d-fga2_p1-adsai-group-mlops_robotics/MLOpsRobotics
+   ```
+4. In the project directory, you should see a pyproject.toml file, which specifies the project dependencies and other configuration         details. To create the environment based on the pyproject.toml file, run the following command:
+   ```
+   poetry install
+   ```
+5. Make sure to activate the environment if not automaticly
 
+Not recommended installation:
 1. Ensure you have Python (version 3.8 or later) installed on your system.
 2. Open a terminal or command prompt.
 3. Run the following command to install the package using `pip`:
 
-   ```bash
+   ```
    pip install mlopsrobotics
    ```
 
    This command will download and install the package along with its dependencies.
 
 4. Once the installation is complete, you can import the package into your Python scripts or notebooks and use its functionality.
 
@@ -135,89 +211,109 @@
 
 ## Usage Inference.py
 The `inference.py` script performs inference using YOLO and a localization model on an image. It takes command-line arguments to specify the input parameters, but also allows for interactive user input to change the default settings.
 
 ### Prerequisites
 Before using the `inference.py` script, make sure you have the following prerequisites:
 
-- YOLO model weight file (`best.pt`) in the `data` directory.
-- Image file to perform inference on (default: `5-c.png`) in the `data/images` directory.
-- Localization model weight file (`weights_Localization_XY_YAW.pt`) in the `data` directory.
+## Default Setup:
+- The default YOLO model weight file (`best.pt`) should be located in the `data/Yolo_weights` directory.
+- The default image file to perform inference on (`5-c.png`) should be present in the `data/images` directory.
+- The default localization model weight file (`weights_Localization_XY_YAW.pt`) should be located in the `data/object_loc_weights` directory.
+
+## Custom Model Setup:
+- If you want to use your own model, please provide the corresponding model files:
+  - YOLO model weight file should be placed in the `data/Yolo_weights` directory.
+  - PNG image file for inference should be located in the `data/test_images/5-c.png` directory.
+  - Localization model weight file should be present in the `data/object_loc_weights` directory.
+
+To use your own models and alter the default options, run the `inference.py` script with the `--user_input yes` flag. This will enable you to provide custom paths for the model files and images, overriding the default options. For example, you can use the following path for the YOLO model: `./data/Yolo_weights/<your_model.pt>`. Make sure to specify the correct paths when using the `--user_input yes` flag.
 
 ### Command-Line Arguments
 The script supports the following command-line arguments:
 
 - `--user_input`: Allows changing the default settings interactively. Accepts values `yes` or `no`. (default: `no`)
-- `--model_path`: Path to the YOLO model weight file. (default: `data/best.pt`)
-- `--image_path`: Path to the image file to perform inference on. (default: `data/images/5-c.png`)
-- `--loc_model_path`: Path to the localization model weight file. (default: `data/weights_Localization_XY_YAW.pt`)
+- `--model_path`: Path to the YOLO model weight file. (default: `./data/Yolo_weights/best.pt`)
+- `--image_path`: Path to the image file to perform inference on. (default: `./data/test_images/5-c.png`)
+- `--loc_model_path`: Path to the localization model weight file. (default: `./data/object_loc_weights/weights_Localization_XY_YAW.pt`)
 
 ### Usage Examples
 1. Perform inference using default settings:
     ```
-    python inference.py
+    python src/inference.py
     ```
 
-2. Perform inference with custom settings:
+2. Perform inference with custom settings interactively:
     ```
-    python inference.py --user_input=yes --model_path=path/to/model.pt --image_path=path/to/image.png --loc_model_path=path/to/loc_model.pt
+    python src/inference.py --user_input yes
     ```
 
-### Custom User Data Format
-The `inference.py` script expects the following format for custom user data:
-
-- YOLO model weight file: The weight file should be in the Darknet format (`.pt` file).
-- Image file: The script supports various image formats, including JPEG, PNG, and BMP.
-- Localization model weight file: The weight file should be in a compatible format for the localization model.
-
-Make sure to provide the correct paths to the respective files when using custom user data.
-
 **Note:** If the `--user_input` flag is set to `yes`, the script will prompt you to enter the paths to the YOLO model weight file, image file, and localization model weight file interactively.
 
-## Usage train.py
+# Usage train.py
 The `train.py` script is used to train a specified model based on user inputs. It provides options to train either a YOLO model, a localization model, or both. This document explains how to use the script and provides examples.
 
-### Prerequisites
-Before using the `train.py` script, ensure that you have the following dependencies installed:
+## Train Script Prerequisites
 
-- Python 3.x
-- argparse module
+Before using the `train.py` script, make sure you have the following prerequisites:
 
-### Running the Script
-To run the script, execute the following command in your terminal:
+### YOLO Model Training:
+- Prepare the training dataset with annotated bounding box labels. The dataset can be created using tools like Roboflow.
+- You should have the API codes ready to put into the CLI
+  
+### Localization Model Training:
+- Prepare the training dataset as follows:
+  .NPZ file(s) with 3 Numpy arrays named arr_0 - arr_1 - arr_2.
+  - arr_0 should contain image arrays with the following shape: (amount_items, 92, 138, 3)
+  - arr_1 should contain the X for the model with the following columns:
+    - column1: Boundingbox Xmin
+    - column2: Boundingbox Xmax
+    - column3: Boundingbox Ymin
+    - column4: Boundingbox Ymax
+    - column5: Classes from 0 to 4 (max 5 different classes allowed)
+  - arr_2 should contain the Y for the model with the following columns:
+    - column1: X Location of the item between -0,1 and 0,1
+    - column2: Y Location of the item between -0,1 and 0,1
+    - column3: Z Location of the item between -0,1 and 0,1
+    - column4: Yaw of the items between -0,1 and 0,1
+      
+**!Important Note:** The number of pictures should match the number of items. So for example, if your image has 3 items, you should have 3 rows of the same image in the image array. So the row index corresponds with the items' X and Y indexes. 
 
-```shell
-python train.py
-```
+**Note:** The module will normalize and process all of the data as long as the above structure is being used.
 
-### Command-line Arguments
-The `train.py` script accepts the following command-line arguments:
+## Running the Script
+To run the script, execute the following command in your terminal. Options can be inputted interactively:
 
-- `--model`: Specifies the model to train. It accepts two options: 'yolo' or 'loc'. This argument is optional.
-- `--user_input`: Allows the user to change the default settings. It accepts a string value ('yes' or 'no'). This argument is optional.
+```
+python train.py
+```
+The script will prompt you to enter the model and user input interactively to change the default settings.
 
-If no command-line arguments are provided, the script will prompt you to enter the model and user input interactively.
+## Interactive Command-line Options
+Settings that can be changed for the **Yolo** model is or press ENTER for default options:
+- api_key: Roboflow API Key for RoboFlow Project
+- workspace_name: Workspace name from RoboFlow Project
+- project_name: Project name from RoboFlow Project
+- version_number: Version Number from RoboFlow Project
+- model_weight: Pre-trained weights file
+- model_path: Option to change pre-trained file
+- img_size: Image Size
+- batch_size: Batch Size
+- epochs: Epochs
+  
+Settings that can be changed for the **Localization** model is or press ENTER for default options:
+- data_path:  The path to the MAP where the dataset(s) are located
+- batch_size: Batch Size
+- epoch_size: Epochs
+- loc_model_path_save: Name of created weights file, file saved in 'data/object_loc_weights/' folder
 
-### Examples
+## Examples
 Here are some examples of how to use the `train.py` script:
 
-1. Train a YOLO model with default settings:
+Train a YOLO model:
 
 ```shell
-python train.py --model yolo
+python src/train.py
 ```
 
-2. Train a localization model with custom settings:
-
-```shell
-python train.py --model loc --user_input yes
-```
-
-3. Train both YOLO and localization models with default settings:
-
-```shell
-python train.py --model both
-```
 
-### Custom User Data Format
-The `train.py` script does not require any custom user data format. It uses the specified model and user input to determine the training process. However, make sure to provide the required data files or directories as per the model's requirements, such as training images, annotations, or configuration files. Refer to the specific model's documentation for more information on the expected data format.
```

