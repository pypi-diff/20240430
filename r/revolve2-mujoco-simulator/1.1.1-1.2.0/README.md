# Comparing `tmp/revolve2_mujoco_simulator-1.1.1-py3-none-any.whl.zip` & `tmp/revolve2_mujoco_simulator-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,24 @@
-Zip file size: 22026 bytes, number of entries: 19
+Zip file size: 25064 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      118 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/__init__.py
 -rw-r--r--  2.0 unx     1340 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_abstraction_to_mujoco_mapping.py
 -rw-r--r--  2.0 unx     1598 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_control_interface_impl.py
--rw-r--r--  2.0 unx     8088 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_custom_mujoco_viewer.py
--rw-r--r--  2.0 unx     4703 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_local_simulator.py
--rw-r--r--  2.0 unx     4220 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_open_gl_vision.py
--rw-r--r--  2.0 unx      162 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_render_backend.py
+-rw-r--r--  2.0 unx     5224 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_local_simulator.py
+-rw-r--r--  2.0 unx     4377 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_open_gl_vision.py
+-rw-r--r--  2.0 unx      167 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_render_backend.py
 -rw-r--r--  2.0 unx    16964 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_scene_to_model.py
--rw-r--r--  2.0 unx     3314 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_simulate_manual_scene.py
--rw-r--r--  2.0 unx     6912 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_simulate_scene.py
+-rw-r--r--  2.0 unx     3307 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_simulate_manual_scene.py
+-rw-r--r--  2.0 unx     8416 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_simulate_scene.py
 -rw-r--r--  2.0 unx     4727 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_simulation_state_impl.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/py.typed
 -rw-r--r--  2.0 unx      162 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/textures/__init__.py
 -rw-r--r--  2.0 unx      507 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/textures/_checker.py
 -rw-r--r--  2.0 unx      414 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/textures/_flat.py
 -rw-r--r--  2.0 unx      462 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/textures/_gradient.py
--rw-r--r--  2.0 unx     3265 b- defN 80-Jan-01 00:00 revolve2_mujoco_simulator-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 revolve2_mujoco_simulator-1.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2077 b- defN 16-Jan-01 00:00 revolve2_mujoco_simulator-1.1.1.dist-info/RECORD
-19 files, 59121 bytes uncompressed, 18444 bytes compressed:  68.8%
+-rw-r--r--  2.0 unx      345 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/viewers/__init__.py
+-rw-r--r--  2.0 unx     9487 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/viewers/_custom_mujoco_viewer.py
+-rw-r--r--  2.0 unx     2379 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/viewers/_native_mujoco_viewer.py
+-rw-r--r--  2.0 unx      729 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/viewers/_viewer_type.py
+-rw-r--r--  2.0 unx     3278 b- defN 80-Jan-01 00:00 revolve2_mujoco_simulator-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 revolve2_mujoco_simulator-1.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2439 b- defN 16-Jan-01 00:00 revolve2_mujoco_simulator-1.2.0.dist-info/RECORD
+22 files, 66528 bytes uncompressed, 20868 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -3,17 +3,14 @@
 
 Filename: revolve2/simulators/mujoco_simulator/_abstraction_to_mujoco_mapping.py
 Comment: 
 
 Filename: revolve2/simulators/mujoco_simulator/_control_interface_impl.py
 Comment: 
 
-Filename: revolve2/simulators/mujoco_simulator/_custom_mujoco_viewer.py
-Comment: 
-
 Filename: revolve2/simulators/mujoco_simulator/_local_simulator.py
 Comment: 
 
 Filename: revolve2/simulators/mujoco_simulator/_open_gl_vision.py
 Comment: 
 
 Filename: revolve2/simulators/mujoco_simulator/_render_backend.py
@@ -42,17 +39,29 @@
 
 Filename: revolve2/simulators/mujoco_simulator/textures/_flat.py
 Comment: 
 
 Filename: revolve2/simulators/mujoco_simulator/textures/_gradient.py
 Comment: 
 
-Filename: revolve2_mujoco_simulator-1.1.1.dist-info/METADATA
+Filename: revolve2/simulators/mujoco_simulator/viewers/__init__.py
+Comment: 
+
+Filename: revolve2/simulators/mujoco_simulator/viewers/_custom_mujoco_viewer.py
+Comment: 
+
+Filename: revolve2/simulators/mujoco_simulator/viewers/_native_mujoco_viewer.py
+Comment: 
+
+Filename: revolve2/simulators/mujoco_simulator/viewers/_viewer_type.py
+Comment: 
+
+Filename: revolve2_mujoco_simulator-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: revolve2_mujoco_simulator-1.1.1.dist-info/WHEEL
+Filename: revolve2_mujoco_simulator-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: revolve2_mujoco_simulator-1.1.1.dist-info/RECORD
+Filename: revolve2_mujoco_simulator-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## revolve2/simulators/mujoco_simulator/_local_simulator.py

```diff
@@ -3,44 +3,48 @@
 import os
 
 from revolve2.simulation.scene import SimulationState
 from revolve2.simulation.simulator import Batch, Simulator
 
 from ._simulate_manual_scene import simulate_manual_scene
 from ._simulate_scene import simulate_scene
+from .viewers import ViewerType
 
 
 class LocalSimulator(Simulator):
     """Simulator using MuJoCo."""
 
     _headless: bool
     _start_paused: bool
     _num_simulators: int
     _cast_shadows: bool
     _fast_sim: bool
     _manual_control: bool
+    _viewer_type: ViewerType
 
     def __init__(
         self,
         headless: bool = False,
         start_paused: bool = False,
         num_simulators: int = 1,
         cast_shadows: bool = False,
         fast_sim: bool = False,
         manual_control: bool = False,
+        viewer_type: ViewerType | str = ViewerType.CUSTOM,
     ):
         """
         Initialize this object.
 
         :param headless: If True, the simulation will not be rendered. This drastically improves performance.
         :param start_paused: If True, start the simulation paused. Only possible when not in headless mode.
         :param num_simulators: The number of simulators to deploy in parallel. They will take one core each but will share space on the main python thread for calculating control.
         :param cast_shadows: Whether shadows are cast in the simulation.
         :param fast_sim: Whether more complex rendering prohibited.
         :param manual_control: Whether the simulation should be controlled manually.
+        :param viewer_type: The viewer-implementation to use in the local simulator.
         """
         assert (
             headless or num_simulators == 1
         ), "Cannot have parallel simulators when visualizing."
 
         assert not (
             headless and start_paused
@@ -48,14 +52,19 @@
 
         self._headless = headless
         self._start_paused = start_paused
         self._num_simulators = num_simulators
         self._cast_shadows = cast_shadows
         self._fast_sim = fast_sim
         self._manual_control = manual_control
+        self._viewer_type = (
+            ViewerType.from_string(viewer_type)
+            if isinstance(viewer_type, str)
+            else viewer_type
+        )
 
     def simulate_batch(self, batch: Batch) -> list[list[SimulationState]]:
         """
         Simulate the provided batch by simulating each contained scene.
 
         :param batch: The batch to run.
         :returns: List of simulation states in ascending order of time.
@@ -67,15 +76,18 @@
         sample_step = (
             None
             if batch.parameters.sampling_frequency is None
             else 1.0 / batch.parameters.sampling_frequency
         )
 
         if batch.record_settings is not None:
-            os.makedirs(batch.record_settings.video_directory, exist_ok=False)
+            os.makedirs(
+                batch.record_settings.video_directory,
+                exist_ok=batch.record_settings.overwrite,
+            )
 
         if self._manual_control:
             if self._headless:
                 raise Exception("Manual control only works with rendered simulations.")
             for scene in batch.scenes:
                 simulate_manual_scene(scene=scene)
             return [[]]
@@ -94,14 +106,15 @@
                         self._start_paused,
                         control_step,
                         sample_step,
                         batch.parameters.simulation_time,
                         batch.parameters.simulation_timestep,
                         self._cast_shadows,
                         self._fast_sim,
+                        self._viewer_type,
                     )
                     for scene_index, scene in enumerate(batch.scenes)
                 ]
                 results = [future.result() for future in futures]
         else:
             results = [
                 simulate_scene(
@@ -112,14 +125,15 @@
                     self._start_paused,
                     control_step,
                     sample_step,
                     batch.parameters.simulation_time,
                     batch.parameters.simulation_timestep,
                     self._cast_shadows,
                     self._fast_sim,
+                    self._viewer_type,
                 )
                 for scene_index, scene in enumerate(batch.scenes)
             ]
 
         logging.info("Finished batch.")
 
         return results
```

## revolve2/simulators/mujoco_simulator/_open_gl_vision.py

```diff
@@ -8,15 +8,20 @@
 from numpy.typing import NDArray
 
 from ._abstraction_to_mujoco_mapping import CameraSensorMujoco
 from ._render_backend import RenderBackend
 
 
 class OpenGLVision:
-    """A class to enable vision / camera sensors using OpenGl."""
+    """
+    A class to enable vision / camera sensors using OpenGl.
+
+    This Class is based on an implementation of Kevin Godin-Dubois <k.j.m.godin-dubois@vu.nl>.
+    Thank you very much for this big contribution!
+    """
 
     _open_gl_context: Any
 
     _mujoco_context: mujoco.MjrContext
     _mujoco_scene: mujoco.MjvScene
 
     _camera: mujoco.MjvCamera
```

## revolve2/simulators/mujoco_simulator/_render_backend.py

```diff
@@ -1,9 +1,9 @@
-from enum import Enum
+from enum import Enum, auto
 
 
 class RenderBackend(Enum):
     """Enumerator for rendering backend libraries."""
 
-    GLFW = "glfw"
-    EGL = "egl"
-    OSMESA = "osmesa"
+    GLFW = auto()
+    EGL = auto()
+    OSMESA = auto()
```

## revolve2/simulators/mujoco_simulator/_simulate_manual_scene.py

```diff
@@ -7,18 +7,18 @@
 from revolve2.ci_group.simulation_parameters import (
     STANDARD_CONTROL_FREQUENCY,
     STANDARD_SIMULATION_TIMESTEP,
 )
 from revolve2.simulation.scene import Scene
 
 from ._control_interface_impl import ControlInterfaceImpl
-from ._custom_mujoco_viewer import CustomMujocoViewer, CustomMujocoViewerMode
 from ._render_backend import RenderBackend
 from ._scene_to_model import scene_to_model
 from ._simulation_state_impl import SimulationStateImpl
+from .viewers import CustomMujocoViewer, CustomMujocoViewerMode
 
 
 def simulate_manual_scene(
     scene: Scene,
     render_backend: RenderBackend = RenderBackend.GLFW,
 ) -> None:
     """
@@ -90,9 +90,9 @@
                 prev_position = position
                 target = positions[prev_position]
 
     except KeyboardInterrupt:
         """If we press ctrl-C this script will end with the finally clause."""
         pass
     finally:
-        viewer.close()
+        viewer.close_viewer()
         logging.info("Testing done.")
```

## revolve2/simulators/mujoco_simulator/_simulate_scene.py

```diff
@@ -6,33 +6,34 @@
 import numpy as np
 import numpy.typing as npt
 
 from revolve2.simulation.scene import Scene, SimulationState
 from revolve2.simulation.simulator import RecordSettings
 
 from ._control_interface_impl import ControlInterfaceImpl
-from ._custom_mujoco_viewer import CustomMujocoViewer
 from ._open_gl_vision import OpenGLVision
 from ._render_backend import RenderBackend
 from ._scene_to_model import scene_to_model
 from ._simulation_state_impl import SimulationStateImpl
+from .viewers import CustomMujocoViewer, NativeMujocoViewer, ViewerType
 
 
 def simulate_scene(
     scene_id: int,
     scene: Scene,
     headless: bool,
     record_settings: RecordSettings | None,
     start_paused: bool,
     control_step: float,
     sample_step: float | None,
     simulation_time: int | None,
     simulation_timestep: float,
     cast_shadows: bool,
     fast_sim: bool,
+    viewer_type: ViewerType,
     render_backend: RenderBackend = RenderBackend.EGL,
 ) -> list[SimulationState]:
     """
     Simulate a scene.
 
     :param scene_id: An id for this scene, unique between all scenes ran in parallel.
     :param scene: The scene to simulate.
@@ -41,82 +42,110 @@
     :param start_paused: If true, the simulation will start in a paused state. Only makessense when headless is False.
     :param control_step: The time between each call to the handle function of the scene handler. In seconds.
     :param sample_step: The time between each state sample of the simulation. In seconds.
     :param simulation_time: How long to simulate for. In seconds.
     :param simulation_timestep: The duration to integrate over during each step of the simulation. In seconds.
     :param cast_shadows: If shadows are cast.
     :param fast_sim: If fancy rendering is disabled.
+    :param viewer_type: The type of viewer used for the rendering in a window.
     :param render_backend: The backend to be used for rendering (EGL by default and switches to GLFW if no cameras are on the robot).
     :returns: The results of simulation. The number of returned states depends on `sample_step`.
+    :raises ValueError: If the viewer is not able to record.
     """
     logging.info(f"Simulating scene {scene_id}")
 
+    """Define mujoco data and model objects for simuating."""
     model, mapping = scene_to_model(
         scene, simulation_timestep, cast_shadows=cast_shadows, fast_sim=fast_sim
     )
+    data = mujoco.MjData(model)
+
+    """Define a control interface for the mujoco simulation (used to control robots)."""
+    control_interface = ControlInterfaceImpl(
+        data=data, abstraction_to_mujoco_mapping=mapping
+    )
+    """Make separate viewer for camera sensors."""
+    camera_viewers = {
+        camera.camera_id: OpenGLVision(
+            model=model, camera=camera, headless=headless, open_gl_lib=render_backend
+        )
+        for camera in mapping.camera_sensor.values()
+    }
+
+    """Define some additional control variables."""
+    last_control_time = 0.0
+    last_sample_time = 0.0
+    last_video_time = 0.0  # time at which last video frame was saved
+
+    simulation_states: list[SimulationState] = (
+        []
+    )  # The measured states of the simulation
 
     """If we dont have cameras and the backend is not set we go to the default GLFW."""
     if len(mapping.camera_sensor.values()) == 0:
         render_backend = RenderBackend.GLFW
-    data = mujoco.MjData(model)
 
+    """Initialize viewer object if we need to render the scene."""
     if not headless or record_settings is not None:
-        viewer = CustomMujocoViewer(
+        match viewer_type:
+            case viewer_type.CUSTOM:
+                viewer = CustomMujocoViewer
+            case viewer_type.NATIVE:
+                viewer = NativeMujocoViewer
+            case _:
+                raise ValueError(
+                    f"Viewer of type {viewer_type} not defined in _simulate_scene."
+                )
+
+        viewer = viewer(
             model,
             data,
+            width=None if record_settings is None else record_settings.width,
+            height=None if record_settings is None else record_settings.height,
             backend=render_backend,
             start_paused=start_paused,
             render_every_frame=False,
+            hide_menus=(record_settings is not None),
         )
-    camera_viewers = {
-        camera.camera_id: OpenGLVision(
-            model=model, camera=camera, headless=headless, open_gl_lib=render_backend
-        )
-        for camera in mapping.camera_sensor.values()
-    }
 
+    """Record the scene if we want to record."""
     if record_settings is not None:
+        if not viewer.can_record:
+            raise ValueError(
+                f"Selected Viewer {type(viewer).__name__} has no functionality to record."
+            )
         video_step = 1 / record_settings.fps
         video_file_path = f"{record_settings.video_directory}/{scene_id}.mp4"
         fourcc = cv2.VideoWriter.fourcc(*"mp4v")
         video = cv2.VideoWriter(
             video_file_path,
             fourcc,
             record_settings.fps,
-            (viewer.viewport.width, viewer.viewport.height),
+            viewer.current_viewport_size(),
         )
 
-        viewer._hide_menu = True
-
-    last_control_time = 0.0
-    last_sample_time = 0.0
-    last_video_time = 0.0  # time at which last video frame was saved
-
-    # The measured states of the simulation
-    simulation_states: list[SimulationState] = []
-
-    # Compute forward dynamics without actually stepping forward in time.
-    # This updates the data so we can read out the initial state.
+    """
+    Compute forward dynamics without actually stepping forward in time.
+    This updates the data so we can read out the initial state.
+    """
     mujoco.mj_forward(model, data)
     images = {
         camera_id: camera_viewer.process(model, data)
         for camera_id, camera_viewer in camera_viewers.items()
     }
 
     # Sample initial state.
     if sample_step is not None:
         simulation_states.append(
             SimulationStateImpl(
                 data=data, abstraction_to_mujoco_mapping=mapping, camera_views=images
             )
         )
 
-    control_interface = ControlInterfaceImpl(
-        data=data, abstraction_to_mujoco_mapping=mapping
-    )
+    """After rendering the initial state, we enter the rendering loop."""
     while (time := data.time) < (
         float("inf") if simulation_time is None else simulation_time
     ):
 
         # do control if it is time
         if time >= last_control_time + control_step:
             last_control_time = math.floor(time / control_step) * control_step
@@ -136,14 +165,15 @@
                         abstraction_to_mujoco_mapping=mapping,
                         camera_views=images,
                     )
                 )
 
         # step simulation
         mujoco.mj_step(model, data)
+        # extract images from camera sensors.
         images = {
             camera_id: camera_viewer.process(model, data)
             for camera_id, camera_viewer in camera_viewers.items()
         }
 
         # render if not headless. also render when recording and if it time for a new video frame.
         if not headless or (
@@ -153,37 +183,38 @@
 
         # capture video frame if it's time
         if record_settings is not None and time >= last_video_time + video_step:
             last_video_time = int(time / video_step) * video_step
 
             # https://github.com/deepmind/mujoco/issues/285 (see also record.cc)
             img: npt.NDArray[np.uint8] = np.empty(
-                (viewer.viewport.height, viewer.viewport.width, 3),
+                (*viewer.current_viewport_size(), 3),
                 dtype=np.uint8,
             )
 
             mujoco.mjr_readPixels(
                 rgb=img,
                 depth=None,
-                viewport=viewer.viewport,
-                con=viewer.ctx,
+                viewport=viewer.view_port,
+                con=viewer.context,
             )
-            img = np.flip(img, axis=0)  # img is upside down initially
+            # Flip the image and map to OpenCV colormap (BGR -> RGB)
+            img = np.flipud(img)[:, :, ::-1]
             video.write(img)
 
+    """Once simulation is done we close the potential viewer and release the potential video."""
     if not headless or record_settings is not None:
-        viewer.close()
+        viewer.close_viewer()
 
     if record_settings is not None:
         video.release()
 
     # Sample one final time.
     if sample_step is not None:
         simulation_states.append(
             SimulationStateImpl(
                 data=data, abstraction_to_mujoco_mapping=mapping, camera_views=images
             )
         )
 
     logging.info(f"Scene {scene_id} done.")
-
     return simulation_states
```

## Comparing `revolve2/simulators/mujoco_simulator/_custom_mujoco_viewer.py` & `revolve2/simulators/mujoco_simulator/viewers/_custom_mujoco_viewer.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 from enum import Enum
 from typing import Any
 
 import glfw
 import mujoco
 import mujoco_viewer
 
-from ._render_backend import RenderBackend
+from revolve2.simulation.simulator import Viewer
+
+from .._render_backend import RenderBackend
 
 
 class CustomMujocoViewerMode(Enum):
     """
     Enumerate different viewer modes for the CustomMujocoViewer.
 
     - CLASSIC mode gives an informative interface for regular simulations.
     - MANUAL mode gives a cut down interface, specific for targeting robot movement manually.
     """
 
     CLASSIC = "classic"
     MANUAL = "manual"
 
 
-class CustomMujocoViewer(mujoco_viewer.MujocoViewer):  # type: ignore
+class CustomMujocoViewer(Viewer, mujoco_viewer.MujocoViewer):  # type: ignore
     """
     Custom Viewer Object that allows for additional keyboard inputs.
 
     We need the type ignore since the mujoco_viewer library is not typed properly and therefor the MujocoViewer class cant be resolved.
     """
 
     _convex_hull_rendering: bool
@@ -42,45 +44,54 @@
     _advance_by_one_step: bool
     _position: int
 
     def __init__(
         self,
         model: mujoco.MjModel,
         data: mujoco.MjData,
+        *,
         backend: RenderBackend,
+        width: int | None = None,
+        height: int | None = None,
         start_paused: bool = False,
         render_every_frame: bool = False,
+        hide_menus: bool = False,
         mode: CustomMujocoViewerMode = CustomMujocoViewerMode.CLASSIC,
+        **_: Any,
     ):
         """
         Initialize the Viewer.
 
         :param model: The mujoco models.
         :param data: The mujoco data.
         :param backend: The backend for rendering.
+        :param width: The width of the viewer (optional, defaults to screen width)
+        :param height: The height of the viewer (optional, defaults to screen height)
         :param start_paused: If the simulation starts paused or not.
         :param render_every_frame: If every frame is rendered or not.
+        :param hide_menus: Start with hidden menus?
         :param mode: The mode of the viewer (classic, manual).
+        :param _: Some unused kwargs.
         """
         match backend:
             case RenderBackend.EGL:
                 glfw.window_hint(glfw.CONTEXT_CREATION_API, glfw.EGL_CONTEXT_API)
             case RenderBackend.OSMESA:
                 glfw.window_hint(glfw.CONTEXT_CREATION_API, glfw.OSMESA_CONTEXT_API)
             case _:  # By default, we are using GLFW.
                 pass
 
         super().__init__(
             model,
             data,
             mode="window",
             title="custom-mujoco-viewer",
-            width=None,
-            height=None,
-            hide_menus=False,
+            width=width,
+            height=height,
+            hide_menus=hide_menus,
         )
 
         self._viewer_mode = mode
         self._position = 0
         self._paused = start_paused
         self._mujoco_version = tuple(map(int, mujoco.__version__.split(".")))
         self._render_every_frame = render_every_frame
@@ -212,21 +223,63 @@
         else:
             match key:
                 case glfw.KEY_K:  # Increment cycle position
                     self._increment_position()
                 case _:
                     pass
 
+    def current_viewport_size(self) -> tuple[int, int]:
+        """
+        Grabs the *current* viewport size (and updates the cached values).
+
+        :return: the viewport size
+        """
+        self.viewport.width, self.viewport.height = glfw.get_framebuffer_size(
+            self.window
+        )
+        return self.viewport.width, self.viewport.height
+
     def render(self) -> int | None:
         """
         Render the scene.
 
         :return: A cycle position if applicable.
         """
         super().render()
-        if self._viewer_mode.value == "manual":
+        if self._viewer_mode == CustomMujocoViewerMode.MANUAL:
             return self._position
         return None
 
     def _increment_position(self) -> None:
         """Increment our cycle position."""
         self._position = (self._position + 1) % 5
+
+    def close_viewer(self) -> None:
+        """Close the viewer."""
+        self.close()
+
+    @property
+    def context(self) -> mujoco.MjrContext:
+        """
+        Get the context.
+
+        :returns: The context.
+        """
+        return self.ctx
+
+    @property
+    def view_port(self) -> mujoco.MjrRect:
+        """
+        Get the view_port.
+
+        :returns: The viewport.
+        """
+        return self.viewport
+
+    @property
+    def can_record(self) -> bool:
+        """
+        Return True.
+
+        :returns: True.
+        """
+        return True
```

## Comparing `revolve2_mujoco_simulator-1.1.1.dist-info/METADATA` & `revolve2_mujoco_simulator-1.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: revolve2-mujoco-simulator
-Version: 1.1.1
+Version: 1.2.0
 Summary: Revolve2: MuJoCo simulator.
 Home-page: https://github.com/ci-group/revolve2
 Author: Aart Stuurman
 Author-email: aartstuurman@hotmail.com
 Requires-Python: >=3.10,<3.12
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Provides-Extra: dev
 Requires-Dist: dm-control (>=1.0.3,<2.0.0)
 Requires-Dist: mujoco (>=2.2.0,<3.0.0)
 Requires-Dist: mujoco-python-viewer (>=0.1.3,<0.2.0)
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0)
-Requires-Dist: revolve2-simulation (==1.1.1)
+Requires-Dist: revolve2-simulation (==1.2.0)
 Project-URL: Repository, https://github.com/ci-group/revolve2
 Description-Content-Type: text/markdown
 
 <img align="right" width="150" height="150"  src="./docs/source/logo_light.png">
 
 # Revolve2
```

## Comparing `revolve2_mujoco_simulator-1.1.1.dist-info/RECORD` & `revolve2_mujoco_simulator-1.2.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 revolve2/simulators/mujoco_simulator/__init__.py,sha256=KKu1kVyrG86GveMs8QMCQ-3zj2dTBM6z1rTeDRa2Exw,118
 revolve2/simulators/mujoco_simulator/_abstraction_to_mujoco_mapping.py,sha256=JO-7pw5znDwTpD68D4-tr9srBAURHgLxWuL_etYMyLs,1340
 revolve2/simulators/mujoco_simulator/_control_interface_impl.py,sha256=l_ItaWGmR5bNVWIcIbAYQwNZ2ph-sSuFrkP65cJQ4Oc,1598
-revolve2/simulators/mujoco_simulator/_custom_mujoco_viewer.py,sha256=3JfrEyPZxq9LarJhPcDeyOSYxUp1lHH_DLJg5uDop9A,8088
-revolve2/simulators/mujoco_simulator/_local_simulator.py,sha256=2BOhtVbsgSTqwzQZW-fF6ABRAgqa-CYt_Ugzxh6-Pn0,4703
-revolve2/simulators/mujoco_simulator/_open_gl_vision.py,sha256=cU2ormlCrKXS8ZKQm6hey5qYGKsMfDyEQwa9E6yVJfM,4220
-revolve2/simulators/mujoco_simulator/_render_backend.py,sha256=XscUnbywbJueXsaLCfjvtykZX0l-8aJwSRFLYDeebjk,162
+revolve2/simulators/mujoco_simulator/_local_simulator.py,sha256=uLQm0WwQKf-mTkh6d4NyX1mTDEy53vPoCy7Pg44D3oc,5224
+revolve2/simulators/mujoco_simulator/_open_gl_vision.py,sha256=-tV5bs6TSHT3TN0qj5qHHYYi0zq7timSXvvGrAu9hag,4377
+revolve2/simulators/mujoco_simulator/_render_backend.py,sha256=HOSE5aYjMwo7C328SV7modbQFM1lCBS1tUSC9RKpS7s,167
 revolve2/simulators/mujoco_simulator/_scene_to_model.py,sha256=E25z38KyxEya4fhlrbXeMBgIXgOORFApeoxATn2PrHY,16964
-revolve2/simulators/mujoco_simulator/_simulate_manual_scene.py,sha256=s0C5QezPsTJgzBfPTRlkAB9A0w0oK5T-yBp4TAr3r1w,3314
-revolve2/simulators/mujoco_simulator/_simulate_scene.py,sha256=ETM9uHZYDayhP3rLQOZcLIvhfKiTjt2-TDT4_TaSSv8,6912
+revolve2/simulators/mujoco_simulator/_simulate_manual_scene.py,sha256=exFsSK2EMik0WXmdXnuBusPpX3Nk1vvGfi2kg5cQxSo,3307
+revolve2/simulators/mujoco_simulator/_simulate_scene.py,sha256=cpX0GhUc2wQewvY5U5TTEhxesYEd8qUnTDQYKszE5wU,8416
 revolve2/simulators/mujoco_simulator/_simulation_state_impl.py,sha256=3m_C9LLlk5fgCP2OtD9r9Rv8NVO1DXbciR8S6jrnejg,4727
 revolve2/simulators/mujoco_simulator/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 revolve2/simulators/mujoco_simulator/textures/__init__.py,sha256=yU3N9CwuuZHeNigXmrxQvsY7ExoBhZHt7p6_-awbiZ0,162
 revolve2/simulators/mujoco_simulator/textures/_checker.py,sha256=gICg92sSTKuKg3wupPQGIMZlshi4rqiPCIj6L301N94,507
 revolve2/simulators/mujoco_simulator/textures/_flat.py,sha256=rZ55XG5sAjvrauKRXW82SPZ70X-qI5SPhyb99ToRdOQ,414
 revolve2/simulators/mujoco_simulator/textures/_gradient.py,sha256=utAbc4U9p0BMJEKNzCuBZJigqZ_d8MMTU8xOytS2sHQ,462
-revolve2_mujoco_simulator-1.1.1.dist-info/METADATA,sha256=KEhcNYW9-XEeblgoyy95MUpSA4zCdjGi86psWqpQx88,3265
-revolve2_mujoco_simulator-1.1.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-revolve2_mujoco_simulator-1.1.1.dist-info/RECORD,,
+revolve2/simulators/mujoco_simulator/viewers/__init__.py,sha256=WIOIu10ERLeWSFVmwdBZBHLi9hpwZw6gYcEFbNENsi0,345
+revolve2/simulators/mujoco_simulator/viewers/_custom_mujoco_viewer.py,sha256=K7VhcM-E5bMAHAImHo9Vl4RcLwDPGEU2YOy0_70etVY,9487
+revolve2/simulators/mujoco_simulator/viewers/_native_mujoco_viewer.py,sha256=yP7ueqebcaarlrBJadVWTrmZg2GHwcupOGCM1-lm-6s,2379
+revolve2/simulators/mujoco_simulator/viewers/_viewer_type.py,sha256=AgsewIA3KDPINxVh7wVPVVAo7P6_1M9yxTINKqFVFpo,729
+revolve2_mujoco_simulator-1.2.0.dist-info/METADATA,sha256=aQEoxUIpg0zGhp8ctvRp_tCj_IcmreOI03G7C-vUlPo,3278
+revolve2_mujoco_simulator-1.2.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+revolve2_mujoco_simulator-1.2.0.dist-info/RECORD,,
```

