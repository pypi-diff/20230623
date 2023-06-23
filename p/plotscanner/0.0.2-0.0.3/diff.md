# Comparing `tmp/plotscanner-0.0.2.tar.gz` & `tmp/plotscanner-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotscanner-0.0.2.tar", last modified: Fri Jun 23 15:19:22 2023, max compression
+gzip compressed data, was "plotscanner-0.0.3.tar", last modified: Fri Jun 23 15:37:05 2023, max compression
```

## Comparing `plotscanner-0.0.2.tar` & `plotscanner-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 15:19:22.683861 plotscanner-0.0.2/
--rw-rw-rw-   0        0        0     1605 2023-06-23 15:19:22.683861 plotscanner-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2023-06-23 15:16:37.000000 plotscanner-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 15:19:22.596189 plotscanner-0.0.2/plotscanner/
--rw-rw-rw-   0        0        0    12881 2023-06-23 13:44:11.000000 plotscanner-0.0.2/plotscanner/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-23 10:14:26.000000 plotscanner-0.0.2/plotscanner/__init__.py
--rw-rw-rw-   0        0        0     2897 2023-06-23 13:42:29.000000 plotscanner-0.0.2/plotscanner/data_frame_table.py
--rw-rw-rw-   0        0        0     3165 2023-06-21 12:51:20.000000 plotscanner-0.0.2/plotscanner/geometry.py
--rw-rw-rw-   0        0        0     3418 2023-06-22 06:35:06.000000 plotscanner-0.0.2/plotscanner/grid.py
--rw-rw-rw-   0        0        0    11361 2023-06-22 13:34:43.000000 plotscanner-0.0.2/plotscanner/plotdigitizer.py
--rw-rw-rw-   0        0        0     3517 2023-06-21 12:51:20.000000 plotscanner-0.0.2/plotscanner/trajectory.py
--rw-rw-rw-   0        0        0    11252 2023-06-23 13:43:16.000000 plotscanner-0.0.2/plotscanner/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-23 15:19:22.682863 plotscanner-0.0.2/plotscanner.egg-info/
--rw-rw-rw-   0        0        0     1605 2023-06-23 15:19:21.000000 plotscanner-0.0.2/plotscanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-06-23 15:19:22.000000 plotscanner-0.0.2/plotscanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 15:19:21.000000 plotscanner-0.0.2/plotscanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-23 15:19:21.000000 plotscanner-0.0.2/plotscanner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 15:19:21.000000 plotscanner-0.0.2/plotscanner.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      109 2023-06-23 15:19:21.000000 plotscanner-0.0.2/plotscanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-23 15:19:21.000000 plotscanner-0.0.2/plotscanner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 15:19:22.684868 plotscanner-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      957 2023-06-23 15:17:18.000000 plotscanner-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:37:05.265301 plotscanner-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-23 15:37:05.265301 plotscanner-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-23 15:36:48.000000 plotscanner-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:37:05.265301 plotscanner-0.0.3/plotscanner/
+-rw-r--r--   0 runner    (1001) docker     (123)    12524 2023-06-23 15:36:48.000000 plotscanner-0.0.3/plotscanner/GUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:36:48.000000 plotscanner-0.0.3/plotscanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-23 15:36:48.000000 plotscanner-0.0.3/plotscanner/data_frame_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-23 15:36:48.000000 plotscanner-0.0.3/plotscanner/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-23 15:36:48.000000 plotscanner-0.0.3/plotscanner/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-06-23 15:36:48.000000 plotscanner-0.0.3/plotscanner/plotdigitizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:37:05.265301 plotscanner-0.0.3/plotscanner/readme_imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)    47773 2023-06-23 15:36:48.000000 plotscanner-0.0.3/plotscanner/readme_imgs/example.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-23 15:36:48.000000 plotscanner-0.0.3/plotscanner/trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:37:05.265301 plotscanner-0.0.3/plotscanner/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-23 15:36:48.000000 plotscanner-0.0.3/plotscanner/ui/buttons.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-23 15:36:48.000000 plotscanner-0.0.3/plotscanner/ui/plots.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-06-23 15:36:48.000000 plotscanner-0.0.3/plotscanner/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:37:05.265301 plotscanner-0.0.3/plotscanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-23 15:37:05.000000 plotscanner-0.0.3/plotscanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-23 15:37:05.000000 plotscanner-0.0.3/plotscanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:37:05.000000 plotscanner-0.0.3/plotscanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 15:37:05.000000 plotscanner-0.0.3/plotscanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:37:05.000000 plotscanner-0.0.3/plotscanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-23 15:37:05.000000 plotscanner-0.0.3/plotscanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 15:37:05.000000 plotscanner-0.0.3/plotscanner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:37:05.269301 plotscanner-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-23 15:36:48.000000 plotscanner-0.0.3/setup.py
```

### Comparing `plotscanner-0.0.2/PKG-INFO` & `plotscanner-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-Metadata-Version: 2.1
-Name: plotscanner
-Version: 0.0.2
-Summary: The application for digitizing images of plots.
-Home-page: https://github.com/IlS0/Plot-digitization
-Author-email: silru@internet.ru
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-# Plotscanner
-
-A __Python3__ application used to convert images of functional data plots to digital format.
-Often data is presented in documents or scientific articles in the form of figures. In order to use this data, it must be digitized in some way. This program allows you to get a scanned image of a plot in _JPEG_ or _PNG_ format and quickly digitize the values. The numbers can be saved to a file (_CSV_, _XLS_, _TXT_, etc.) and used.
-
-## Documentation 
-You can find the documentation for all of the application's basic modules [here](https://github.com/IlS0/Plot-digitization/tree/main/docs/plotscanner).
-
-## Installation
-`$ pip install plotscanner`
-
-
-### Docker-image
-
-You can download a docker-image of the application if you want to use the back-end part in the container 
-`$ docker pull ils0/plotscanner`
-
-or build it yourself with the following command:
-
-`$ docker build -t plotscanner .`
-
-
-## Run
-Start the application by running the command in the terminal:
-`$ plotscanner`
-
-Follow the instructions in the app window to work correctly.
-### Image preparing
-Plotscanner requires the input data in the correct form to work right. Before loading the image, crop it and save only the axes and lines of the plot like this.
-![Example image](./plotscanner/readme_imgs/example.jpg)
-
-
+Metadata-Version: 2.1
+Name: plotscanner
+Version: 0.0.3
+Summary: The application for digitizing images of plots.
+Home-page: https://github.com/IlS0/Plot-digitization
+Author-email: silru@internet.ru
+Description-Content-Type: text/markdown
+
+# Plotscanner
+
+A __Python3__ application used to convert images of functional data plots to digital format.
+Often data is presented in documents or scientific articles in the form of figures. In order to use this data, it must be digitized in some way. This program allows you to get a scanned image of a plot in _JPEG_ or _PNG_ format and quickly digitize the values. The numbers can be saved to a file (_CSV_, _XLS_, _TXT_, etc.) and used.
+
+## Documentation 
+You can find the documentation for all of the application's basic modules [here](https://github.com/IlS0/Plot-digitization/tree/main/docs/plotscanner).
+
+## Installation
+`$ pip install plotscanner`
+
+
+### Docker-image
+
+You can download a docker-image of the application if you want to use the back-end part in the container
+
+`$ docker pull ils0/plotscanner`
+
+or build it yourself with the following command:
+
+`$ docker build -t plotscanner .`
+
+
+## Run
+Start the application by running the command in the terminal:
+`$ plotscanner`
+
+Follow the instructions in the app window to work correctly.
+### Image preparing
+Plotscanner requires the input data in the correct form to work right. Before loading the image, crop it and save only the axes and lines of the plot like this.
+![Example image](./plotscanner/readme_imgs/example.jpg)
```

### Comparing `plotscanner-0.0.2/README.md` & `plotscanner-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# Plotscanner
-
-A __Python3__ application used to convert images of functional data plots to digital format.
-Often data is presented in documents or scientific articles in the form of figures. In order to use this data, it must be digitized in some way. This program allows you to get a scanned image of a plot in _JPEG_ or _PNG_ format and quickly digitize the values. The numbers can be saved to a file (_CSV_, _XLS_, _TXT_, etc.) and used.
-
-## Documentation 
-You can find the documentation for all of the application's basic modules [here](https://github.com/IlS0/Plot-digitization/tree/main/docs/plotscanner).
-
-## Installation
-`$ pip install plotscanner`
-
-
-### Docker-image
-
-You can download a docker-image of the application if you want to use the back-end part in the container 
-`$ docker pull ils0/plotscanner`
-
-or build it yourself with the following command:
-
-`$ docker build -t plotscanner .`
-
-
-## Run
-Start the application by running the command in the terminal:
-`$ plotscanner`
-
-Follow the instructions in the app window to work correctly.
-### Image preparing
-Plotscanner requires the input data in the correct form to work right. Before loading the image, crop it and save only the axes and lines of the plot like this.
-![Example image](./plotscanner/readme_imgs/example.jpg)
+# Plotscanner
+
+A __Python3__ application used to convert images of functional data plots to digital format.
+Often data is presented in documents or scientific articles in the form of figures. In order to use this data, it must be digitized in some way. This program allows you to get a scanned image of a plot in _JPEG_ or _PNG_ format and quickly digitize the values. The numbers can be saved to a file (_CSV_, _XLS_, _TXT_, etc.) and used.
+
+## Documentation 
+You can find the documentation for all of the application's basic modules [here](https://github.com/IlS0/Plot-digitization/tree/main/docs/plotscanner).
+
+## Installation
+`$ pip install plotscanner`
+
+
+### Docker-image
+
+You can download a docker-image of the application if you want to use the back-end part in the container
+
+`$ docker pull ils0/plotscanner`
+
+or build it yourself with the following command:
+
+`$ docker build -t plotscanner .`
+
+
+## Run
+Start the application by running the command in the terminal:
+`$ plotscanner`
+
+Follow the instructions in the app window to work correctly.
+### Image preparing
+Plotscanner requires the input data in the correct form to work right. Before loading the image, crop it and save only the axes and lines of the plot like this.
+![Example image](./plotscanner/readme_imgs/example.jpg)
```

### Comparing `plotscanner-0.0.2/plotscanner/GUI.py` & `plotscanner-0.0.3/plotscanner/GUI.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,357 +1,357 @@
-import os
-import subprocess
-import sys
-
-import numpy as np
-import pandas as pd
-
-from PyQt5 import QtCore, uic
-from PyQt5.QtWidgets import (QApplication, QFileDialog, QHBoxLayout,
-                             QHeaderView, QMainWindow, QMessageBox,
-                             QPushButton, QSlider, QVBoxLayout, QWidget)
-
-
-from .data_frame_table import DataFrameTable
-from .widgets import Magnifier, PlotCanvas, ImageCanvas
-
-path = os.path.abspath(os.path.dirname(__file__))
-
-
-def start_digitizer(df, path_to_image):
-    """
-    Starts the digitization process.
-
-    Args:
-        df (pandas.DataFrame): A DataFrame containing the locations and points to be digitized.
-        path_to_image (str): The path to the image to be digitized.
-
-    Returns:
-        int: The return code of the subprocess call.
-    """
-    locations = list(df.apply(lambda row: (
-        row['Y Image'], row['X Image']), axis=1))
-    points = list(df.apply(lambda row: (row['Y Plot'], row['X Plot']), axis=1))
-    script_path = "plotdigitizer.py"
-    script_path = os.path.join(path, script_path)
-    pts = " ".join([f"-p {','.join(map(str,pt))}" for pt in points])
-    locs = " ".join([f"-l {','.join(map(str,pt))}" for pt in locations])
-    cmd = "python \"" + script_path + "\" \"" + path_to_image + "\" " + f"{pts} {locs}"
-
-    returncode = subprocess.call(cmd)
-
-    if returncode != 0:
-        # Error handling
-        print(f"Error when running command: return code {returncode}")
-
-    return returncode
-
-
-def replace_placeholder(
-        parent,
-        widget_new,
-        placeholder_name,
-        fixed_size=False):
-    """
-    Replaces a placeholder widget with a new widget in the window.
-
-    Args:
-        parent (QWidget): The widget in which the replacement is performed.
-        widget_new (QWidget): The new widget for replacement.
-        placeholder_name (str): The name of the placeholder widget to be replaced.
-        fixed_size (bool): Flag to set a fixed size for the new widget.
-
-    Returns:
-        None
-    """
-    # Find the old widget by name
-    widget_old = parent.findChild(QWidget, placeholder_name)
-    # Get the parent layout for the old widget
-    containingLayout = widget_old.parent().layout()
-    # Replace the old widget with the new one in the layout
-    containingLayout.replaceWidget(widget_old, widget_new)
-
-    # Save sizes
-    # Save minimum size for new widget
-    widget_new.setMinimumSize(widget_old.minimumSize())
-
-    # Set fixed size for new widget
-    if fixed_size:
-        widget_new.setFixedSize(widget_old.size())
-
-
-def sort_lists(x, y):
-    """
-    Sorts two lists (x and y) in ascending order of values in the x list.
-
-    Args:
-        x (list): The list of values to be sorted.
-        y (list): The list of values corresponding to the values in the x list.
-
-    Returns:
-        tuple: A tuple of two sorted lists (x_sorted, y_sorted).
-    """
-    # Create a list of pairs (x, y)
-    xy_pairs = list(zip(x, y))
-    # Sort the list of pairs by the value of x
-    xy_pairs.sort(key=lambda pair: pair[0])
-    # Split the sorted pairs back into two lists
-    x_sorted, y_sorted = zip(*xy_pairs)
-    return list(x_sorted), list(y_sorted)
-
-
-class ButtonsWidget(QWidget):
-    """
-    Виджет кнопок, в нём находятся: текстовая подсказка, magnifier, slider, buttons
-    """
-
-    def __init__(self):
-        QWidget.__init__(self)
-        # Загрузка дизайна виджета из файла
-        uic.loadUi(os.path.join(path, "ui", "buttons.ui"), self)
-
-
-class GraphPreviewer(QWidget):
-    """
-    Chart view widget containing 2 windows: the left one shows the original image,
-    the right one shows the graph plotted from points.
-    """
-
-    def __init__(self):
-        QWidget.__init__(self)
-        # Load the widget design from a file
-        uic.loadUi(os.path.join(path, "ui", "plots.ui"), self)
-
-
-class MainWindow(QMainWindow):
-    """
-    The main window of the application.
-    """
-
-    def __init__(self):
-        QMainWindow.__init__(self)
-        self.setWindowTitle("Plot Scanner")
-        # Horizontal layout: buttons and table on the left, graphs on the right
-        hbox = QHBoxLayout()
-        # Freeze the left layout with buttons so it doesn't stretch
-        hbox.setStretch(1, 2)
-        # Vertical layout: buttons on top, points table at the bottom
-        vbox = QVBoxLayout()
-        hbox.addLayout(vbox)
-
-        buttons = ButtonsWidget()
-        graph = GraphPreviewer()
-        vbox.addWidget(buttons)
-        hbox.addWidget(graph)
-
-        # Central widget for the main window
-        cw = QWidget()
-        cw.setLayout(hbox)
-        self.setCentralWidget(cw)
-
-        # Find buttons created in designer
-        self.button_load = buttons.findChild(QPushButton, "loadButton")
-        self.button_create = buttons.findChild(QPushButton, "createButton")
-        self.button_save = buttons.findChild(QPushButton, "saveButton")
-        # Find magnifier scale slider
-        self.scale_slider = buttons.findChild(QSlider, "scaleSlider")
-
-        # Click handlers
-        self.button_load.clicked.connect(self.load_plot_image)
-        self.button_save.clicked.connect(self.save_points)
-        self.button_create.clicked.connect(self.create_plot)
-
-        # Canvases for displaying images directly in the application window
-        self.origImCanvas = ImageCanvas(self)
-        self.readyPlotCanvas = PlotCanvas()
-        self.magnifierImCanvas = Magnifier(self)
-
-        # Create a table with 4 columns
-        self.table = DataFrameTable()
-        self.table.setColumnCount(4)
-        self.table.setHorizontalHeaderLabels(
-            ['X Image', 'Y Image', 'X Plot', 'Y Plot'])
-        # Set column resize mode to Stretch
-        self.table.horizontalHeader().setSectionResizeMode(QHeaderView.Stretch)
-        vbox.addWidget(self.table)
-
-        self.table.cellClicked.connect(self.on_cell_clicked)
-
-        # Replace placeholders with image output widgets
-        replace_placeholder(self, self.origImCanvas, "origWidget")
-        replace_placeholder(self, self.readyPlotCanvas, "plotWidget")
-        replace_placeholder(buttons, self.magnifierImCanvas,
-                            "magnifierWidget", fixed_size=True)
-
-        # Connect mouse wheel to magnifier scale change
-        self.scale_slider.valueChanged.connect(
-            lambda value: self.on_value_changed(value))
-
-        self.selected_row = None
-
-    def resizeEvent(self, event):
-        """
-        Handles window size changes (need to recalculate coefficients).
-        """
-        # Check for image presence in canvas
-        if self.origImCanvas.img is not None:
-            self.origImCanvas.count_koeffs()
-
-    def on_value_changed(self, value):
-        """
-        Handles changes in slider value (change magnifier scale).
-        """
-        # Check for image presence in canvas
-        if self.origImCanvas.img is not None:
-            self.origImCanvas.add_padding(value)
-            # Recalculate coefficients
-            self.origImCanvas.count_koeffs()
-            self.magnifierImCanvas.update_magnifier_point()
-
-            self.magnifierImCanvas.update_canvas()
-
-    def load_plot_image(self):
-        """
-        Prompts the user to select an image in the file explorer.
-        Loads and displays the selected image.
-        """
-        fname = QFileDialog.getOpenFileName(
-            self, 'Open file', path, "Image files (*.jpg *.png)")
-        # Cancelled - do nothing
-        if fname[0] == '':
-            return
-        self.path_to_image = fname[0]
-        # Display image on canvas
-        self.origImCanvas.show_user_image(fname)
-        # Update magnifier
-        self.magnifierImCanvas.update_magnifier_point()
-        self.origImCanvas.mouseMoved(0, 0)
-        # New image - old points not needed
-        self.table.clear_table()
-        self.selected_row = None
-        self.readyPlotCanvas.points = []
-
-    # Table row selected - highlight point
-    def on_cell_clicked(self, row, column):
-        """
-        Handles clicking on a table cell.
-        Changes the color of the selected point to red.
-        Changes the previous point back to blue.
-        """
-        if self.selected_row is not None:
-            self.origImCanvas.points[self.selected_row].set_facecolor('blue')
-        self.origImCanvas.points[row].set_facecolor('red')
-        self.selected_row = row
-        self.origImCanvas.update_canvas()
-
-    def eventFilter(self, source, event):
-        """
-        Filters events to handle key presses on the table.
-
-        Args:
-            source (QObject): The object that generated the event.
-            event (QEvent): The event to be filtered.
-
-        Returns:
-            bool: Whether the event was handled.
-        """
-        if (source is self.table and event.type() == QtCore.QEvent.KeyPress):
-            row = self.table.currentRow()
-            col = self.table.currentColumn()
-            if event.key() == QtCore.Qt.Key_Up:
-                if row - 1 >= 0:
-                    self.on_cell_clicked(row - 1, None)
-            elif event.key() == QtCore.Qt.Key_Down:
-                if (row + 1) < len(self.origImCanvas.points):
-                    self.on_cell_clicked(row + 1, None)
-            if event.key() == QtCore.Qt.Key_Tab:
-                if col == 3 and (row + 1) < len(self.origImCanvas.points):
-                    self.on_cell_clicked(row + 1, None)
-                if col == 0:
-                    self.on_cell_clicked(row, None)
-        return super().eventFilter(source, event)
-
-    def save_points(self):
-        """
-        Prompts the user for the path and extension of the output file and writes the points to it.
-        """
-        # Check for image presence in canvas
-        if self.origImCanvas.img is None:
-            widget = QWidget()
-            QMessageBox.warning(
-                widget,
-                "Attention",
-                "Points have not been calculated yet")
-            return
-        file_name, file_type = QFileDialog.getSaveFileName(
-            self,
-            'Save File',
-            '',
-            'CSV(*.csv);;Excel(*.xlsx);;TSV(*.tsv);;JSON(*.json);;XML(*.xml);;DAT(*.dat);;TXT(*.txt)'
-        )
-        if file_name:
-            df = self.readyPlotCanvas.points
-            # Spaces are not supported in some formats
-            df.columns = [col.replace(' ', '_') for col in df.columns]
-            if 'CSV' in file_type:
-                df.to_csv(file_name, index=False)
-            elif 'Excel' in file_type:
-                df.to_excel(file_name, index=False)
-            elif 'TSV' in file_type:
-                df.to_csv(file_name, index=False, sep='\t')
-            elif 'TXT' in file_type:
-                df.to_csv(file_name, index=False, sep='\t')
-            elif 'DAT' in file_type:
-                df.to_csv(file_name, index=False, sep=' ')
-            elif 'JSON' in file_type:
-                df.to_json(file_name)
-            elif 'XML' in file_type:
-                df.to_xml(file_name)
-
-    def create_plot(self):
-        """
-        Calculates the points of the new graph and plots it.
-        """
-        # Check for image presence in canvas
-        if self.origImCanvas.img is None:
-            return
-        # Copy table from GUI to DataFrame
-        df = self.table.save_to_df()
-
-        # Start digitization
-        returncode = start_digitizer(df, self.path_to_image)
-        if returncode != 0:
-            msg = QMessageBox()
-            msg.setIcon(QMessageBox.Critical)
-            msg.setText(f"Ошибка {str(returncode)}")
-            msg.setInformativeText("Оцифровка не удалась, пожалуйста, "
-                                   "проверьте првильность ввода данных")
-            msg.setWindowTitle("Ошибка")
-            msg.exec_()
-            return
-        points = np.load('points.npy')
-        # Convert to lists
-        x, y = zip(*points)
-        x, y = sort_lists(x, y)
-        # Remove old plot
-        ax = self.readyPlotCanvas.figure.axes[0]
-        for line in ax.lines:
-            line.remove()
-        self.readyPlotCanvas.draw_plot(x, y)
-        self.readyPlotCanvas.points = pd.DataFrame({'X': x, 'Y': y})
-
-
-def main():
-    """
-    The main function that starts the application.
-    """
-    app = QApplication(sys.argv)
-    window = MainWindow()
-    window.resize(1280, 650)
-
-    window.show()
-    app.installEventFilter(window)
-    sys.exit(app.exec_())
-
-
-if __name__ == "__main__":
-    main()
+import os
+import subprocess
+import sys
+
+import numpy as np
+import pandas as pd
+
+from PyQt5 import QtCore, uic
+from PyQt5.QtWidgets import (QApplication, QFileDialog, QHBoxLayout,
+                             QHeaderView, QMainWindow, QMessageBox,
+                             QPushButton, QSlider, QVBoxLayout, QWidget)
+
+
+from .data_frame_table import DataFrameTable
+from .widgets import Magnifier, PlotCanvas, ImageCanvas
+
+path = os.path.abspath(os.path.dirname(__file__))
+
+
+def start_digitizer(df, path_to_image):
+    """
+    Starts the digitization process.
+
+    Args:
+        df (pandas.DataFrame): A DataFrame containing the locations and points to be digitized.
+        path_to_image (str): The path to the image to be digitized.
+
+    Returns:
+        int: The return code of the subprocess call.
+    """
+    locations = list(df.apply(lambda row: (
+        row['Y Image'], row['X Image']), axis=1))
+    points = list(df.apply(lambda row: (row['Y Plot'], row['X Plot']), axis=1))
+    script_path = "plotdigitizer.py"
+    script_path = os.path.join(path, script_path)
+    pts = " ".join([f"-p {','.join(map(str,pt))}" for pt in points])
+    locs = " ".join([f"-l {','.join(map(str,pt))}" for pt in locations])
+    cmd = "python \"" + script_path + "\" \"" + path_to_image + "\" " + f"{pts} {locs}"
+
+    returncode = subprocess.call(cmd)
+
+    if returncode != 0:
+        # Error handling
+        print(f"Error when running command: return code {returncode}")
+
+    return returncode
+
+
+def replace_placeholder(
+        parent,
+        widget_new,
+        placeholder_name,
+        fixed_size=False):
+    """
+    Replaces a placeholder widget with a new widget in the window.
+
+    Args:
+        parent (QWidget): The widget in which the replacement is performed.
+        widget_new (QWidget): The new widget for replacement.
+        placeholder_name (str): The name of the placeholder widget to be replaced.
+        fixed_size (bool): Flag to set a fixed size for the new widget.
+
+    Returns:
+        None
+    """
+    # Find the old widget by name
+    widget_old = parent.findChild(QWidget, placeholder_name)
+    # Get the parent layout for the old widget
+    containingLayout = widget_old.parent().layout()
+    # Replace the old widget with the new one in the layout
+    containingLayout.replaceWidget(widget_old, widget_new)
+
+    # Save sizes
+    # Save minimum size for new widget
+    widget_new.setMinimumSize(widget_old.minimumSize())
+
+    # Set fixed size for new widget
+    if fixed_size:
+        widget_new.setFixedSize(widget_old.size())
+
+
+def sort_lists(x, y):
+    """
+    Sorts two lists (x and y) in ascending order of values in the x list.
+
+    Args:
+        x (list): The list of values to be sorted.
+        y (list): The list of values corresponding to the values in the x list.
+
+    Returns:
+        tuple: A tuple of two sorted lists (x_sorted, y_sorted).
+    """
+    # Create a list of pairs (x, y)
+    xy_pairs = list(zip(x, y))
+    # Sort the list of pairs by the value of x
+    xy_pairs.sort(key=lambda pair: pair[0])
+    # Split the sorted pairs back into two lists
+    x_sorted, y_sorted = zip(*xy_pairs)
+    return list(x_sorted), list(y_sorted)
+
+
+class ButtonsWidget(QWidget):
+    """
+    Виджет кнопок, в нём находятся: текстовая подсказка, magnifier, slider, buttons
+    """
+
+    def __init__(self):
+        QWidget.__init__(self)
+        # Загрузка дизайна виджета из файла
+        uic.loadUi(os.path.join(path, "ui", "buttons.ui"), self)
+
+
+class GraphPreviewer(QWidget):
+    """
+    Chart view widget containing 2 windows: the left one shows the original image,
+    the right one shows the graph plotted from points.
+    """
+
+    def __init__(self):
+        QWidget.__init__(self)
+        # Load the widget design from a file
+        uic.loadUi(os.path.join(path, "ui", "plots.ui"), self)
+
+
+class MainWindow(QMainWindow):
+    """
+    The main window of the application.
+    """
+
+    def __init__(self):
+        QMainWindow.__init__(self)
+        self.setWindowTitle("Plot Scanner")
+        # Horizontal layout: buttons and table on the left, graphs on the right
+        hbox = QHBoxLayout()
+        # Freeze the left layout with buttons so it doesn't stretch
+        hbox.setStretch(1, 2)
+        # Vertical layout: buttons on top, points table at the bottom
+        vbox = QVBoxLayout()
+        hbox.addLayout(vbox)
+
+        buttons = ButtonsWidget()
+        graph = GraphPreviewer()
+        vbox.addWidget(buttons)
+        hbox.addWidget(graph)
+
+        # Central widget for the main window
+        cw = QWidget()
+        cw.setLayout(hbox)
+        self.setCentralWidget(cw)
+
+        # Find buttons created in designer
+        self.button_load = buttons.findChild(QPushButton, "loadButton")
+        self.button_create = buttons.findChild(QPushButton, "createButton")
+        self.button_save = buttons.findChild(QPushButton, "saveButton")
+        # Find magnifier scale slider
+        self.scale_slider = buttons.findChild(QSlider, "scaleSlider")
+
+        # Click handlers
+        self.button_load.clicked.connect(self.load_plot_image)
+        self.button_save.clicked.connect(self.save_points)
+        self.button_create.clicked.connect(self.create_plot)
+
+        # Canvases for displaying images directly in the application window
+        self.origImCanvas = ImageCanvas(self)
+        self.readyPlotCanvas = PlotCanvas()
+        self.magnifierImCanvas = Magnifier(self)
+
+        # Create a table with 4 columns
+        self.table = DataFrameTable()
+        self.table.setColumnCount(4)
+        self.table.setHorizontalHeaderLabels(
+            ['X Image', 'Y Image', 'X Plot', 'Y Plot'])
+        # Set column resize mode to Stretch
+        self.table.horizontalHeader().setSectionResizeMode(QHeaderView.Stretch)
+        vbox.addWidget(self.table)
+
+        self.table.cellClicked.connect(self.on_cell_clicked)
+
+        # Replace placeholders with image output widgets
+        replace_placeholder(self, self.origImCanvas, "origWidget")
+        replace_placeholder(self, self.readyPlotCanvas, "plotWidget")
+        replace_placeholder(buttons, self.magnifierImCanvas,
+                            "magnifierWidget", fixed_size=True)
+
+        # Connect mouse wheel to magnifier scale change
+        self.scale_slider.valueChanged.connect(
+            lambda value: self.on_value_changed(value))
+
+        self.selected_row = None
+
+    def resizeEvent(self, event):
+        """
+        Handles window size changes (need to recalculate coefficients).
+        """
+        # Check for image presence in canvas
+        if self.origImCanvas.img is not None:
+            self.origImCanvas.count_koeffs()
+
+    def on_value_changed(self, value):
+        """
+        Handles changes in slider value (change magnifier scale).
+        """
+        # Check for image presence in canvas
+        if self.origImCanvas.img is not None:
+            self.origImCanvas.add_padding(value)
+            # Recalculate coefficients
+            self.origImCanvas.count_koeffs()
+            self.magnifierImCanvas.update_magnifier_point()
+
+            self.magnifierImCanvas.update_canvas()
+
+    def load_plot_image(self):
+        """
+        Prompts the user to select an image in the file explorer.
+        Loads and displays the selected image.
+        """
+        fname = QFileDialog.getOpenFileName(
+            self, 'Open file', path, "Image files (*.jpg *.png)")
+        # Cancelled - do nothing
+        if fname[0] == '':
+            return
+        self.path_to_image = fname[0]
+        # Display image on canvas
+        self.origImCanvas.show_user_image(fname)
+        # Update magnifier
+        self.magnifierImCanvas.update_magnifier_point()
+        self.origImCanvas.mouseMoved(0, 0)
+        # New image - old points not needed
+        self.table.clear_table()
+        self.selected_row = None
+        self.readyPlotCanvas.points = []
+
+    # Table row selected - highlight point
+    def on_cell_clicked(self, row, column):
+        """
+        Handles clicking on a table cell.
+        Changes the color of the selected point to red.
+        Changes the previous point back to blue.
+        """
+        if self.selected_row is not None:
+            self.origImCanvas.points[self.selected_row].set_facecolor('blue')
+        self.origImCanvas.points[row].set_facecolor('red')
+        self.selected_row = row
+        self.origImCanvas.update_canvas()
+
+    def eventFilter(self, source, event):
+        """
+        Filters events to handle key presses on the table.
+
+        Args:
+            source (QObject): The object that generated the event.
+            event (QEvent): The event to be filtered.
+
+        Returns:
+            bool: Whether the event was handled.
+        """
+        if (source is self.table and event.type() == QtCore.QEvent.KeyPress):
+            row = self.table.currentRow()
+            col = self.table.currentColumn()
+            if event.key() == QtCore.Qt.Key_Up:
+                if row - 1 >= 0:
+                    self.on_cell_clicked(row - 1, None)
+            elif event.key() == QtCore.Qt.Key_Down:
+                if (row + 1) < len(self.origImCanvas.points):
+                    self.on_cell_clicked(row + 1, None)
+            if event.key() == QtCore.Qt.Key_Tab:
+                if col == 3 and (row + 1) < len(self.origImCanvas.points):
+                    self.on_cell_clicked(row + 1, None)
+                if col == 0:
+                    self.on_cell_clicked(row, None)
+        return super().eventFilter(source, event)
+
+    def save_points(self):
+        """
+        Prompts the user for the path and extension of the output file and writes the points to it.
+        """
+        # Check for image presence in canvas
+        if self.origImCanvas.img is None:
+            widget = QWidget()
+            QMessageBox.warning(
+                widget,
+                "Attention",
+                "Points have not been calculated yet")
+            return
+        file_name, file_type = QFileDialog.getSaveFileName(
+            self,
+            'Save File',
+            '',
+            'CSV(*.csv);;Excel(*.xlsx);;TSV(*.tsv);;JSON(*.json);;XML(*.xml);;DAT(*.dat);;TXT(*.txt)'
+        )
+        if file_name:
+            df = self.readyPlotCanvas.points
+            # Spaces are not supported in some formats
+            df.columns = [col.replace(' ', '_') for col in df.columns]
+            if 'CSV' in file_type:
+                df.to_csv(file_name, index=False)
+            elif 'Excel' in file_type:
+                df.to_excel(file_name, index=False)
+            elif 'TSV' in file_type:
+                df.to_csv(file_name, index=False, sep='\t')
+            elif 'TXT' in file_type:
+                df.to_csv(file_name, index=False, sep='\t')
+            elif 'DAT' in file_type:
+                df.to_csv(file_name, index=False, sep=' ')
+            elif 'JSON' in file_type:
+                df.to_json(file_name)
+            elif 'XML' in file_type:
+                df.to_xml(file_name)
+
+    def create_plot(self):
+        """
+        Calculates the points of the new graph and plots it.
+        """
+        # Check for image presence in canvas
+        if self.origImCanvas.img is None:
+            return
+        # Copy table from GUI to DataFrame
+        df = self.table.save_to_df()
+
+        # Start digitization
+        returncode = start_digitizer(df, self.path_to_image)
+        if returncode != 0:
+            msg = QMessageBox()
+            msg.setIcon(QMessageBox.Critical)
+            msg.setText(f"Ошибка {str(returncode)}")
+            msg.setInformativeText("Оцифровка не удалась, пожалуйста, "
+                                   "проверьте првильность ввода данных")
+            msg.setWindowTitle("Ошибка")
+            msg.exec_()
+            return
+        points = np.load('points.npy')
+        # Convert to lists
+        x, y = zip(*points)
+        x, y = sort_lists(x, y)
+        # Remove old plot
+        ax = self.readyPlotCanvas.figure.axes[0]
+        for line in ax.lines:
+            line.remove()
+        self.readyPlotCanvas.draw_plot(x, y)
+        self.readyPlotCanvas.points = pd.DataFrame({'X': x, 'Y': y})
+
+
+def main():
+    """
+    The main function that starts the application.
+    """
+    app = QApplication(sys.argv)
+    window = MainWindow()
+    window.resize(1280, 650)
+
+    window.show()
+    app.installEventFilter(window)
+    sys.exit(app.exec_())
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `plotscanner-0.0.2/plotscanner/data_frame_table.py` & `plotscanner-0.0.3/plotscanner/data_frame_table.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-import pandas as pd
-from PyQt5.QtCore import Qt
-from PyQt5.QtWidgets import QTableWidget, QTableWidgetItem
-
-
-class DataFrameTable(QTableWidget):
-    """
-    A QTableWidget that can be used to display and edit data in a DataFrame.
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def edit_lock(self, colum_count):
-        """
-        Prevents editing of the first `colum_count` columns.
-
-        Args:
-            colum_count (int): The number of columns to lock.
-        """
-        # Prevent editing of the first `colum_count` columns
-        for row in range(self.rowCount()):
-            for col in range(colum_count):
-                item = self.item(row, col)
-                item.setFlags(item.flags() & ~Qt.ItemIsEditable)
-
-    def save_to_df(self):
-        """
-        Saves the data in the table to a DataFrame.
-
-        Returns:
-            DataFrame: The DataFrame containing the data from the table.
-        """
-        # Get table dimensions
-        rows = self.rowCount()
-        cols = self.columnCount()
-
-        # Create an empty list to store data
-        data = []
-
-        # Extract data from table
-        for row in range(rows):
-            row_data = []
-            for col in range(cols):
-                item = self.item(row, col)
-                if item is not None:
-                    row_data.append(item.text())
-                else:
-                    row_data.append('')
-            data.append(row_data)
-
-        # Create a DataFrame with data from the table
-        df = pd.DataFrame(data, columns=[self.horizontalHeaderItem(
-            col).text() for col in range(cols)])
-        return df
-
-    def add_row(self, x, y):
-        """
-        Adds a row to the table.
-
-        Args:
-            x (int): The value to be added to the first column of the new row.
-            y (int): The value to be added to the second column of the new row.
-        """
-        # Add a row to the table
-        row_position = self.rowCount()
-        self.insertRow(row_position)
-        self.setItem(row_position, 0, QTableWidgetItem(str(x)))
-        self.setItem(row_position, 1, QTableWidgetItem(str(y)))
-        self.setItem(row_position, 2, QTableWidgetItem("0"))
-        self.setItem(row_position, 3, QTableWidgetItem("0"))
-        # Prevent editing of the first two columns
-        self.edit_lock(2)
-
-    def remove_row(self, index):
-        """
-        Removes a row from the table.
-
-        Args:
-            index (int): The index of the row to be removed.
-        """
-        # Remove a row by index
-        self.removeRow(index)
-
-    def clear_table(self):
-        """
-        Removes all rows from the table.
-        """
-        # Remove all rows from the table
-        while self.rowCount() > 0:
-            self.removeRow(0)
+import pandas as pd
+from PyQt5.QtCore import Qt
+from PyQt5.QtWidgets import QTableWidget, QTableWidgetItem
+
+
+class DataFrameTable(QTableWidget):
+    """
+    A QTableWidget that can be used to display and edit data in a DataFrame.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def edit_lock(self, colum_count):
+        """
+        Prevents editing of the first `colum_count` columns.
+
+        Args:
+            colum_count (int): The number of columns to lock.
+        """
+        # Prevent editing of the first `colum_count` columns
+        for row in range(self.rowCount()):
+            for col in range(colum_count):
+                item = self.item(row, col)
+                item.setFlags(item.flags() & ~Qt.ItemIsEditable)
+
+    def save_to_df(self):
+        """
+        Saves the data in the table to a DataFrame.
+
+        Returns:
+            DataFrame: The DataFrame containing the data from the table.
+        """
+        # Get table dimensions
+        rows = self.rowCount()
+        cols = self.columnCount()
+
+        # Create an empty list to store data
+        data = []
+
+        # Extract data from table
+        for row in range(rows):
+            row_data = []
+            for col in range(cols):
+                item = self.item(row, col)
+                if item is not None:
+                    row_data.append(item.text())
+                else:
+                    row_data.append('')
+            data.append(row_data)
+
+        # Create a DataFrame with data from the table
+        df = pd.DataFrame(data, columns=[self.horizontalHeaderItem(
+            col).text() for col in range(cols)])
+        return df
+
+    def add_row(self, x, y):
+        """
+        Adds a row to the table.
+
+        Args:
+            x (int): The value to be added to the first column of the new row.
+            y (int): The value to be added to the second column of the new row.
+        """
+        # Add a row to the table
+        row_position = self.rowCount()
+        self.insertRow(row_position)
+        self.setItem(row_position, 0, QTableWidgetItem(str(x)))
+        self.setItem(row_position, 1, QTableWidgetItem(str(y)))
+        self.setItem(row_position, 2, QTableWidgetItem("0"))
+        self.setItem(row_position, 3, QTableWidgetItem("0"))
+        # Prevent editing of the first two columns
+        self.edit_lock(2)
+
+    def remove_row(self, index):
+        """
+        Removes a row from the table.
+
+        Args:
+            index (int): The index of the row to be removed.
+        """
+        # Remove a row by index
+        self.removeRow(index)
+
+    def clear_table(self):
+        """
+        Removes all rows from the table.
+        """
+        # Remove all rows from the table
+        while self.rowCount() > 0:
+            self.removeRow(0)
```

### Comparing `plotscanner-0.0.2/plotscanner/geometry.py` & `plotscanner-0.0.3/plotscanner/geometry.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import typing as T
-import statistics
-import math
-
-
-class Point:
-    """A point in 2D space."""
-
-    def __init__(self, x, y):
-        """
-        Initialize a point.
-
-        Args:
-            x: A float representing the x-coordinate of the point.
-            y: A float representing the y-coordinate of the point.
-
-        Returns:
-            None.
-        """
-        self.x = int(x)
-        self.y = int(y)
-
-    @classmethod
-    def fromCSV(cls, csv: str) -> "Point":
-        xy = [float(x) for x in csv.split(",")]
-        return cls(xy[0], xy[1])
-
-    def __eq__(self, other) -> bool:
-        """
-        Check if two points are equal.
-
-        Args:
-            other: An object representing the other point.
-
-        Returns:
-            A boolean indicating whether the two points are equal.
-        """
-        return (self.x == other.x) and (self.y == other.y)
-
-    def __hash__(self):
-        """
-    Compute origin of given points.
-
-    Args:
-        pts: A list of Point objects representing the points.
-
-    Returns:
-        A Point object representing the origin of the points.
-    """
-        return hash((self.x, self.y))
-
-    def __repr__(self):
-        """
-        Return a string representation of the point.
-
-        Args:
-            None.
-
-        Returns:
-            A string representation of the point.
-        """
-        return f"({self.x}, {self.y})"
-
-    def __iter__(self):
-        """
-        Return an iterator over the coordinates of the point.
-
-        Args:
-            None.
-
-        Returns:
-            An iterator over the coordinates of the point.
-        """
-        return iter((self.x, self.y))
-
-
-def find_origin(pts: T.List[Point]) -> Point:
-    """
-    Compute origin of given points.
-
-    Args:
-        pts: A list of Point objects representing the points.
-
-    Returns:
-        A Point object representing the origin of the points.
-    """
-    horizontal = set()
-    for i, p1 in enumerate(pts):
-        for _, p2 in enumerate(pts[i + 1:]):
-            if abs(p1.x - p2.x) <= 2:
-                continue
-            m = (p2.y - p1.y) / (p2.x - p1.x)
-            if abs(m) < math.tan(math.pi / 180 * 5):  # <5 deg is horizontal.
-                horizontal.add(p1)
-                horizontal.add(p2)
-
-    points = set(pts)
-    assert len(horizontal) > 1, f"Must have at least two colinear points {horizontal}"
-    verticals = points - horizontal
-    assert len(verticals) > 0, "Must be at least one vertical point"
-    originY = statistics.mean([p.y for p in horizontal])
-    originX = statistics.mean([p.x for p in verticals])
-    return Point(originX, originY)
-
-
-def test_origin():
-    pts = [Point(81, 69), Point(1779, 68), Point(81, 449)]
-    p = find_origin(pts)
-    assert p == Point(81, 68), p == Point(81, 68)
-
-    pts = [Point(23, 26), Point(140, 23), Point(22, 106)]
-    o = find_origin(pts)
-    assert o == Point(22, 24), o
-
-    pts = [Point(2, 12), Point(897, 12), Point(2, 183)]
-    o = find_origin(pts)
-    assert o == Point(2, 12), 0
-
-
-if __name__ == "__main__":
-    test_origin()
+import typing as T
+import statistics
+import math
+
+
+class Point:
+    """A point in 2D space."""
+
+    def __init__(self, x, y):
+        """
+        Initialize a point.
+
+        Args:
+            x: A float representing the x-coordinate of the point.
+            y: A float representing the y-coordinate of the point.
+
+        Returns:
+            None.
+        """
+        self.x = int(x)
+        self.y = int(y)
+
+    @classmethod
+    def fromCSV(cls, csv: str) -> "Point":
+        xy = [float(x) for x in csv.split(",")]
+        return cls(xy[0], xy[1])
+
+    def __eq__(self, other) -> bool:
+        """
+        Check if two points are equal.
+
+        Args:
+            other: An object representing the other point.
+
+        Returns:
+            A boolean indicating whether the two points are equal.
+        """
+        return (self.x == other.x) and (self.y == other.y)
+
+    def __hash__(self):
+        """
+    Compute origin of given points.
+
+    Args:
+        pts: A list of Point objects representing the points.
+
+    Returns:
+        A Point object representing the origin of the points.
+    """
+        return hash((self.x, self.y))
+
+    def __repr__(self):
+        """
+        Return a string representation of the point.
+
+        Args:
+            None.
+
+        Returns:
+            A string representation of the point.
+        """
+        return f"({self.x}, {self.y})"
+
+    def __iter__(self):
+        """
+        Return an iterator over the coordinates of the point.
+
+        Args:
+            None.
+
+        Returns:
+            An iterator over the coordinates of the point.
+        """
+        return iter((self.x, self.y))
+
+
+def find_origin(pts: T.List[Point]) -> Point:
+    """
+    Compute origin of given points.
+
+    Args:
+        pts: A list of Point objects representing the points.
+
+    Returns:
+        A Point object representing the origin of the points.
+    """
+    horizontal = set()
+    for i, p1 in enumerate(pts):
+        for _, p2 in enumerate(pts[i + 1:]):
+            if abs(p1.x - p2.x) <= 2:
+                continue
+            m = (p2.y - p1.y) / (p2.x - p1.x)
+            if abs(m) < math.tan(math.pi / 180 * 5):  # <5 deg is horizontal.
+                horizontal.add(p1)
+                horizontal.add(p2)
+
+    points = set(pts)
+    assert len(horizontal) > 1, f"Must have at least two colinear points {horizontal}"
+    verticals = points - horizontal
+    assert len(verticals) > 0, "Must be at least one vertical point"
+    originY = statistics.mean([p.y for p in horizontal])
+    originX = statistics.mean([p.x for p in verticals])
+    return Point(originX, originY)
+
+
+def test_origin():
+    pts = [Point(81, 69), Point(1779, 68), Point(81, 449)]
+    p = find_origin(pts)
+    assert p == Point(81, 68), p == Point(81, 68)
+
+    pts = [Point(23, 26), Point(140, 23), Point(22, 106)]
+    o = find_origin(pts)
+    assert o == Point(22, 24), o
+
+    pts = [Point(2, 12), Point(897, 12), Point(2, 183)]
+    o = find_origin(pts)
+    assert o == Point(2, 12), 0
+
+
+if __name__ == "__main__":
+    test_origin()
```

### Comparing `plotscanner-0.0.2/plotscanner/grid.py` & `plotscanner-0.0.3/plotscanner/grid.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-from pathlib import Path
-import cv2 as cv
-import numpy as np
-
-import tempfile
-
-TEMP = tempfile.gettempdir()
-
-
-def _save_fig(img, outfile):
-    """
-    Saves the image to the specified file.
-
-    Args:
-        img: A numpy array representing the image to save.
-        outfile: A string representing the path to the output file.
-
-    Returns:
-        None.
-    """
-    print(f"Saved to {outfile}")
-    cv.imwrite(outfile, img)
-
-
-def remove_horizontal_grid_simple(img) -> np.ndarray:
-    """
-    Removes horizontal grid lines from an image using a simple algorithm.
-
-    Args:
-        img: A numpy array representing the image.
-
-    Returns:
-        A numpy array representing the image with the horizontal grid lines removed.
-    """
-    μ, σ = img.mean(), img.std()
-    for i, row in enumerate(img):
-        if row.mean() < μ - σ:
-            # I can simply remove the row.
-            img[i, :] = img.max()
-    return img
-
-
-def heal(orig):
-    """
-    Applies a morphological opening operation to the image to remove small objects.
-
-    Args:
-        orig: A numpy array representing the original image.
-
-    Returns:
-        A numpy array representing the image with small objects removed.
-    """
-    kernel = np.ones((3, 3), np.uint8)
-    img = cv.morphologyEx(orig.copy(), cv.MORPH_OPEN, kernel, iterations=2)
-    return img
-
-
-def remove_grid(
-    orig, num_iter=3, background_color: int = 255, grid_size: int = 2
-) -> np.ndarray:
-    """
-    Removes the grid from an image.
-
-    Args:
-        orig: A numpy array representing the original image.
-        num_iter: An integer representing the number of iterations to perform.
-        background_color: An integer representing the background color of the image.
-        grid_size: An integer representing the size of the grid lines.
-
-    Returns:
-        A numpy array representing the image with the grid removed.
-    """
-    img = orig.copy()
-    thres = cv.threshold(img, 0, 255, cv.THRESH_BINARY_INV + cv.THRESH_OTSU)[1]
-    # Remove horizontal lines
-    horizontal_kernel = cv.getStructuringElement(cv.MORPH_RECT, (40, 1))
-    remove_horizontal = cv.morphologyEx(
-        thres, cv.MORPH_OPEN, horizontal_kernel, iterations=num_iter
-    )
-    cnts = cv.findContours(remove_horizontal, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
-    cnts = cnts[0] if len(cnts) == 2 else cnts[1]
-    for c in cnts:
-        cv.drawContours(img, [c], -1, background_color, grid_size)
-
-    # Remove vertical lines
-    vertical_kernel = cv.getStructuringElement(cv.MORPH_RECT, (1, 40))
-    remove_vertical = cv.morphologyEx(
-        thres, cv.MORPH_OPEN, vertical_kernel, iterations=num_iter
-    )
-    cnts = cv.findContours(remove_vertical, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
-    cnts = cnts[0] if len(cnts) == 2 else cnts[1]
-    for c in cnts:
-        cv.drawContours(img, [c], -1, background_color, grid_size)
-    return img
-
-
-def test_remove_grid(imgfile: Path, debug: bool = True):
-    img = cv.imread(str(imgfile), 0)
-    if debug:
-        _save_fig(img, f"{TEMP}/orig.png")
-    withoutgrid = remove_grid(img)
-    assert withoutgrid.mean() > img.mean()
-    if debug:
-        _save_fig(withoutgrid, f"{TEMP}/without_grid.png")
-
-
-if __name__ == "__main__":
-    sdir = Path(__file__).parent
-    test_remove_grid(sdir / "../figures/graph_with_grid.png", True)
+from pathlib import Path
+import cv2 as cv
+import numpy as np
+
+import tempfile
+
+TEMP = tempfile.gettempdir()
+
+
+def _save_fig(img, outfile):
+    """
+    Saves the image to the specified file.
+
+    Args:
+        img: A numpy array representing the image to save.
+        outfile: A string representing the path to the output file.
+
+    Returns:
+        None.
+    """
+    print(f"Saved to {outfile}")
+    cv.imwrite(outfile, img)
+
+
+def remove_horizontal_grid_simple(img) -> np.ndarray:
+    """
+    Removes horizontal grid lines from an image using a simple algorithm.
+
+    Args:
+        img: A numpy array representing the image.
+
+    Returns:
+        A numpy array representing the image with the horizontal grid lines removed.
+    """
+    μ, σ = img.mean(), img.std()
+    for i, row in enumerate(img):
+        if row.mean() < μ - σ:
+            # I can simply remove the row.
+            img[i, :] = img.max()
+    return img
+
+
+def heal(orig):
+    """
+    Applies a morphological opening operation to the image to remove small objects.
+
+    Args:
+        orig: A numpy array representing the original image.
+
+    Returns:
+        A numpy array representing the image with small objects removed.
+    """
+    kernel = np.ones((3, 3), np.uint8)
+    img = cv.morphologyEx(orig.copy(), cv.MORPH_OPEN, kernel, iterations=2)
+    return img
+
+
+def remove_grid(
+    orig, num_iter=3, background_color: int = 255, grid_size: int = 2
+) -> np.ndarray:
+    """
+    Removes the grid from an image.
+
+    Args:
+        orig: A numpy array representing the original image.
+        num_iter: An integer representing the number of iterations to perform.
+        background_color: An integer representing the background color of the image.
+        grid_size: An integer representing the size of the grid lines.
+
+    Returns:
+        A numpy array representing the image with the grid removed.
+    """
+    img = orig.copy()
+    thres = cv.threshold(img, 0, 255, cv.THRESH_BINARY_INV + cv.THRESH_OTSU)[1]
+    # Remove horizontal lines
+    horizontal_kernel = cv.getStructuringElement(cv.MORPH_RECT, (40, 1))
+    remove_horizontal = cv.morphologyEx(
+        thres, cv.MORPH_OPEN, horizontal_kernel, iterations=num_iter
+    )
+    cnts = cv.findContours(remove_horizontal, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
+    cnts = cnts[0] if len(cnts) == 2 else cnts[1]
+    for c in cnts:
+        cv.drawContours(img, [c], -1, background_color, grid_size)
+
+    # Remove vertical lines
+    vertical_kernel = cv.getStructuringElement(cv.MORPH_RECT, (1, 40))
+    remove_vertical = cv.morphologyEx(
+        thres, cv.MORPH_OPEN, vertical_kernel, iterations=num_iter
+    )
+    cnts = cv.findContours(remove_vertical, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)
+    cnts = cnts[0] if len(cnts) == 2 else cnts[1]
+    for c in cnts:
+        cv.drawContours(img, [c], -1, background_color, grid_size)
+    return img
+
+
+def test_remove_grid(imgfile: Path, debug: bool = True):
+    img = cv.imread(str(imgfile), 0)
+    if debug:
+        _save_fig(img, f"{TEMP}/orig.png")
+    withoutgrid = remove_grid(img)
+    assert withoutgrid.mean() > img.mean()
+    if debug:
+        _save_fig(withoutgrid, f"{TEMP}/without_grid.png")
+
+
+if __name__ == "__main__":
+    sdir = Path(__file__).parent
+    test_remove_grid(sdir / "../figures/graph_with_grid.png", True)
```

### Comparing `plotscanner-0.0.2/plotscanner/plotdigitizer.py` & `plotscanner-0.0.3/plotscanner/plotdigitizer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,392 +1,392 @@
-import os
-import typing as T
-import tempfile
-import hashlib
-from pathlib import Path
-
-import cv2 as cv
-
-import numpy as np
-import numpy.typing as npt
-import numpy.polynomial.polynomial as poly
-
-import grid
-from trajectory import find_trajectory, normalize
-import geometry
-
-# Logger
-import logging
-
-LOGLEVEL = os.environ.get("LOGLEVEL", "INFO").upper()
-logging.basicConfig(level=LOGLEVEL)
-
-WindowName_ = "PlotDigitizer"
-ix_, iy_ = 0, 0
-params_: T.Dict[str, T.Any] = {}
-
-args_: T.Optional[T.Any] = None
-
-# NOTE: remember these are cv coordinates and not numpy.
-locations_: T.List[geometry.Point] = []
-points_: T.List[geometry.Point] = []
-
-img_: np.ndarray = np.zeros((1, 1))
-
-
-def cache() -> Path:
-    """
-    Returns the path to the cache directory.
-
-    Returns:
-        Path to the cache directory.
-    """
-    c = Path(tempfile.gettempdir()) / "plotdigitizer"
-    c.mkdir(parents=True, exist_ok=True)
-    return c
-
-
-def data_to_hash(data) -> str:
-    """
-    Returns the SHA1 hash of the data.
-
-    Args:
-        data: data to hash
-
-    Returns:
-        SHA1 hash of the data.
-    """
-    return hashlib.sha1(data).hexdigest()
-
-
-def save_img_in_cache(
-        img: npt.ArrayLike, filename: T.Optional[T.Union[Path, str]] = None
-):
-    """
-    Saves the image in the cache directory.
-
-    Args:
-        img: image to save
-        filename: filename to use. If None, the SHA1 hash of the image is used.
-
-    Returns:
-        None
-    """
-    if filename is None:
-        filename = Path(f"{data_to_hash(img)}.png")
-    outpath = cache() / filename
-    cv.imwrite(str(outpath), img)
-    logging.debug(f" Saved to {outpath}")
-
-
-def plot_traj(traj, outfile: Path):
-    """ 
-    Plots the trajectory and saves it to outfile.
-
-    Args:
-        traj: trajectory to plot
-        outfile: output file
-
-    Returns:   
-        None
-    """
-    global locations_
-    import matplotlib.pyplot as plt
-
-    x, y = zip(*traj)
-    plt.figure()
-    plt.subplot(211)
-
-    for p in locations_:
-        csize = img_.shape[0] // 40
-        cv.circle(img_, (p.x, img_.shape[0] - p.y), csize, 128, -1)
-
-    plt.imshow(img_, interpolation="none", cmap="gray")
-    plt.axis(False)
-    plt.title("Original")
-    plt.subplot(212)
-    plt.title("Reconstructed")
-    plt.plot(x, y)
-    plt.tight_layout()
-    if not str(outfile):
-        plt.show()
-    else:
-        plt.savefig(outfile)
-        logging.info(f"Saved to {outfile}")
-    plt.close()
-
-
-def list_to_points(points) -> T.List[geometry.Point]:
-    """
-    Converts a list of strings representing points to a list of Point objects.
-
-    Args:
-        points: A list of strings representing points in CSV format.
-
-    Returns:
-        A list of Point objects.
-    """
-    ps = [geometry.Point.fromCSV(x) for x in points]
-    return ps
-
-
-def axis_transformation(p, P: T.List[geometry.Point]):
-    """Compute m and offset for model Y = m X + offset that is used to transform
-    axis X to Y
-
-    Args:
-        p: A list of tuples representing the old axis.
-        P: A list of Point objects representing the new axis.
-
-    Returns:
-        A tuple containing the slope and offset for the transformation.
-    """
-
-    # Currently only linear maps and only 2D.
-    px, py = zip(*p)
-    Px, Py = zip(*P)
-    offX, sX = poly.polyfit(px, Px, 1)
-    offY, sY = poly.polyfit(py, Py, 1)
-    return ((sX, sY), (offX, offY))
-
-
-def transform_axis(img, erase_near_axis: int = 0):
-    """
-    Transforms the axis of the image based on the user's clicks.
-
-    Args:
-        img: A numpy array representing the image to transform.
-        erase_near_axis: An integer representing the number of rows and columns to erase near the axis.
-    Returns:
-        A tuple containing the slope and offset for the transformation.
-    """
-    global locations_
-    global points_
-    # extra: extra rows and cols to erase. Help in containing error near axis.
-    # compute the transformation between old and new axis.
-    T = axis_transformation(points_, locations_)
-    p = geometry.find_origin(locations_)
-    offCols, offRows = p.x, p.y
-    logging.info(f"{locations_} → origin {offCols}, {offRows}")
-    img[:, : offCols + erase_near_axis] = params_["background"]
-    img[-offRows - erase_near_axis:, :] = params_["background"]
-    logging.debug(f"Tranformation params: {T}")
-    return T
-
-
-def _find_trajectory_colors(
-        img: np.ndarray, plot: bool = False
-) -> T.Tuple[int, T.List[int]]:
-    """
-    Finds the background and trajectory colors in the image.
-
-    Args:
-        img: A numpy array representing the image.
-
-    Returns:
-        A tuple containing the background color and a list of trajectory colors.
-    """
-    # Each trajectory color x is bounded in the range x-3 to x+2 (interval of
-    # 5) -> total 51 bins. Also it is very unlikely that colors which are too
-    # close to each other are part of different trajecotries. It is safe to
-    # assme a binwidth of at least 10px.
-    hs, bs = np.histogram(img.flatten(), 255 // 10, (0, img.max()))
-
-    # Now a trajectory is only trajectory if number of pixels close to the
-    # width of the image (we are using at least 75% of width).
-    hs[hs < img.shape[1] * 3 // 4] = 0
-
-    if plot:
-        import matplotlib.pyplot as plt
-
-        plt.figure()
-        plt.bar(bs[:-1], np.log(hs))
-        plt.xlabel("color")
-        plt.ylabel("log(#pixel)")
-        plt.show()
-
-    # background is usually the color which is most count. We can find it
-    # easily by sorting the histogram.
-    hist = sorted(zip(hs, bs), reverse=True)
-
-    # background is the most occuring pixel value.
-    bgcolor = int(hist[0][1])
-
-    # we assume that bgcolor is close to white.
-    if bgcolor < 128:
-        logging.error(
-            "I computed that background is 'dark' which is unacceptable to me."
-        )
-        quit(-1)
-
-    # If the background is white, search from the trajectories from the black.
-    trajcolors = [int(b) for h, b in hist if h > 0 and b / bgcolor < 0.5]
-    return bgcolor, trajcolors
-
-
-def compute_foregrond_background_stats(img) -> T.Dict[str, float]:
-    """
-    Computes the foreground and background color of the image.
-
-    Args:
-        img: A numpy array representing the image.
-
-    Returns:
-        A dictionary containing the computed parameters.
-    """
-    params: T.Dict[str, T.Any] = {}
-    # Compute the histogram. It should be a multimodal histogram. Find peaks
-    # and these are the colors of background and foregorunds. Currently
-    # implementation is very simple.
-    bgcolor, trajcolors = _find_trajectory_colors(img)
-    params["background"] = bgcolor
-    params["timeseries_colors"] = trajcolors
-    logging.debug(f" computed parameters: {params}")
-    return params
-
-
-def process_image(img):
-    """
-    Processes the image to extract data.
-
-    Args:
-        img: A numpy array representing the image.
-
-    Returns:
-        traj: A numpy array representing the trajectory.
-    """
-    global params_
-    global args_
-    params_ = compute_foregrond_background_stats(img)
-
-    T = transform_axis(img, erase_near_axis=3)
-    assert img.std() > 0.0, "No data in the image!"
-    logging.info(f" {img.mean()}  {img.std()}")
-    save_img_in_cache(img, f"{args_.INPUT.name}.transformed_axis.png")
-
-    # extract the plot that has color which is farthest from the background.
-    trajcolor = params_["timeseries_colors"][0]
-    img = normalize(img)
-    traj, img = find_trajectory(img, trajcolor, T)
-    save_img_in_cache(img, f"{args_.INPUT.name}.final.png")
-    return traj
-
-
-def run(args):
-    """
-    Runs the program.
-
-    Args:
-        args: A namespace containing the arguments.
-    """
-    global locations_, points_
-    global img_, args_
-    args_ = args
-
-    infile = Path(args.INPUT)
-    assert infile.exists(), f"{infile} does not exists."
-    logging.info(f"Extracting trajectories from {infile}")
-
-    # reads into gray-scale.
-    img_ = cv.imread(str(infile), 0)
-    img_ = normalize(img_)
-
-    # erosion after dilation (closes gaps)
-    if args_.preprocess:
-        kernel = np.ones((1, 1), np.uint8)
-        img_ = cv.morphologyEx(img_, cv.MORPH_CLOSE, kernel)
-        save_img_in_cache(img_, Path(f"{args_.INPUT.name}.close.png"))
-
-    # remove grids.
-    img_ = grid.remove_grid(img_)
-    save_img_in_cache(img_, Path(f"{args_.INPUT.name}.without_grid.png"))
-
-    # rescale it again.
-    img_ = normalize(img_)
-    logging.debug(" {img_.min()=} {img_.max()=}")
-    assert img_.max() <= 255
-    assert img_.min() < img_.mean() < img_.max(), "Could not read meaningful data"
-    save_img_in_cache(img_, args_.INPUT.name)
-
-    points_ = list_to_points(args.data_point)
-    locations_ = list_to_points(args.location)
-    logging.debug(f"data points {args.data_point} → location on image {args.location}")
-
-    if len(locations_) != len(points_):
-        logging.warning(
-            "Either the location of data-points are not specified or their numbers don't"
-            " match with given datapoints. Asking user..."
-        )
-
-    traj = process_image(img_)
-
-    if args_.plot is not None:
-        plot_traj(traj, args_.plot)
-
-    outfile = args.output or f"{args.INPUT}.traj.csv"
-    with open(outfile, "w") as f:
-        for r in traj:
-            f.write("%g %g\n" % (r))
-    logging.info("Wrote trajectory to %s" % outfile)
-    
-    
-    np.save('points.npy', traj)
-
-
-def main():
-    """
-    Main function.
-
-    Returns:
-        A namespace containing the arguments.
-    """
-    # Argument parser.
-    import argparse
-
-    description = """Digitize image."""
-    parser = argparse.ArgumentParser(description=description)
-    parser.add_argument("INPUT", type=Path, help="Input image file.")
-    parser.add_argument(
-        "--data-point",
-        "-p",
-        required=True,
-        action="append",
-        help="Datapoints (min 3 required). You have to click on them later."
-             " At least 3 points are recommended. e.g -p 0,0 -p 10,0 -p 0,1 "
-             "Make sure that point are comma separated without any space.",
-    )
-    parser.add_argument(
-        "--location",
-        "-l",
-        required=False,
-        default=[],
-        action="append",
-        help="Location of a points on figure in pixels (integer)."
-             " These values should appear in the same order as -p option."
-             " If not given, you will be asked to click on the figure.",
-    )
-    parser.add_argument(
-        "--plot",
-        default=None,
-        required=False,
-        help="Plot the final result. Requires matplotlib.",
-    )
-    parser.add_argument(
-        "--output",
-        "-o",
-        required=False,
-        type=str,
-        help="Name of the output file else trajectory will be written to "
-             " <INPUT>.traj.csv",
-    )
-    parser.add_argument(
-        "--preprocess",
-        required=False,
-        action="store_true",
-        help="Preprocess the image. Useful with bad resolution images.",
-    )
-    args = parser.parse_args()
-    run(args)
-
-
-if __name__ == "__main__":
-    main()
+import os
+import typing as T
+import tempfile
+import hashlib
+from pathlib import Path
+
+import cv2 as cv
+
+import numpy as np
+import numpy.typing as npt
+import numpy.polynomial.polynomial as poly
+
+import grid
+from trajectory import find_trajectory, normalize
+import geometry
+
+# Logger
+import logging
+
+LOGLEVEL = os.environ.get("LOGLEVEL", "INFO").upper()
+logging.basicConfig(level=LOGLEVEL)
+
+WindowName_ = "PlotDigitizer"
+ix_, iy_ = 0, 0
+params_: T.Dict[str, T.Any] = {}
+
+args_: T.Optional[T.Any] = None
+
+# NOTE: remember these are cv coordinates and not numpy.
+locations_: T.List[geometry.Point] = []
+points_: T.List[geometry.Point] = []
+
+img_: np.ndarray = np.zeros((1, 1))
+
+
+def cache() -> Path:
+    """
+    Returns the path to the cache directory.
+
+    Returns:
+        Path to the cache directory.
+    """
+    c = Path(tempfile.gettempdir()) / "plotdigitizer"
+    c.mkdir(parents=True, exist_ok=True)
+    return c
+
+
+def data_to_hash(data) -> str:
+    """
+    Returns the SHA1 hash of the data.
+
+    Args:
+        data: data to hash
+
+    Returns:
+        SHA1 hash of the data.
+    """
+    return hashlib.sha1(data).hexdigest()
+
+
+def save_img_in_cache(
+        img: npt.ArrayLike, filename: T.Optional[T.Union[Path, str]] = None
+):
+    """
+    Saves the image in the cache directory.
+
+    Args:
+        img: image to save
+        filename: filename to use. If None, the SHA1 hash of the image is used.
+
+    Returns:
+        None
+    """
+    if filename is None:
+        filename = Path(f"{data_to_hash(img)}.png")
+    outpath = cache() / filename
+    cv.imwrite(str(outpath), img)
+    logging.debug(f" Saved to {outpath}")
+
+
+def plot_traj(traj, outfile: Path):
+    """ 
+    Plots the trajectory and saves it to outfile.
+
+    Args:
+        traj: trajectory to plot
+        outfile: output file
+
+    Returns:   
+        None
+    """
+    global locations_
+    import matplotlib.pyplot as plt
+
+    x, y = zip(*traj)
+    plt.figure()
+    plt.subplot(211)
+
+    for p in locations_:
+        csize = img_.shape[0] // 40
+        cv.circle(img_, (p.x, img_.shape[0] - p.y), csize, 128, -1)
+
+    plt.imshow(img_, interpolation="none", cmap="gray")
+    plt.axis(False)
+    plt.title("Original")
+    plt.subplot(212)
+    plt.title("Reconstructed")
+    plt.plot(x, y)
+    plt.tight_layout()
+    if not str(outfile):
+        plt.show()
+    else:
+        plt.savefig(outfile)
+        logging.info(f"Saved to {outfile}")
+    plt.close()
+
+
+def list_to_points(points) -> T.List[geometry.Point]:
+    """
+    Converts a list of strings representing points to a list of Point objects.
+
+    Args:
+        points: A list of strings representing points in CSV format.
+
+    Returns:
+        A list of Point objects.
+    """
+    ps = [geometry.Point.fromCSV(x) for x in points]
+    return ps
+
+
+def axis_transformation(p, P: T.List[geometry.Point]):
+    """Compute m and offset for model Y = m X + offset that is used to transform
+    axis X to Y
+
+    Args:
+        p: A list of tuples representing the old axis.
+        P: A list of Point objects representing the new axis.
+
+    Returns:
+        A tuple containing the slope and offset for the transformation.
+    """
+
+    # Currently only linear maps and only 2D.
+    px, py = zip(*p)
+    Px, Py = zip(*P)
+    offX, sX = poly.polyfit(px, Px, 1)
+    offY, sY = poly.polyfit(py, Py, 1)
+    return ((sX, sY), (offX, offY))
+
+
+def transform_axis(img, erase_near_axis: int = 0):
+    """
+    Transforms the axis of the image based on the user's clicks.
+
+    Args:
+        img: A numpy array representing the image to transform.
+        erase_near_axis: An integer representing the number of rows and columns to erase near the axis.
+    Returns:
+        A tuple containing the slope and offset for the transformation.
+    """
+    global locations_
+    global points_
+    # extra: extra rows and cols to erase. Help in containing error near axis.
+    # compute the transformation between old and new axis.
+    T = axis_transformation(points_, locations_)
+    p = geometry.find_origin(locations_)
+    offCols, offRows = p.x, p.y
+    logging.info(f"{locations_} → origin {offCols}, {offRows}")
+    img[:, : offCols + erase_near_axis] = params_["background"]
+    img[-offRows - erase_near_axis:, :] = params_["background"]
+    logging.debug(f"Tranformation params: {T}")
+    return T
+
+
+def _find_trajectory_colors(
+        img: np.ndarray, plot: bool = False
+) -> T.Tuple[int, T.List[int]]:
+    """
+    Finds the background and trajectory colors in the image.
+
+    Args:
+        img: A numpy array representing the image.
+
+    Returns:
+        A tuple containing the background color and a list of trajectory colors.
+    """
+    # Each trajectory color x is bounded in the range x-3 to x+2 (interval of
+    # 5) -> total 51 bins. Also it is very unlikely that colors which are too
+    # close to each other are part of different trajecotries. It is safe to
+    # assme a binwidth of at least 10px.
+    hs, bs = np.histogram(img.flatten(), 255 // 10, (0, img.max()))
+
+    # Now a trajectory is only trajectory if number of pixels close to the
+    # width of the image (we are using at least 75% of width).
+    hs[hs < img.shape[1] * 3 // 4] = 0
+
+    if plot:
+        import matplotlib.pyplot as plt
+
+        plt.figure()
+        plt.bar(bs[:-1], np.log(hs))
+        plt.xlabel("color")
+        plt.ylabel("log(#pixel)")
+        plt.show()
+
+    # background is usually the color which is most count. We can find it
+    # easily by sorting the histogram.
+    hist = sorted(zip(hs, bs), reverse=True)
+
+    # background is the most occuring pixel value.
+    bgcolor = int(hist[0][1])
+
+    # we assume that bgcolor is close to white.
+    if bgcolor < 128:
+        logging.error(
+            "I computed that background is 'dark' which is unacceptable to me."
+        )
+        quit(-1)
+
+    # If the background is white, search from the trajectories from the black.
+    trajcolors = [int(b) for h, b in hist if h > 0 and b / bgcolor < 0.5]
+    return bgcolor, trajcolors
+
+
+def compute_foregrond_background_stats(img) -> T.Dict[str, float]:
+    """
+    Computes the foreground and background color of the image.
+
+    Args:
+        img: A numpy array representing the image.
+
+    Returns:
+        A dictionary containing the computed parameters.
+    """
+    params: T.Dict[str, T.Any] = {}
+    # Compute the histogram. It should be a multimodal histogram. Find peaks
+    # and these are the colors of background and foregorunds. Currently
+    # implementation is very simple.
+    bgcolor, trajcolors = _find_trajectory_colors(img)
+    params["background"] = bgcolor
+    params["timeseries_colors"] = trajcolors
+    logging.debug(f" computed parameters: {params}")
+    return params
+
+
+def process_image(img):
+    """
+    Processes the image to extract data.
+
+    Args:
+        img: A numpy array representing the image.
+
+    Returns:
+        traj: A numpy array representing the trajectory.
+    """
+    global params_
+    global args_
+    params_ = compute_foregrond_background_stats(img)
+
+    T = transform_axis(img, erase_near_axis=3)
+    assert img.std() > 0.0, "No data in the image!"
+    logging.info(f" {img.mean()}  {img.std()}")
+    save_img_in_cache(img, f"{args_.INPUT.name}.transformed_axis.png")
+
+    # extract the plot that has color which is farthest from the background.
+    trajcolor = params_["timeseries_colors"][0]
+    img = normalize(img)
+    traj, img = find_trajectory(img, trajcolor, T)
+    save_img_in_cache(img, f"{args_.INPUT.name}.final.png")
+    return traj
+
+
+def run(args):
+    """
+    Runs the program.
+
+    Args:
+        args: A namespace containing the arguments.
+    """
+    global locations_, points_
+    global img_, args_
+    args_ = args
+
+    infile = Path(args.INPUT)
+    assert infile.exists(), f"{infile} does not exists."
+    logging.info(f"Extracting trajectories from {infile}")
+
+    # reads into gray-scale.
+    img_ = cv.imread(str(infile), 0)
+    img_ = normalize(img_)
+
+    # erosion after dilation (closes gaps)
+    if args_.preprocess:
+        kernel = np.ones((1, 1), np.uint8)
+        img_ = cv.morphologyEx(img_, cv.MORPH_CLOSE, kernel)
+        save_img_in_cache(img_, Path(f"{args_.INPUT.name}.close.png"))
+
+    # remove grids.
+    img_ = grid.remove_grid(img_)
+    save_img_in_cache(img_, Path(f"{args_.INPUT.name}.without_grid.png"))
+
+    # rescale it again.
+    img_ = normalize(img_)
+    logging.debug(" {img_.min()=} {img_.max()=}")
+    assert img_.max() <= 255
+    assert img_.min() < img_.mean() < img_.max(), "Could not read meaningful data"
+    save_img_in_cache(img_, args_.INPUT.name)
+
+    points_ = list_to_points(args.data_point)
+    locations_ = list_to_points(args.location)
+    logging.debug(f"data points {args.data_point} → location on image {args.location}")
+
+    if len(locations_) != len(points_):
+        logging.warning(
+            "Either the location of data-points are not specified or their numbers don't"
+            " match with given datapoints. Asking user..."
+        )
+
+    traj = process_image(img_)
+
+    if args_.plot is not None:
+        plot_traj(traj, args_.plot)
+
+    outfile = args.output or f"{args.INPUT}.traj.csv"
+    with open(outfile, "w") as f:
+        for r in traj:
+            f.write("%g %g\n" % (r))
+    logging.info("Wrote trajectory to %s" % outfile)
+    
+    
+    np.save('points.npy', traj)
+
+
+def main():
+    """
+    Main function.
+
+    Returns:
+        A namespace containing the arguments.
+    """
+    # Argument parser.
+    import argparse
+
+    description = """Digitize image."""
+    parser = argparse.ArgumentParser(description=description)
+    parser.add_argument("INPUT", type=Path, help="Input image file.")
+    parser.add_argument(
+        "--data-point",
+        "-p",
+        required=True,
+        action="append",
+        help="Datapoints (min 3 required). You have to click on them later."
+             " At least 3 points are recommended. e.g -p 0,0 -p 10,0 -p 0,1 "
+             "Make sure that point are comma separated without any space.",
+    )
+    parser.add_argument(
+        "--location",
+        "-l",
+        required=False,
+        default=[],
+        action="append",
+        help="Location of a points on figure in pixels (integer)."
+             " These values should appear in the same order as -p option."
+             " If not given, you will be asked to click on the figure.",
+    )
+    parser.add_argument(
+        "--plot",
+        default=None,
+        required=False,
+        help="Plot the final result. Requires matplotlib.",
+    )
+    parser.add_argument(
+        "--output",
+        "-o",
+        required=False,
+        type=str,
+        help="Name of the output file else trajectory will be written to "
+             " <INPUT>.traj.csv",
+    )
+    parser.add_argument(
+        "--preprocess",
+        required=False,
+        action="store_true",
+        help="Preprocess the image. Useful with bad resolution images.",
+    )
+    args = parser.parse_args()
+    run(args)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `plotscanner-0.0.2/plotscanner/trajectory.py` & `plotscanner-0.0.3/plotscanner/trajectory.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-import numpy as np
-import cv2 as cv
-from collections import defaultdict
-import logging
-
-
-def _find_center(vec):
-    """
-    Find the center of a vector.
-
-    Args:
-        vec: A numpy array representing the vector.
-
-    Returns:
-        A float representing the center of the vector.
-    """
-    return np.median(vec)
-
-
-def normalize(img):
-    """
-    Normalize an image to 0-255.
-
-    Args:
-        img: A numpy array representing the image.
-
-    Returns:
-        A numpy array representing the normalized image.
-    """
-    return np.interp(img, (img.min(), img.max()), (0, 255)).astype(np.uint8)
-
-
-def fit_trajectory_using_median(traj, T, img):
-    """
-    Fit a trajectory using the median.
-
-    Args:
-        traj: A defaultdict representing the trajectory.
-        T: A tuple representing the transformation.
-        img: A numpy array representing the image.
-
-    Returns:
-        A list of tuples representing the trajectory.
-    """
-    (sX, sY), (offX, offY) = T
-    res = []
-    r, _ = img.shape
-
-    # x, y = zip(*sorted(traj.items()))
-    # logging.info((xvec, ys))
-
-    for k in sorted(traj):
-        x = k
-
-        vals = np.array(traj[k])
-
-        # For each x, we may multiple pixels in column of the image which might
-        # be y. Usually experience is that the trajectories are close to the
-        # top rather to the bottom. So we discard call pixel which are below
-        # the center of mass (median here)
-        # These are opencv pixles. So there valus starts from the top. 0
-        # belogs to top row. Therefore > rather than <.
-        avg = np.median(vals)
-        vals = vals[np.where(vals >= avg)]
-        if len(vals) == 0:
-            continue
-
-        # Still we have multiple candidates for y for each x.
-        # We find the center of these points and call it the y for given x.
-        y = _find_center(vals)
-        cv.circle(img, (x, int(y)), 1, 255, -1)
-        x1 = (x - offX) / sX
-        y1 = (r - y - offY) / sY
-        res.append((x1, y1))
-
-    # sort by x-axis.
-    return sorted(res)
-
-
-def _valid_px(val: int) -> int:
-    """
-    Ensure that a pixel value is within the valid range.
-
-    Args:
-        val: An integer representing the pixel value.
-
-    Returns:
-        An integer representing the valid pixel value.
-    """
-    return min(max(0, val), 255)
-
-
-def find_trajectory(img: np.ndarray, pixel: int, T):
-    """
-    Find the trajectory of a pixel in an image.
-
-    Args:
-        img: A numpy array representing the image.
-        pixel: An integer representing the pixel value.
-        T: A tuple representing the transformation.
-
-    Returns:
-        result: A list of tuples representing the trajectory.
-        img: A numpy array representing the image.
-    """
-    logging.info(f"Extracting trajectory for color {pixel}")
-    assert (
-            img.min() <= pixel <= img.max()
-    ), f"{pixel} is outside the range: [{img.min()}, {img.max()}]"
-
-    # Find all pixels which belongs to a trajectory.
-    o = 6
-    _clower, _cupper = _valid_px(pixel - o // 2), _valid_px(pixel + o // 2)
-
-    Y, X = np.where((img >= _clower) & (img <= _cupper))
-    traj = defaultdict(list)
-    for x, y in zip(X, Y):
-        traj[x].append(y)
-
-    assert traj, "Empty trajectory"
-
-    # this is a simple fit using median.
-    new = np.zeros_like(img)
-    res = fit_trajectory_using_median(traj, T, new)
-    return res, np.vstack((img, new))
+import numpy as np
+import cv2 as cv
+from collections import defaultdict
+import logging
+
+
+def _find_center(vec):
+    """
+    Find the center of a vector.
+
+    Args:
+        vec: A numpy array representing the vector.
+
+    Returns:
+        A float representing the center of the vector.
+    """
+    return np.median(vec)
+
+
+def normalize(img):
+    """
+    Normalize an image to 0-255.
+
+    Args:
+        img: A numpy array representing the image.
+
+    Returns:
+        A numpy array representing the normalized image.
+    """
+    return np.interp(img, (img.min(), img.max()), (0, 255)).astype(np.uint8)
+
+
+def fit_trajectory_using_median(traj, T, img):
+    """
+    Fit a trajectory using the median.
+
+    Args:
+        traj: A defaultdict representing the trajectory.
+        T: A tuple representing the transformation.
+        img: A numpy array representing the image.
+
+    Returns:
+        A list of tuples representing the trajectory.
+    """
+    (sX, sY), (offX, offY) = T
+    res = []
+    r, _ = img.shape
+
+    # x, y = zip(*sorted(traj.items()))
+    # logging.info((xvec, ys))
+
+    for k in sorted(traj):
+        x = k
+
+        vals = np.array(traj[k])
+
+        # For each x, we may multiple pixels in column of the image which might
+        # be y. Usually experience is that the trajectories are close to the
+        # top rather to the bottom. So we discard call pixel which are below
+        # the center of mass (median here)
+        # These are opencv pixles. So there valus starts from the top. 0
+        # belogs to top row. Therefore > rather than <.
+        avg = np.median(vals)
+        vals = vals[np.where(vals >= avg)]
+        if len(vals) == 0:
+            continue
+
+        # Still we have multiple candidates for y for each x.
+        # We find the center of these points and call it the y for given x.
+        y = _find_center(vals)
+        cv.circle(img, (x, int(y)), 1, 255, -1)
+        x1 = (x - offX) / sX
+        y1 = (r - y - offY) / sY
+        res.append((x1, y1))
+
+    # sort by x-axis.
+    return sorted(res)
+
+
+def _valid_px(val: int) -> int:
+    """
+    Ensure that a pixel value is within the valid range.
+
+    Args:
+        val: An integer representing the pixel value.
+
+    Returns:
+        An integer representing the valid pixel value.
+    """
+    return min(max(0, val), 255)
+
+
+def find_trajectory(img: np.ndarray, pixel: int, T):
+    """
+    Find the trajectory of a pixel in an image.
+
+    Args:
+        img: A numpy array representing the image.
+        pixel: An integer representing the pixel value.
+        T: A tuple representing the transformation.
+
+    Returns:
+        result: A list of tuples representing the trajectory.
+        img: A numpy array representing the image.
+    """
+    logging.info(f"Extracting trajectory for color {pixel}")
+    assert (
+            img.min() <= pixel <= img.max()
+    ), f"{pixel} is outside the range: [{img.min()}, {img.max()}]"
+
+    # Find all pixels which belongs to a trajectory.
+    o = 6
+    _clower, _cupper = _valid_px(pixel - o // 2), _valid_px(pixel + o // 2)
+
+    Y, X = np.where((img >= _clower) & (img <= _cupper))
+    traj = defaultdict(list)
+    for x, y in zip(X, Y):
+        traj[x].append(y)
+
+    assert traj, "Empty trajectory"
+
+    # this is a simple fit using median.
+    new = np.zeros_like(img)
+    res = fit_trajectory_using_median(traj, T, new)
+    return res, np.vstack((img, new))
```

### Comparing `plotscanner-0.0.2/plotscanner/widgets.py` & `plotscanner-0.0.3/plotscanner/widgets.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,330 +1,330 @@
-from math import ceil
-
-import cv2
-import matplotlib
-import numpy as np
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
-from matplotlib.figure import Figure
-from PyQt5 import QtCore
-from PyQt5.QtGui import QMouseEvent
-
-
-class MplCanvas(FigureCanvasQTAgg):
-    """
-    Matplotlib Qt Embedding
-    """
-
-    def __init__(self, parent=None, width=10, height=10, dpi=100):
-        self.fig = Figure(figsize=(width, height), dpi=dpi)
-        super(MplCanvas, self).__init__(self.fig)
-        self.axes = self.fig.add_subplot(1, 1, 1)
-
-    def update_canvas(self):
-        """
-        Updates the canvas by redrawing it.
-        """
-        self.fig.canvas.draw()
-
-
-class Magnifier(MplCanvas):
-    """
-    Magnifier for user image
-    """
-
-    def __init__(self, parent):
-        super().__init__()
-        # Remove margins and axes
-        self.axes.axis("off")
-        self.fig.subplots_adjust(left=0, bottom=0, right=1, top=1)
-
-        self.parent = parent
-
-        # Point in the center of the magnifier
-        self.circle = self.draw_magnifier_point((10, 10), 3)
-
-    def draw_magnifier_point(self, point, radius):
-        """
-        Draws a point in the center of the magnifier.
-
-        Args:
-            point (tuple): The coordinates of the point to be drawn.
-            radius (int): The radius of the point to be drawn.
-
-        Returns:
-            Circle: The circle object representing the point.
-        """
-        x, y = point
-        circle = matplotlib.patches.Circle(
-            (x, y), radius, facecolor='red', edgecolor='red')
-        self.axes.add_patch(circle)
-        return circle
-
-    def update_magnifier_point(self):
-        """
-        Redraws the point in the center of the magnifier (erases the old one).
-        """
-        # Get value from slider
-        padding = self.parent.scale_slider.value()
-
-        self.circle.remove()
-        self.circle = self.draw_magnifier_point(
-            (padding, padding), ceil(padding / 32))
-
-
-class PlotCanvas(MplCanvas):
-    """
-    The digitized plot.
-    """
-
-    def __init__(self):
-        super().__init__()
-        self.img = None
-        self.orig = None
-
-    def draw_plot(self, x, y):
-        """
-        Draws a plot with the given x and y values.
-
-        Args:
-            x (list): The x values of the plot.
-            y (list): The y values of the plot.
-        """
-        self.axes.plot(x, y)
-        self.axes.set_xlabel('x')
-        self.axes.set_ylabel('y')
-        self.update_canvas()
-
-
-class ImageCanvas(MplCanvas):
-    """
-    The user's image.
-    """
-
-    def __init__(self, parent):
-        super().__init__()
-        self.img = None
-        self.orig = None
-        # Reduce margins and disable axes
-        self.axes.axis("off")
-        # Remove image margins
-        self.fig.subplots_adjust(left=0, bottom=0, right=1, top=1)
-        self.parent = parent
-        # Get value from slider
-        self.padding = parent.scale_slider.value()  # on each side
-        self.setMouseTracking(True)
-        self.points = []
-        self.mpl_connect('button_press_event', self.on_click)
-
-        # Coefficients
-        self.k_image = 1
-        self.k_canvas = 1
-        self.image_over_canvas = 1
-        self.pad = 10
-
-    def show_user_image(self, path):
-        """
-        Opens the image at the specified path.
-
-        Args:
-            path (str): The path to the image to be opened.
-        """
-        # Check path validity
-        if path[0] == '':
-            return
-        # Clear points
-        for i in range(len(self.points)):
-            self.remove_point(0)
-        # Original image
-        self.orig = cv2.imread(path[0])
-        self.orig = self.orig[..., ::-1]
-        # Image to be shown to user
-        self.img = np.array(self.orig, copy=True)
-        # Get value from slider
-        self.padding = self.parent.scale_slider.value()
-        # Add padding for magnifier
-        self.add_padding(self.padding)
-        self.axes.imshow(self.orig, cmap='gray')
-        self.update_canvas()
-        self.count_koeffs()
-
-    def add_padding(self, padding):
-        """
-        Adds white pixels around the perimeter of the image.
-
-        Args:
-            padding (int): The number of pixels to add on each side of the image.
-        """
-        self.padding = padding
-        # Padding
-        old_image_height, old_image_width, channels = self.orig.shape
-        # Create new image of desired size and color (white) for padding
-        new_image_width = old_image_width + padding * 2
-        new_image_height = old_image_height + padding * 2
-        color = (255, 255, 255)  # white
-        result = np.full((new_image_height, new_image_width,
-                          channels), color, dtype=np.uint8)
-
-        # Compute center offset
-        x_center = (new_image_width - old_image_width) // 2
-        y_center = (new_image_height - old_image_height) // 2
-
-        # Copy original image into center of result image
-        result[y_center:y_center + old_image_height,
-               x_center:x_center + old_image_width] = self.orig
-
-        self.img = result
-
-    def mouseMoveEvent(self, a0: QMouseEvent) -> None:
-        """
-        Handles mouse movement events.
-
-        Args:
-            a0 (QMouseEvent): The mouse event to be handled.
-        """
-        x = a0.pos().x()
-        y = a0.pos().y()
-        self.mouseMoved(x, y)
-        return super().mouseMoveEvent(a0)
-
-    def remove_point(self, index):
-        """
-        Removes a point.
-
-        Args:
-            index (int): The index of the point to be removed.
-        """
-        circle = self.points.pop(index)
-        self.parent.table.remove_row(index)
-        circle.remove()
-        self.update_canvas()
-
-    def add_point(self, x, y, radius):
-        """
-        Adds a point.
-
-        Args:
-            x (int): The x coordinate of the point to be added.
-            y (int): The y coordinate of the point to be added.
-            radius (int): The radius of the point to be added.
-        """
-        if len(self.points) >= 3:
-            return
-        h, _, _ = self.orig.shape
-        self.parent.table.add_row(int(x), int(h - y))
-        circle = matplotlib.patches.Circle(
-            (x, y), radius, facecolor='blue', edgecolor='blue')
-        self.axes.add_patch(circle)
-        self.points.append(circle)
-        self.update_canvas()
-
-    def on_click(self, event):
-        """
-        Handles left mouse button clicks - adds or removes a point.
-
-        Args:
-            event (MouseEvent): The mouse event to be handled.
-        """
-        if self.img is not None:
-            for i, circle in enumerate(self.points):
-                if circle.contains(event)[0]:
-                    self.parent.selected_row = None
-                    self.remove_point(i)
-                    return
-            x, y = event.xdata, event.ydata
-            if x is not None and y is not None:
-                radius = 7
-                self.add_point(x, y, radius)
-
-    def wheelEvent(self, event):
-        """
-        Handles mouse wheel events.
-
-        Args:
-            event (WheelEvent): The wheel event to be handled.
-        """
-        if event.angleDelta().y() > 0:
-            # Wheel is scrolling up
-            value = self.parent.scale_slider.value() - self.parent.scale_slider.singleStep()
-            if value >= self.parent.scale_slider.minimum():
-                self.parent.scale_slider.setValue(value)
-        else:
-            # Wheel is scrolling down
-            value = self.parent.scale_slider.value() + self.parent.scale_slider.singleStep()
-            if value <= self.parent.scale_slider.maximum():
-                self.parent.scale_slider.setValue(value)
-        # For smoothness
-        cursor_pos = event.pos()
-        self.mouseMoved(cursor_pos.x(), cursor_pos.y())
-
-    def count_koeffs(self):
-        """
-        Calculates the aspect ratio and scale coefficients for the image and canvas.
-        The coefficients only change under certain conditions, so it's better to calculate them once.
-        These coefficients are needed for the magnifier.
-        """
-        # Get original image from canvas
-        orig = self.orig
-        # Check for image presence in canvas
-        if orig is None:
-            return
-
-        # Get image dimensions
-        h_image, w_image, _ = orig.shape
-        # Get canvas dimensions
-        w_canvas, h_canvas = self.size().width(), self.size().height()
-
-        # Calculate aspect ratio coefficients for image and canvas (w:h)
-        self.k_image = w_image / h_image
-        self.k_canvas = w_canvas / h_canvas
-
-        # Convert canvas coordinates to image coordinates with padding
-        # Here, padding is the area of the canvas not occupied by the image
-        if self.k_canvas > self.k_image:  # Vertical image - padding on sides
-            # Calculate scale coefficient image / canvas
-            self.image_over_canvas = h_image / h_canvas
-            self.pad = round((w_canvas - h_canvas * self.k_image) / 2)
-        else:  # Horizontal image - padding on top and bottom
-            self.image_over_canvas = w_image / w_canvas
-            self.pad = round((h_canvas - w_canvas / self.k_image) / 2)
-
-    def mouseMoved(self, x, y):
-        """
-        Handles mouse movement within the canvas (redraws the magnification).
-
-        Args:
-            x (int): The x coordinate of the mouse cursor.
-            y (int): The y coordinate of the mouse cursor.
-        """
-        # Get image (with padding) from canvas
-        # Here padding is additional white pixels around the perimeter,
-        # so that it is possible to crop the edges of the image for the magnifier
-        img = self.img
-        # Check for image presence in canvas
-        if img is None:
-            return
-        padding = self.padding
-        # Get image dimensions (with padding)
-        h_image, w_image, _ = img.shape
-
-        # Convert canvas coordinates to image coordinates with padding
-        if self.k_canvas > self.k_image:  # Vertical image - padding on sides
-            x_image = round((x - self.pad) * self.image_over_canvas)
-            y_image = round((y) * self.image_over_canvas)
-        else:  # Horizontal image - padding on top and bottom
-            x_image = round((x) * self.image_over_canvas)
-            y_image = round((y - self.pad) * self.image_over_canvas)
-
-        # Transition from padded image to unpadded image
-        # Recalculate coordinates
-        y_image += padding
-        x_image += padding
-        # Handle edge values
-        y_image = max(padding, min(y_image, h_image - padding - 1))
-        x_image = max(padding, min(x_image, w_image - padding - 1))
-
-        # Crop padded image
-        img = img[y_image - padding:y_image + padding,
-                  x_image - padding:x_image + padding, :]
-
-        self.parent.magnifierImCanvas.axes.imshow(img, cmap='gray')
-        self.parent.magnifierImCanvas.update_canvas()
+from math import ceil
+
+import cv2
+import matplotlib
+import numpy as np
+from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
+from matplotlib.figure import Figure
+from PyQt5 import QtCore
+from PyQt5.QtGui import QMouseEvent
+
+
+class MplCanvas(FigureCanvasQTAgg):
+    """
+    Matplotlib Qt Embedding
+    """
+
+    def __init__(self, parent=None, width=10, height=10, dpi=100):
+        self.fig = Figure(figsize=(width, height), dpi=dpi)
+        super(MplCanvas, self).__init__(self.fig)
+        self.axes = self.fig.add_subplot(1, 1, 1)
+
+    def update_canvas(self):
+        """
+        Updates the canvas by redrawing it.
+        """
+        self.fig.canvas.draw()
+
+
+class Magnifier(MplCanvas):
+    """
+    Magnifier for user image
+    """
+
+    def __init__(self, parent):
+        super().__init__()
+        # Remove margins and axes
+        self.axes.axis("off")
+        self.fig.subplots_adjust(left=0, bottom=0, right=1, top=1)
+
+        self.parent = parent
+
+        # Point in the center of the magnifier
+        self.circle = self.draw_magnifier_point((10, 10), 3)
+
+    def draw_magnifier_point(self, point, radius):
+        """
+        Draws a point in the center of the magnifier.
+
+        Args:
+            point (tuple): The coordinates of the point to be drawn.
+            radius (int): The radius of the point to be drawn.
+
+        Returns:
+            Circle: The circle object representing the point.
+        """
+        x, y = point
+        circle = matplotlib.patches.Circle(
+            (x, y), radius, facecolor='red', edgecolor='red')
+        self.axes.add_patch(circle)
+        return circle
+
+    def update_magnifier_point(self):
+        """
+        Redraws the point in the center of the magnifier (erases the old one).
+        """
+        # Get value from slider
+        padding = self.parent.scale_slider.value()
+
+        self.circle.remove()
+        self.circle = self.draw_magnifier_point(
+            (padding, padding), ceil(padding / 32))
+
+
+class PlotCanvas(MplCanvas):
+    """
+    The digitized plot.
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.img = None
+        self.orig = None
+
+    def draw_plot(self, x, y):
+        """
+        Draws a plot with the given x and y values.
+
+        Args:
+            x (list): The x values of the plot.
+            y (list): The y values of the plot.
+        """
+        self.axes.plot(x, y)
+        self.axes.set_xlabel('x')
+        self.axes.set_ylabel('y')
+        self.update_canvas()
+
+
+class ImageCanvas(MplCanvas):
+    """
+    The user's image.
+    """
+
+    def __init__(self, parent):
+        super().__init__()
+        self.img = None
+        self.orig = None
+        # Reduce margins and disable axes
+        self.axes.axis("off")
+        # Remove image margins
+        self.fig.subplots_adjust(left=0, bottom=0, right=1, top=1)
+        self.parent = parent
+        # Get value from slider
+        self.padding = parent.scale_slider.value()  # on each side
+        self.setMouseTracking(True)
+        self.points = []
+        self.mpl_connect('button_press_event', self.on_click)
+
+        # Coefficients
+        self.k_image = 1
+        self.k_canvas = 1
+        self.image_over_canvas = 1
+        self.pad = 10
+
+    def show_user_image(self, path):
+        """
+        Opens the image at the specified path.
+
+        Args:
+            path (str): The path to the image to be opened.
+        """
+        # Check path validity
+        if path[0] == '':
+            return
+        # Clear points
+        for i in range(len(self.points)):
+            self.remove_point(0)
+        # Original image
+        self.orig = cv2.imread(path[0])
+        self.orig = self.orig[..., ::-1]
+        # Image to be shown to user
+        self.img = np.array(self.orig, copy=True)
+        # Get value from slider
+        self.padding = self.parent.scale_slider.value()
+        # Add padding for magnifier
+        self.add_padding(self.padding)
+        self.axes.imshow(self.orig, cmap='gray')
+        self.update_canvas()
+        self.count_koeffs()
+
+    def add_padding(self, padding):
+        """
+        Adds white pixels around the perimeter of the image.
+
+        Args:
+            padding (int): The number of pixels to add on each side of the image.
+        """
+        self.padding = padding
+        # Padding
+        old_image_height, old_image_width, channels = self.orig.shape
+        # Create new image of desired size and color (white) for padding
+        new_image_width = old_image_width + padding * 2
+        new_image_height = old_image_height + padding * 2
+        color = (255, 255, 255)  # white
+        result = np.full((new_image_height, new_image_width,
+                          channels), color, dtype=np.uint8)
+
+        # Compute center offset
+        x_center = (new_image_width - old_image_width) // 2
+        y_center = (new_image_height - old_image_height) // 2
+
+        # Copy original image into center of result image
+        result[y_center:y_center + old_image_height,
+               x_center:x_center + old_image_width] = self.orig
+
+        self.img = result
+
+    def mouseMoveEvent(self, a0: QMouseEvent) -> None:
+        """
+        Handles mouse movement events.
+
+        Args:
+            a0 (QMouseEvent): The mouse event to be handled.
+        """
+        x = a0.pos().x()
+        y = a0.pos().y()
+        self.mouseMoved(x, y)
+        return super().mouseMoveEvent(a0)
+
+    def remove_point(self, index):
+        """
+        Removes a point.
+
+        Args:
+            index (int): The index of the point to be removed.
+        """
+        circle = self.points.pop(index)
+        self.parent.table.remove_row(index)
+        circle.remove()
+        self.update_canvas()
+
+    def add_point(self, x, y, radius):
+        """
+        Adds a point.
+
+        Args:
+            x (int): The x coordinate of the point to be added.
+            y (int): The y coordinate of the point to be added.
+            radius (int): The radius of the point to be added.
+        """
+        if len(self.points) >= 3:
+            return
+        h, _, _ = self.orig.shape
+        self.parent.table.add_row(int(x), int(h - y))
+        circle = matplotlib.patches.Circle(
+            (x, y), radius, facecolor='blue', edgecolor='blue')
+        self.axes.add_patch(circle)
+        self.points.append(circle)
+        self.update_canvas()
+
+    def on_click(self, event):
+        """
+        Handles left mouse button clicks - adds or removes a point.
+
+        Args:
+            event (MouseEvent): The mouse event to be handled.
+        """
+        if self.img is not None:
+            for i, circle in enumerate(self.points):
+                if circle.contains(event)[0]:
+                    self.parent.selected_row = None
+                    self.remove_point(i)
+                    return
+            x, y = event.xdata, event.ydata
+            if x is not None and y is not None:
+                radius = 7
+                self.add_point(x, y, radius)
+
+    def wheelEvent(self, event):
+        """
+        Handles mouse wheel events.
+
+        Args:
+            event (WheelEvent): The wheel event to be handled.
+        """
+        if event.angleDelta().y() > 0:
+            # Wheel is scrolling up
+            value = self.parent.scale_slider.value() - self.parent.scale_slider.singleStep()
+            if value >= self.parent.scale_slider.minimum():
+                self.parent.scale_slider.setValue(value)
+        else:
+            # Wheel is scrolling down
+            value = self.parent.scale_slider.value() + self.parent.scale_slider.singleStep()
+            if value <= self.parent.scale_slider.maximum():
+                self.parent.scale_slider.setValue(value)
+        # For smoothness
+        cursor_pos = event.pos()
+        self.mouseMoved(cursor_pos.x(), cursor_pos.y())
+
+    def count_koeffs(self):
+        """
+        Calculates the aspect ratio and scale coefficients for the image and canvas.
+        The coefficients only change under certain conditions, so it's better to calculate them once.
+        These coefficients are needed for the magnifier.
+        """
+        # Get original image from canvas
+        orig = self.orig
+        # Check for image presence in canvas
+        if orig is None:
+            return
+
+        # Get image dimensions
+        h_image, w_image, _ = orig.shape
+        # Get canvas dimensions
+        w_canvas, h_canvas = self.size().width(), self.size().height()
+
+        # Calculate aspect ratio coefficients for image and canvas (w:h)
+        self.k_image = w_image / h_image
+        self.k_canvas = w_canvas / h_canvas
+
+        # Convert canvas coordinates to image coordinates with padding
+        # Here, padding is the area of the canvas not occupied by the image
+        if self.k_canvas > self.k_image:  # Vertical image - padding on sides
+            # Calculate scale coefficient image / canvas
+            self.image_over_canvas = h_image / h_canvas
+            self.pad = round((w_canvas - h_canvas * self.k_image) / 2)
+        else:  # Horizontal image - padding on top and bottom
+            self.image_over_canvas = w_image / w_canvas
+            self.pad = round((h_canvas - w_canvas / self.k_image) / 2)
+
+    def mouseMoved(self, x, y):
+        """
+        Handles mouse movement within the canvas (redraws the magnification).
+
+        Args:
+            x (int): The x coordinate of the mouse cursor.
+            y (int): The y coordinate of the mouse cursor.
+        """
+        # Get image (with padding) from canvas
+        # Here padding is additional white pixels around the perimeter,
+        # so that it is possible to crop the edges of the image for the magnifier
+        img = self.img
+        # Check for image presence in canvas
+        if img is None:
+            return
+        padding = self.padding
+        # Get image dimensions (with padding)
+        h_image, w_image, _ = img.shape
+
+        # Convert canvas coordinates to image coordinates with padding
+        if self.k_canvas > self.k_image:  # Vertical image - padding on sides
+            x_image = round((x - self.pad) * self.image_over_canvas)
+            y_image = round((y) * self.image_over_canvas)
+        else:  # Horizontal image - padding on top and bottom
+            x_image = round((x) * self.image_over_canvas)
+            y_image = round((y - self.pad) * self.image_over_canvas)
+
+        # Transition from padded image to unpadded image
+        # Recalculate coordinates
+        y_image += padding
+        x_image += padding
+        # Handle edge values
+        y_image = max(padding, min(y_image, h_image - padding - 1))
+        x_image = max(padding, min(x_image, w_image - padding - 1))
+
+        # Crop padded image
+        img = img[y_image - padding:y_image + padding,
+                  x_image - padding:x_image + padding, :]
+
+        self.parent.magnifierImCanvas.axes.imshow(img, cmap='gray')
+        self.parent.magnifierImCanvas.update_canvas()
```

### Comparing `plotscanner-0.0.2/plotscanner.egg-info/PKG-INFO` & `plotscanner-0.0.3/plotscanner.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-Metadata-Version: 2.1
-Name: plotscanner
-Version: 0.0.2
-Summary: The application for digitizing images of plots.
-Home-page: https://github.com/IlS0/Plot-digitization
-Author-email: silru@internet.ru
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-# Plotscanner
-
-A __Python3__ application used to convert images of functional data plots to digital format.
-Often data is presented in documents or scientific articles in the form of figures. In order to use this data, it must be digitized in some way. This program allows you to get a scanned image of a plot in _JPEG_ or _PNG_ format and quickly digitize the values. The numbers can be saved to a file (_CSV_, _XLS_, _TXT_, etc.) and used.
-
-## Documentation 
-You can find the documentation for all of the application's basic modules [here](https://github.com/IlS0/Plot-digitization/tree/main/docs/plotscanner).
-
-## Installation
-`$ pip install plotscanner`
-
-
-### Docker-image
-
-You can download a docker-image of the application if you want to use the back-end part in the container 
-`$ docker pull ils0/plotscanner`
-
-or build it yourself with the following command:
-
-`$ docker build -t plotscanner .`
-
-
-## Run
-Start the application by running the command in the terminal:
-`$ plotscanner`
-
-Follow the instructions in the app window to work correctly.
-### Image preparing
-Plotscanner requires the input data in the correct form to work right. Before loading the image, crop it and save only the axes and lines of the plot like this.
-![Example image](./plotscanner/readme_imgs/example.jpg)
-
-
+Metadata-Version: 2.1
+Name: plotscanner
+Version: 0.0.3
+Summary: The application for digitizing images of plots.
+Home-page: https://github.com/IlS0/Plot-digitization
+Author-email: silru@internet.ru
+Description-Content-Type: text/markdown
+
+# Plotscanner
+
+A __Python3__ application used to convert images of functional data plots to digital format.
+Often data is presented in documents or scientific articles in the form of figures. In order to use this data, it must be digitized in some way. This program allows you to get a scanned image of a plot in _JPEG_ or _PNG_ format and quickly digitize the values. The numbers can be saved to a file (_CSV_, _XLS_, _TXT_, etc.) and used.
+
+## Documentation 
+You can find the documentation for all of the application's basic modules [here](https://github.com/IlS0/Plot-digitization/tree/main/docs/plotscanner).
+
+## Installation
+`$ pip install plotscanner`
+
+
+### Docker-image
+
+You can download a docker-image of the application if you want to use the back-end part in the container
+
+`$ docker pull ils0/plotscanner`
+
+or build it yourself with the following command:
+
+`$ docker build -t plotscanner .`
+
+
+## Run
+Start the application by running the command in the terminal:
+`$ plotscanner`
+
+Follow the instructions in the app window to work correctly.
+### Image preparing
+Plotscanner requires the input data in the correct form to work right. Before loading the image, crop it and save only the axes and lines of the plot like this.
+![Example image](./plotscanner/readme_imgs/example.jpg)
```

### Comparing `plotscanner-0.0.2/setup.py` & `plotscanner-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fin:
     long_description = fin.read()
 
 setup(name='plotscanner',
-      version='0.0.2',
+      version='0.0.3',
       description='The application for digitizing images of plots.',
       packages=['plotscanner'],
       py_modules = ['plotscanner'],
       author_email='silru@internet.ru',
       zip_safe=False,
       long_description=long_description,
       long_description_content_type="text/markdown",
```

