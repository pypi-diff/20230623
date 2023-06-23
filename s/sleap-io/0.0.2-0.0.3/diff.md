# Comparing `tmp/sleap_io-0.0.2-py3-none-any.whl.zip` & `tmp/sleap_io-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 28955 bytes, number of entries: 18
--rw-r--r--  2.0 unx      637 b- defN 22-Dec-13 04:48 sleap_io/__init__.py
--rw-r--r--  2.0 unx       86 b- defN 22-Dec-13 04:48 sleap_io/io/__init__.py
--rw-r--r--  2.0 unx    11420 b- defN 22-Dec-13 04:48 sleap_io/io/labelstudio.py
+Zip file size: 34905 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      642 b- defN 23-Jun-23 20:06 sleap_io/__init__.py
+-rw-r--r--  2.0 unx       86 b- defN 22-Aug-03 04:32 sleap_io/io/__init__.py
+-rw-r--r--  2.0 unx    11647 b- defN 23-Jun-23 17:08 sleap_io/io/labelstudio.py
 -rw-r--r--  2.0 unx     2177 b- defN 22-Dec-13 04:48 sleap_io/io/main.py
--rw-r--r--  2.0 unx    17566 b- defN 22-Dec-13 04:48 sleap_io/io/nwb.py
--rw-r--r--  2.0 unx     8478 b- defN 22-Dec-13 04:48 sleap_io/io/slp.py
--rw-r--r--  2.0 unx     7810 b- defN 22-Dec-13 04:48 sleap_io/io/utils.py
--rw-r--r--  2.0 unx       54 b- defN 22-Dec-13 04:48 sleap_io/model/__init__.py
--rw-r--r--  2.0 unx    14032 b- defN 22-Dec-13 04:48 sleap_io/model/instance.py
--rw-r--r--  2.0 unx     2271 b- defN 22-Dec-13 04:48 sleap_io/model/labeled_frame.py
--rw-r--r--  2.0 unx     7377 b- defN 22-Dec-13 04:48 sleap_io/model/labels.py
+-rw-r--r--  2.0 unx    17498 b- defN 23-Jun-23 17:08 sleap_io/io/nwb.py
+-rw-r--r--  2.0 unx     8905 b- defN 23-Jun-23 20:06 sleap_io/io/slp.py
+-rw-r--r--  2.0 unx     7773 b- defN 23-Jun-23 17:08 sleap_io/io/utils.py
+-rw-r--r--  2.0 unx    21686 b- defN 23-Jun-23 20:06 sleap_io/io/video.py
+-rw-r--r--  2.0 unx       54 b- defN 22-Jul-23 01:13 sleap_io/model/__init__.py
+-rw-r--r--  2.0 unx    14128 b- defN 23-Jun-23 20:06 sleap_io/model/instance.py
+-rw-r--r--  2.0 unx     2425 b- defN 23-Jun-23 20:06 sleap_io/model/labeled_frame.py
+-rw-r--r--  2.0 unx     7235 b- defN 23-Jun-23 20:06 sleap_io/model/labels.py
 -rw-r--r--  2.0 unx     6376 b- defN 22-Dec-13 04:48 sleap_io/model/skeleton.py
--rw-r--r--  2.0 unx      933 b- defN 22-Dec-13 04:48 sleap_io/model/video.py
--rw-r--r--  2.0 unx     1517 b- defN 22-Dec-13 04:48 sleap_io-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4545 b- defN 22-Dec-13 04:48 sleap_io-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-13 04:48 sleap_io-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Dec-13 04:48 sleap_io-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1428 b- defN 22-Dec-13 04:48 sleap_io-0.0.2.dist-info/RECORD
-18 files, 86808 bytes uncompressed, 26637 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx     4067 b- defN 23-Jun-23 20:06 sleap_io/model/video.py
+-rw-r--r--  2.0 unx     1517 b- defN 23-Jun-23 20:24 sleap_io-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3118 b- defN 23-Jun-23 20:24 sleap_io-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 20:24 sleap_io-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-23 20:24 sleap_io-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1507 b- defN 23-Jun-23 20:24 sleap_io-0.0.3.dist-info/RECORD
+19 files, 110942 bytes uncompressed, 32471 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -15,14 +15,17 @@
 
 Filename: sleap_io/io/slp.py
 Comment: 
 
 Filename: sleap_io/io/utils.py
 Comment: 
 
+Filename: sleap_io/io/video.py
+Comment: 
+
 Filename: sleap_io/model/__init__.py
 Comment: 
 
 Filename: sleap_io/model/instance.py
 Comment: 
 
 Filename: sleap_io/model/labeled_frame.py
@@ -33,23 +36,23 @@
 
 Filename: sleap_io/model/skeleton.py
 Comment: 
 
 Filename: sleap_io/model/video.py
 Comment: 
 
-Filename: sleap_io-0.0.2.dist-info/LICENSE
+Filename: sleap_io-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: sleap_io-0.0.2.dist-info/METADATA
+Filename: sleap_io-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: sleap_io-0.0.2.dist-info/WHEEL
+Filename: sleap_io-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: sleap_io-0.0.2.dist-info/top_level.txt
+Filename: sleap_io-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sleap_io-0.0.2.dist-info/RECORD
+Filename: sleap_io-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sleap_io/__init__.py

```diff
@@ -1,12 +1,12 @@
 """This module exposes all high level APIs for sleap-io."""
 
 # Define package version.
-# This is read dynamically by setuptools in setup.cfg to determine the release version.
-__version__ = "0.0.2"
+# This is read dynamically by setuptools in pyproject.toml to determine the release version.
+__version__ = "0.0.3"
 
 from sleap_io.model.skeleton import Node, Edge, Skeleton, Symmetry
 from sleap_io.model.video import Video
 from sleap_io.model.instance import (
     Point,
     PredictedPoint,
     Track,
```

## sleap_io/io/labelstudio.py

```diff
@@ -9,14 +9,15 @@
 """
 
 import datetime
 import simplejson as json
 import math
 import uuid
 from typing import Dict, Iterable, List, Tuple, Optional, Union
+import warnings
 
 from sleap_io import Instance, LabeledFrame, Labels, Node, Point, Video, Skeleton
 
 
 def read_labels(
     labels_path: str, skeleton: Optional[Union[Skeleton, List[str]]] = None
 ) -> Labels:
@@ -70,15 +71,15 @@
                         node_names.add(node_name)
 
     skeleton = Skeleton(nodes=list(node_names))
     return skeleton
 
 
 def parse_tasks(tasks: List[Dict], skeleton: Skeleton) -> Labels:
-    """Read Label Studio style annotations from a file and return a `Labels` object
+    """Read Label Studio style annotations from a file and return a `Labels` object.
 
     Args:
         tasks: Collection of tasks to be converted to `Labels`.
         skeleton: `Skeleton` with the nodes and edges to be used.
 
     Returns:
         Parsed labels as a `Labels` instance.
@@ -103,15 +104,14 @@
 
     Args:
         labels: SLEAP `Labels` to be converted to Label Studio task format.
 
     Returns:
         Label Studio dictionaries of the `Labels` data.
     """
-
     out = []
     for frame in labels.labeled_frames:
         if frame.video.shape is not None:
             height = frame.video.shape[1]
             width = frame.video.shape[2]
         else:
             height = 100
@@ -224,21 +224,28 @@
     with open(filename, "w") as f:
         json.dump(ls_dicts, f, indent=4, default=_encode)
 
 
 def task_to_labeled_frame(
     task: dict, skeleton: Skeleton, key: str = "annotations"
 ) -> LabeledFrame:
-    """Parse annotations from an entry"""
+    """Parse annotations from an entry.
+
+    Args:
+        task: Label Studio task to be parsed.
+        skeleton: Skeleton to use for parsing.
+        key: Key to use for parsing annotations. Defaults to "annotations".
 
+    Returns:
+        Parsed `LabeledFrame` instance.
+    """
     if len(task[key]) > 1:
-        print(
-            "WARNING: Task {}: Multiple annotations found, only taking the first!".format(
-                task.get("id", "??")
-            )
+        warnings.warn(
+            f"Task {task.get('id', '??')}: Multiple annotations found, "
+            "only taking the first!"
         )
 
     # only parse the first entry result
     to_parse = task[key][0]["result"]
 
     individuals = filter_and_index(to_parse, "rectanglelabels")
     keypoints = filter_and_index(to_parse, "keypointlabels")
@@ -260,16 +267,17 @@
                     continue
 
                 points[node] = Point(x_pos, y_pos)
 
             if len(points) > 0:
                 instances.append(Instance(points, skeleton))
 
-    # If this is multi-animal, any leftover keypoints should be unique bodyparts, and will be collected here
-    # if single-animal, we only have 'unique bodyparts' [in a way] and the process is identical
+    # If this is multi-animal, any leftover keypoints should be unique bodyparts, and
+    # will be collected here if single-animal, we only have 'unique bodyparts' [in a
+    # way] and the process is identical
     points = {}
     for _, kpt in keypoints.items():
         node = Node(kpt["value"]["keypointlabels"][0])
         points[node] = Point(
             (kpt["value"]["x"] * kpt["original_width"]) / 100,
             (kpt["value"]["y"] * kpt["original_height"]) / 100,
             visible=True,
@@ -279,23 +287,23 @@
 
     video, frame_idx = video_from_task(task)
 
     return LabeledFrame(video, frame_idx, instances)
 
 
 def filter_and_index(annotations: Iterable[dict], annot_type: str) -> Dict[str, dict]:
-    """Filter annotations based on the type field and index them by ID
+    """Filter annotations based on the type field and index them by ID.
 
     Args:
         annotation: annotations to filter and index
         annot_type: annotation type to filter e.x. 'keypointlabels' or 'rectanglelabels'
 
     Returns:
-        Dict[str, dict] - indexed and filtered annotations. Only annotations of type
-        `annot_type` will survive, and annotations are indexed by ID.
+        Dict of ndexed and filtered annotations. Only annotations of type `annot_type`
+        will survive, and annotations are indexed by ID.
     """
     filtered = list(filter(lambda d: d["type"] == annot_type, annotations))
     indexed = {item["id"]: item for item in filtered}
     return indexed
 
 
 def build_relation_map(annotations: Iterable[dict]) -> Dict[str, List[str]]:
```

## sleap_io/io/nwb.py

```diff
@@ -1,9 +1,8 @@
-"""Functions to write and read from the neurodata without borders (NWB) format. 
-"""
+"""Functions to write and read from the neurodata without borders (NWB) format."""
 from copy import deepcopy
 from typing import List, Optional, Union
 from pathlib import Path
 import datetime
 import uuid
 import re
 
@@ -56,15 +55,14 @@
 
         # Get track
         test_pose_estimation: PoseEstimation = test_processing_module[track_keys[0]]
         node_names = test_pose_estimation.nodes[:]
         edge_inds = test_pose_estimation.edges[:]
 
         for processing_module in nwb_file.values():
-
             # Get track keys
             _track_keys: List[str] = list(processing_module.fields["data_interfaces"])
             is_tracked: bool = re.sub("[0-9]+", "", _track_keys[0]) == "track"
 
             # Figure out the max number of frames and the canonical timestamps
             timestamps = np.empty(())
             for track_key in _track_keys:
@@ -142,46 +140,44 @@
 
 def write_nwb(
     labels: Labels,
     nwbfile_path: str,
     nwb_file_kwargs: Optional[dict] = None,
     pose_estimation_metadata: Optional[dict] = None,
 ):
-    """Write labels to an nwb file and save it to the nwbfile_path given
+    """Write labels to an nwb file and save it to the nwbfile_path given.
 
     Args:
-        labels (Labels): A general label object
-        nwbfile_path (str): The path where the nwb file is to be written
-        nwb_file_kwargs (Optional[dict], optional): A dict containing metadata to
-        the nwbfile. Example:
-        nwb_file_kwargs = {
-            'session_description: 'your_session_description',
-            'identifier': 'your session_identifier',
-        }
-        For a full list of possible values see:
-        https://pynwb.readthedocs.io/en/stable/pynwb.file.html#pynwb.file.NWBFile
-
-        Defaults to None and default values are used to generate the nwb file.
-
-        pose_estimation_metadata (dict): This argument has a dual purpose:
-
-        1) It can be used to pass time information about the video which is
-        necessary for synchronizing frames in pose estimation tracking to other
-        modalities. Either the video timestamps can be passed to
-        This can be used to pass the timestamps with the key `video_timestamps`
-        or the sampling rate with key`video_sample_rate`.
-
-        e.g. pose_estimation_metadata["video_timestamps"] = np.array(timestamps)
-        or   pose_estimation_metadata["video_sample_rate] = 15  # In Hz
-
-        2) The other use of this dictionary is to ovewrite sleap-io default
-        arguments for the PoseEstimation container.
-        see https://github.com/rly/ndx-pose for a full list or arguments.
-    """
+        labels: A general `Labels` object.
+        nwbfile_path: The path where the nwb file is to be written.
+        nwb_file_kwargs: A dict containing metadata to the nwbfile. Example:
+            nwb_file_kwargs = {
+                'session_description: 'your_session_description',
+                'identifier': 'your session_identifier',
+            }
+            For a full list of possible values see:
+            https://pynwb.readthedocs.io/en/stable/pynwb.file.html#pynwb.file.NWBFile
+
+            Defaults to None and default values are used to generate the nwb file.
+
+        pose_estimation_metadata: This argument has a dual purpose:
+
+            1) It can be used to pass time information about the video which is
+            necessary for synchronizing frames in pose estimation tracking to other
+            modalities. Either the video timestamps can be passed to
+            This can be used to pass the timestamps with the key `video_timestamps`
+            or the sampling rate with key`video_sample_rate`.
 
+            e.g. pose_estimation_metadata["video_timestamps"] = np.array(timestamps)
+            or   pose_estimation_metadata["video_sample_rate] = 15  # In Hz
+
+            2) The other use of this dictionary is to ovewrite sleap-io default
+            arguments for the PoseEstimation container.
+            see https://github.com/rly/ndx-pose for a full list or arguments.
+    """
     nwb_file_kwargs = nwb_file_kwargs or dict()
 
     # Add required values for nwbfile if not present
     session_description = nwb_file_kwargs.get(
         "session_description", "Processed SLEAP pose data"
     )
     session_start_time = nwb_file_kwargs.get(
@@ -224,28 +220,26 @@
             2) The other use of this dictionary is to ovewrite sleap-io default
             arguments for the PoseEstimation container.
             see https://github.com/rly/ndx-pose for a full list or arguments.
 
     Returns:
         An in-memory nwbfile with the data from the labels object appended.
     """
-
     pose_estimation_metadata = pose_estimation_metadata or dict()
 
     # Extract default metadata
     provenance = labels.provenance
     default_metadata = dict(scorer=str(provenance))
     sleap_version = provenance.get("sleap_version", None)
     default_metadata["source_software_version"] = sleap_version
 
     labels_data_df = convert_predictions_to_dataframe(labels)
 
     # For every video create a processing module
     for video_index, video in enumerate(labels.videos):
-
         video_path = Path(video.filename)
         processing_module_name = f"SLEAP_VIDEO_{video_index:03}_{video_path.stem}"
         nwb_processing_module = get_processing_module_for_video(
             processing_module_name, nwbfile
         )
 
         # Propagate video metadata
@@ -278,15 +272,15 @@
 def append_nwb(
     labels: Labels, filename: str, pose_estimation_metadata: Optional[dict] = None
 ):
     """Append a SLEAP `Labels` object to an existing NWB data file.
 
     Args:
         labels: A general `Labels` object.
-        nwbfile: And in-memory nwbfile where the data is to be appended.
+        filename: The path to the NWB file.
         pose_estimation_metadata: Metadata for pose estimation. See `append_nwb_data`
             for details.
 
     See also: append_nwb_data
     """
     with NWBHDF5IO(filename, mode="a", load_namespaces=True) as io:
         nwb_file = io.read()
@@ -324,15 +318,15 @@
 def build_pose_estimation_container_for_track(
     labels_data_df: pd.DataFrame,
     labels: Labels,
     track_name: str,
     video: Video,
     pose_estimation_metadata: dict,
 ) -> PoseEstimation:
-    """Creates a PoseEstimation container for a track.
+    """Create a PoseEstimation container for a track.
 
     Args:
         labels_data_df (pd.DataFrame): A pandas object with the data corresponding
         to the predicted instances associated to this labels object.
         labels (Labels): A general labels object
         track_name (str): The name of the track in labels.tracks
         video (Video): The video to which data belongs to
@@ -393,33 +387,30 @@
 
     return pose_estimation_container
 
 
 def build_track_pose_estimation_list(
     track_data_df: pd.DataFrame, timestamps: ArrayLike
 ) -> List[PoseEstimationSeries]:
-    """An auxiliar function to build a list of PoseEstimationSeries associated with
-    a Track object.
+    """Build a list of PoseEstimationSeries from tracks.
 
     Args:
         track_data_df (pd.DataFrame): A pandas DataFrame object containing the
         trajectories for all the nodes associated with a specific track.
 
     Returns:
         List[PoseEstimationSeries]: The list of all the PoseEstimationSeries.
         One for each node.
     """
-
     name_of_nodes_in_track = track_data_df.columns.get_level_values(
         "node_name"
     ).unique()
 
     pose_estimation_series_list: List[PoseEstimationSeries] = []
     for node_name in name_of_nodes_in_track:
-
         # Drop data with missing values
         data_for_node = track_data_df[node_name].dropna(axis="index", how="any")
 
         node_trajectory = data_for_node[["x", "y"]].to_numpy()
         confidence = data_for_node["score"].to_numpy()
 
         reference_frame = (
```

## sleap_io/io/slp.py

```diff
@@ -1,12 +1,12 @@
 """This module handles direct I/O operations for working with .slp files."""
 
 from __future__ import annotations
 import numpy as np
-import json
+import simplejson as json
 from typing import Union
 from sleap_io import (
     Video,
     Skeleton,
     Edge,
     Node,
     Track,
@@ -14,14 +14,15 @@
     PredictedPoint,
     Instance,
     PredictedInstance,
     LabeledFrame,
     Labels,
 )
 from sleap_io.io.utils import read_hdf5_attrs, read_hdf5_dataset
+from sleap_io.io.video import VideoBackend
 from enum import IntEnum
 
 
 class InstanceType(IntEnum):
     """Enumeration of instance types to integers."""
 
     USER = 0
@@ -37,16 +38,26 @@
     Returns:
         A list of `Video` objects.
     """
     # TODO (DS) - Find shape of video
     videos = [json.loads(x) for x in read_hdf5_dataset(labels_path, "videos_json")]
     video_objects = []
     for video in videos:
+        backend = video["backend"]
+        try:
+            backend = VideoBackend.from_filename(
+                backend["filename"],
+                dataset=backend.get("dataset", None),
+                grayscale=backend.get("grayscale", None),
+                input_format=backend.get("input_format", None),
+            )
+        except ValueError:
+            backend = None
         video_objects.append(
-            Video(filename=video["backend"]["filename"], backend=video["backend"])
+            Video(filename=video["backend"]["filename"], backend=backend)
         )
     return video_objects
 
 
 def read_tracks(labels_path: str) -> list[Track]:
     """Read `Track` dataset in a SLEAP labels file.
```

## sleap_io/io/utils.py

```diff
@@ -25,15 +25,15 @@
 
 def _overwrite_hdf5_dataset(
     f: Union[h5py.File, h5py.Group], dataset: str, data: np.ndarray
 ):
     """Overwrite dataset in HDF5 file.
 
     Args:
-        filename: Path to an HDF5 file.
+        f: Handle to HDF5 file.
         dataset: Path to a dataset.
         data: Data to write to dataset.
     """
     try:
         del f[dataset]
     except KeyError:
         pass
@@ -172,32 +172,31 @@
     with h5py.File(filename, "r+") as f:
         ds = f[dataset]
         for attr_name, attr_value in attributes.items():
             _overwrite_hdf5_attr(ds, attr_name, attr_value)
 
 
 def convert_predictions_to_dataframe(labels: Labels) -> pd.DataFrame:
-    """Helper function to convert predictions data to a Pandas dataframe.
+    """Convert predictions data to a Pandas dataframe.
 
     Args:
-        labels (Labels): A general label object.
-
-    Raises:
-        ValueError: If no frames in the label objects contain predicted instances.
+        labels: A general label object.
 
     Returns:
         pd.DataFrame: A pandas data frame with the structured data with
         hierarchical columns. The column hierarchy is:
                 "video_path",
                 "skeleton_name",
                 "track_name",
                 "node_name",
         And it is indexed by the frames.
-    """
 
+    Raises:
+        ValueError: If no frames in the label objects contain predicted instances.
+    """
     # Form pairs of labeled_frames and predicted instances
     labeled_frames = labels.labeled_frames
     all_frame_instance_tuples: Generator[
         tuple[LabeledFrame, PredictedInstance], None, None
     ] = (
         (label_frame, instance)  # type: ignore
         for label_frame in labeled_frames
```

## sleap_io/model/instance.py

```diff
@@ -15,54 +15,57 @@
 import math
 
 
 @define
 class Point:
     """A 2D spatial landmark and metadata associated with annotation.
 
-    Class Variables:
-    eq_atol: Controls absolute tolerence allowed in `x` and `y` when comparing two `Point`s for equality
-    eq_rtol: Controls relative tolerence allowed in `x` and `y` when comparing two `Point`s for equality
-
     Attributes:
         x: The horizontal pixel location of point in image coordinates.
         y: The vertical pixel location of point in image coordinates.
         visible: Whether point is visible in the image or not.
         complete: Has the point been verified by the user labeler.
+
+    Class variables:
+        eq_atol: Controls absolute tolerence allowed in `x` and `y` when comparing two
+            `Point`s for equality.
+        eq_rtol: Controls relative tolerence allowed in `x` and `y` when comparing two
+            `Point`s for equality.
+
     """
 
     eq_atol: ClassVar[float] = 1e-08
     eq_rtol: ClassVar[float] = 0
 
     x: float
     y: float
     visible: bool = True
     complete: bool = False
 
     def __eq__(self, other: object):
-        """Compare `self` and `other` for equality
+        """Compare `self` and `other` for equality.
 
         Precision error between the respective `x` and `y` properties of two
         instances may be allowed or controlled via the `Point.eq_atol` and
         `Point.eq_rtol` class variables. Set to zero to disable their effect.
         Internally, `numpy.isclose()` is used for the comparison:
         https://numpy.org/doc/stable/reference/generated/numpy.isclose.html
 
         Args:
-            self, other: instance of `Point` to compare
+            other: Instance of `Point` to compare to.
 
         Returns:
-            True if all attributes of `self` and `other` are the identical (possibly allowing
-            precision error for `x` and `y` attributes).
+            True if all attributes of `self` and `other` are the identical (possibly
+            allowing precision error for `x` and `y` attributes).
         """
-        # check that other is a Point
+        # Check that other is a Point.
         if type(other) is not type(self):
             return False
 
-        # we know that we have some kind of point at this point
+        # We know that we have some kind of point at this point.
         other = cast(Point, other)
 
         return bool(
             np.all(
                 np.isclose(
                     [self.x, self.y],
                     [other.x, other.y],
@@ -102,24 +105,24 @@
         return (
             np.array([self.x, self.y, self.score])
             if self.visible
             else np.full((3,), np.nan)
         )
 
     def __eq__(self, other: object):
-        """Compare `self` and `other` for equality
+        """Compare `self` and `other` for equality.
 
         See `Point.__eq__()` for important notes about point equality semantics!
 
         Args:
             self, other: instance of `PredictedPoint` to compare
 
         Returns:
-            True if all attributes of `self` and `other` are the identical (possibly allowing
-            precision error for `x` and `y` attributes).
+            True if all attributes of `self` and `other` are the identical (possibly
+            allowing precision error for `x` and `y` attributes).
         """
         if not super().__eq__(other):
             return False
 
         # we know that we have a point at this point
         other = cast(PredictedPoint, other)
 
@@ -146,15 +149,15 @@
     name: str = ""
 
 
 def _compare_points(
     a: Union[dict[Node, Point], dict[Node, PredictedPoint]],
     b: Union[dict[Node, Point], dict[Node, PredictedPoint]],
 ) -> bool:
-    """Compare two sets of points for equality
+    """Compare two sets of points for equality.
 
     To satisfy equaity, the two set of points must:
         1) each contain the same set of `Nodes`
         2) for each node, the two `Point`s must satisfy normal `Point` equality
 
     Args:
         a: collection of points
@@ -201,15 +204,15 @@
 
     _POINT_TYPE = Point
 
     def _make_default_point(self, x, y):
         return self._POINT_TYPE(x, y, visible=not (math.isnan(x) or math.isnan(y)))
 
     def _convert_points(self, attr, points):
-        """Callback for maintaining points mappings between nodes and points."""
+        """Maintain points mappings between nodes and points."""
         if type(points) == np.ndarray:
             points = points.tolist()
 
         if type(points) == list:
             if len(points) != len(self.skeleton):
                 raise ValueError(
                     "If specifying points as a list, must provide as many points as "
@@ -361,14 +364,16 @@
             points=node_points,
             skeleton=skeleton,
             score=instance_score,
             tracking_score=tracking_score,
             track=track,
         )
 
-    def numpy(self) -> np.ndarray:
+    def numpy(self, scores: bool = False) -> np.ndarray:
         """Return the instance points as a numpy array."""
         pts = np.full((len(self.skeleton), 3), np.nan)
         for node, point in self.points.items():
             if point.visible:
                 pts[self.skeleton.index(node)] = point.numpy()
+        if not scores:
+            pts = pts[:, :2]
         return pts
```

## sleap_io/model/labeled_frame.py

```diff
@@ -57,7 +57,12 @@
         """
         n_instances = len(self.instances)
         n_nodes = len(self.instances[0]) if n_instances > 0 else 0
         pts = np.full((n_instances, n_nodes, 2), np.nan)
         for i, inst in enumerate(self.instances):
             pts[i] = inst.numpy()[:, 0:2]
         return pts
+
+    @property
+    def image(self) -> np.ndarray:
+        """Return the image of the frame as a numpy array."""
+        return self.video[self.frame_idx]
```

## sleap_io/model/labels.py

```diff
@@ -160,23 +160,19 @@
             tracks = np.full((n_frames, n_tracks, n_nodes, 3), np.nan, dtype="float32")
         else:
             tracks = np.full((n_frames, n_tracks, n_nodes, 2), np.nan, dtype="float32")
         for lf in lfs:
             i = int(lf.frame_idx - first_frame)
             if untracked:
                 for j, inst in enumerate(lf.predicted_instances):
-                    tracks[i, j] = (
-                        inst.numpy() if return_confidence else inst.numpy()[:, 0:2]
-                    )
+                    tracks[i, j] = inst.numpy(scores=return_confidence)
             else:
                 tracked_instances = [
                     inst
                     for inst in lf.instances
                     if type(inst) == PredictedInstance and inst.track is not None
                 ]
                 for inst in tracked_instances:
                     j = self.tracks.index(inst.track)  # type: ignore[arg-type]
-                    tracks[i, j] = (
-                        inst.numpy() if return_confidence else inst.numpy()[:, 0:2]
-                    )
+                    tracks[i, j] = inst.numpy(scores=return_confidence)
 
         return tracks
```

## sleap_io/model/video.py

```diff
@@ -2,28 +2,124 @@
 
 The `Video` class is a SLEAP data structure that stores information regarding
 a video and its components used in SLEAP.
 """
 
 from __future__ import annotations
 from attrs import define
-from typing import Any, Tuple, Optional
+from typing import Tuple, Optional, Optional
+import numpy as np
+from sleap_io.io.video import VideoBackend
 
 
-@define(auto_attribs=True)
+@define
 class Video:
     """`Video` class used by sleap to represent videos and data associated with them.
 
     This class is used to store information regarding a video and its components.
     It is used to store the video's `filename`, `shape`, and the video's `backend`.
 
+    To create a `Video` object, use the `from_filename` method which will select the
+    backend appropriately.
+
     Args:
         filename: The filename of the video.
-        shape: The shape of the video. In the format: (frames, height, width, channels).
         backend: An object that implements the basic methods for reading and
             manipulating frames of a specific video type.
 
+    See also: VideoBackend
     """
 
     filename: str
-    shape: Optional[Tuple[int, int, int, int]] = None
-    backend: Any = None
+    backend: Optional[VideoBackend] = None
+
+    @classmethod
+    def from_filename(
+        cls,
+        filename: str,
+        dataset: Optional[str] = None,
+        grayscale: Optional[str] = None,
+        **kwargs,
+    ) -> VideoBackend:
+        """Create a Video from a filename.
+
+        Args:
+            filename: Path to video file.
+            dataset: Name of dataset in HDF5 file.
+            grayscale: Whether to force grayscale. If None, autodetect on first frame
+                load.
+
+        Returns:
+            Video instance with the appropriate backend instantiated.
+        """
+        return cls(
+            filename=filename,
+            backend=VideoBackend.from_filename(
+                filename, dataset=dataset, grayscale=grayscale, **kwargs
+            ),
+        )
+
+    @property
+    def shape(self) -> Tuple[int, int, int, int] | None:
+        """Return the shape of the video as (num_frames, height, width, channels).
+
+        If the video backend is not set or it cannot determine the shape of the video,
+        this will return None.
+        """
+        return self._get_shape()
+
+    def _get_shape(self) -> Tuple[int, int, int, int] | None:
+        """Return the shape of the video as (num_frames, height, width, channels).
+
+        This suppresses errors related to querying the backend for the video shape, such
+        as when it has not been set or when the video file is not found.
+        """
+        try:
+            return self.backend.shape
+        except:
+            return None
+
+    def __len__(self) -> int:
+        """Return the length of the video as the number of frames."""
+        shape = self.shape
+        return 0 if shape is None else shape[0]
+
+    def __repr__(self) -> str:
+        """Informal string representation (for print or format)."""
+        dataset = (
+            f"dataset={self.backend.dataset}, "
+            if getattr(self.backend, "dataset", "")
+            else ""
+        )
+        return (
+            "Video("
+            f'filename="{self.filename}", '
+            f"shape={self.shape}, "
+            f"{dataset}"
+            f"backend={type(self.backend).__name__}"
+            ")"
+        )
+
+    def __str__(self) -> str:
+        """Informal string representation (for print or format)."""
+        return self.__repr__()
+
+    def __getitem__(self, inds: int | list[int] | slice) -> np.ndarray:
+        """Return the frames of the video at the given indices.
+
+        Args:
+            ind: Index or list of indices of frames to read.
+
+        Returns:
+            Frame or frames as a numpy array of shape `(height, width, channels)` if a
+            scalar index is provided, or `(frames, height, width, channels)` if a list
+            of indices is provided.
+
+        See also: VideoBackend.get_frame, VideoBackend.get_frames
+        """
+        if self.backend is None:
+            raise ValueError(
+                "Video backend is not set. "
+                "This may be because the video reader could not be determined "
+                "automatically from the filename."
+            )
+        return self.backend[inds]
```

## Comparing `sleap_io-0.0.2.dist-info/LICENSE` & `sleap_io-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

