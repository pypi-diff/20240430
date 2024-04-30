# Comparing `tmp/midiscripter-0.1.2.tar.gz` & `tmp/midiscripter-0.1.3.tar.gz`

## Comparing `midiscripter-0.1.2.tar` & `midiscripter-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/base/__init__.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/base/msg_base.py
--rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/base/port_base.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/base/shared.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/cli/__init__.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/cli/starters.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/file_event/__init__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/file_event/file_event_msg.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/file_event/file_event_port.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/__init__.py
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/app.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/log_widget.py
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/main_window.py
--rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/menu_bar.py
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/ports_widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/__init__.py
--rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/button.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/gui_msg.py
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/gui_widget_base.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/layout.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/list.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/mixins.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/gui/gui_widgets/text.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/keyboard/__init__.py
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/keyboard/keyboard_msg.py
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/keyboard/keyboard_port.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/logger/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/logger/console_sink.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/logger/html_sink.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/logger/log.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/metronome/__init__.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/metronome/metronome_port.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/midi/__init__.py
--rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/midi/midi_msg.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/midi/midi_note_data.py
--rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/midi/midi_port.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/midi/midi_ports_update.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/osc/__init__.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/osc/osc_msg.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/osc/osc_port.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/osc/osc_query_maker.py
--rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/resources/icon.ico
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 midiscripter-0.1.2/midiscripter/resources/icon.svg
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 midiscripter-0.1.2/LICENSE
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 midiscripter-0.1.2/README.md
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 midiscripter-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    13761 2020-02-02 00:00:00.000000 midiscripter-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/base/__init__.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/base/msg_base.py
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/base/port_base.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/base/shared.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/cli/__init__.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/cli/starters.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/file_event/__init__.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/file_event/file_event_msg.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/file_event/file_event_port.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/__init__.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/app.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/log_widget.py
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/main_window.py
+-rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/menu_bar.py
+-rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/ports_widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/gui_widgets/__init__.py
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/gui_widgets/button.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/gui_widgets/gui_msg.py
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/gui_widgets/gui_widget_base.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/gui_widgets/layout.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/gui_widgets/list.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/gui_widgets/mixins.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/gui/gui_widgets/text.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/keyboard/__init__.py
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/keyboard/keyboard_msg.py
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/keyboard/keyboard_port.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/logger/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/logger/console_sink.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/logger/html_sink.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/logger/log.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/metronome/__init__.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/metronome/metronome_port.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/midi/__init__.py
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/midi/midi_msg.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/midi/midi_note_data.py
+-rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/midi/midi_port.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/midi/midi_ports_update.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/osc/__init__.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/osc/osc_msg.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/osc/osc_port.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/osc/osc_query_maker.py
+-rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/resources/icon.ico
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 midiscripter-0.1.3/midiscripter/resources/icon.svg
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 midiscripter-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 midiscripter-0.1.3/README.md
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 midiscripter-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    13962 2020-02-02 00:00:00.000000 midiscripter-0.1.3/PKG-INFO
```

### Comparing `midiscripter-0.1.2/midiscripter/base/msg_base.py` & `midiscripter-0.1.3/midiscripter/base/msg_base.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/base/port_base.py` & `midiscripter-0.1.3/midiscripter/base/port_base.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/base/shared.py` & `midiscripter-0.1.3/midiscripter/base/shared.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/cli/starters.py` & `midiscripter-0.1.3/midiscripter/cli/starters.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import NoReturn
 
 import midiscripter.base.shared
 import midiscripter.base.port_base
 import midiscripter.logger.console_sink
 import midiscripter.midi
 import midiscripter.logger.log
-from midiscripter.logger import log  
+from midiscripter.logger import log
 
 
 def start_cli_debug() -> NoReturn:
     """Starts the script with log output to console.
     Console prints increase latency and jitter. Use for debugging only.
     """
     log._sink = midiscripter.logger.console_sink.ConsoleSink()
```

### Comparing `midiscripter-0.1.2/midiscripter/file_event/file_event_msg.py` & `midiscripter-0.1.3/midiscripter/file_event/file_event_msg.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/file_event/file_event_port.py` & `midiscripter-0.1.3/midiscripter/file_event/file_event_port.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/gui/app.py` & `midiscripter-0.1.3/midiscripter/gui/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,25 @@
         super().__init__()
         self.setOrganizationName('MIDI Scripter')
         self.setApplicationName(pathlib.Path(midiscripter.base.shared.script_path).name)
         icon_path = pathlib.Path(midiscripter.__file__).parent / 'resources' / 'icon.ico'
         self.setWindowIcon(QIcon(str(icon_path)))
 
         self.__time_until_restart_sec = self.RESTART_DELAY
-        self.request_restart.connect(self.restart)
+        self.request_restart.connect(self, self.restart)
         self.aboutToQuit.connect(self.__cleanup)
 
     def prepare_main_window(self, minimized_to_tray: bool = False):
         self.main_window = midiscripter.gui.main_window.MainWindow(self.widgets_to_add)
-        
+
         if not minimized_to_tray:
             self.main_window.show_from_tray()
         else:
             self.main_window.close()
-            
+
     def restart_at_file_change(self, msg: 'midiscripter.file_event.file_change_msg.FileEventMsg'):
         if msg.type not in (midiscripter.file_event.file_event_msg.FileEventType.CREATED,
                             midiscripter.file_event.file_event_msg.FileEventType.MODIFIED):
             return
 
         self.__time_until_restart_sec = self.RESTART_DELAY
         sleep_step_sec = 0.1
@@ -88,15 +88,15 @@
 
 def start_gui() -> NoReturn:
     """Starts the script and runs GUI. Logging goes to GUI Log widget."""
     midiscripter.base.shared._raise_current_process_cpu_priority()
 
     sigint_exit_code = {'Windows': -1073741510, 'Linux': 130, 'Darwin': 2}[platform.system()]
     signal.signal(signal.SIGINT, lambda *_: app_instance.exit(sigint_exit_code))
-    
+
     signal_checker_dummy_timer = QTimer()  # runs python code from Qt to allow the signal to trigger
     signal_checker_dummy_timer.start(1000)
     signal_checker_dummy_timer.timeout.connect(lambda: None)  # dummy python code to run
 
     start_minimized_to_tray = '--tray' in sys.argv
 
     with midiscripter.base.port_base._all_opened():
```

### Comparing `midiscripter-0.1.2/midiscripter/gui/log_widget.py` & `midiscripter-0.1.3/midiscripter/gui/log_widget.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/gui/main_window.py` & `midiscripter-0.1.3/midiscripter/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/gui/menu_bar.py` & `midiscripter-0.1.3/midiscripter/gui/menu_bar.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/gui/ports_widget.py` & `midiscripter-0.1.3/midiscripter/gui/ports_widget.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/gui/gui_widgets/button.py` & `midiscripter-0.1.3/midiscripter/gui/gui_widgets/button.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/gui/gui_widgets/gui_msg.py` & `midiscripter-0.1.3/midiscripter/gui/gui_widgets/gui_msg.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/gui/gui_widgets/gui_widget_base.py` & `midiscripter-0.1.3/midiscripter/gui/gui_widgets/gui_widget_base.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/gui/gui_widgets/layout.py` & `midiscripter-0.1.3/midiscripter/gui/gui_widgets/layout.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/gui/gui_widgets/list.py` & `midiscripter-0.1.3/midiscripter/gui/gui_widgets/list.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/gui/gui_widgets/mixins.py` & `midiscripter-0.1.3/midiscripter/gui/gui_widgets/mixins.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/gui/gui_widgets/text.py` & `midiscripter-0.1.3/midiscripter/gui/gui_widgets/text.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/keyboard/keyboard_msg.py` & `midiscripter-0.1.3/midiscripter/keyboard/keyboard_msg.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/keyboard/keyboard_port.py` & `midiscripter-0.1.3/midiscripter/keyboard/keyboard_port.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/logger/console_sink.py` & `midiscripter-0.1.3/midiscripter/logger/console_sink.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/logger/html_sink.py` & `midiscripter-0.1.3/midiscripter/logger/html_sink.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/logger/log.py` & `midiscripter-0.1.3/midiscripter/logger/log.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/metronome/metronome_port.py` & `midiscripter-0.1.3/midiscripter/metronome/metronome_port.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/midi/midi_msg.py` & `midiscripter-0.1.3/midiscripter/midi/midi_msg.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/midi/midi_note_data.py` & `midiscripter-0.1.3/midiscripter/midi/midi_note_data.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/midi/midi_port.py` & `midiscripter-0.1.3/midiscripter/midi/midi_port.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/midi/midi_ports_update.py` & `midiscripter-0.1.3/midiscripter/midi/midi_ports_update.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/osc/osc_msg.py` & `midiscripter-0.1.3/midiscripter/osc/osc_msg.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/osc/osc_port.py` & `midiscripter-0.1.3/midiscripter/osc/osc_port.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/osc/osc_query_maker.py` & `midiscripter-0.1.3/midiscripter/osc/osc_query_maker.py`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/resources/icon.ico` & `midiscripter-0.1.3/midiscripter/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/midiscripter/resources/icon.svg` & `midiscripter-0.1.3/midiscripter/resources/icon.svg`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/LICENSE` & `midiscripter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `midiscripter-0.1.2/README.md` & `midiscripter-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		msg.data1 += 12 * int(octave_selector.selected_item_text)  # modify
 		proxy_output.send(msg)  # route
 
 if __name__ == '__main__':  # combine multiple scripts by importing them
 	start_gui()  # opens helpful customizable GUI
 ```
 
-![Screenshot](/examples/octave_transposer/screenshot.png)
+![Screenshot](https://github.com/Maboroshy/midi-scripter/blob/master/examples/octave_transposer/screenshot.png?raw=true)
 
 [Scripting guide and API documentation available](https://maboroshy.github.io/midi-scripter)
 
 Easy tasks for MIDI Scripter:  
 1. Filter, modify and route MIDI, OSC and keyboard messages in any way.  
 2. Map MIDI, OSC and keyboard to each other.  
 3. Map any Python code to input message.  
@@ -41,15 +41,15 @@
 1. Create and map complex macros involving multiple hardware or virtual MIDI controllers.
 2. Make custom sequencer or MIDI input generator.
 3. Make music education ot trainer GUI application based on MIDI input.
 
 Currently MIDI Scripter is at "beta" development stage. It's fully functional but needs some more testing. It targets only Windows for now but Linux and macOS support will follow.
 
 ## Installation
-1. [Python 3.11+](https://www.python.org/downloads/).
+1. [Python 3.11+](https://www.python.org/downloads/) with "Add python.exe to PATH" option.
 2. [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html) for virtual MIDI output ports on Windows.
 3. `pip install midiscripter` in console.
 
 ## Setup
 Run loopMIDI and add virtual ports you want to send MIDI messages. You can enable its autostart option.
 
 Enable virtual MIDI output ports as MIDI inputs in DAW.
```

### Comparing `midiscripter-0.1.2/pyproject.toml` & `midiscripter-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'midiscripter'
-version = '0.1.2'
+version = '0.1.3'
 description = 'Framework for scripting MIDI, keyboard and Open Sound Control input and output'
 readme = 'README.md'
 requires-python = '>=3.11'
 license = {file = "LICENSE"}
 keywords = ['MIDI', 'OSC', 'script', 'automation', 'input']
-authors = [
-  {name = 'Maboroshy'},
-]
+authors = [{name = 'Maboroshy'}]
 classifiers = [
   'Development Status :: 4 - Beta',
   'Programming Language :: Python',
   'Programming Language :: Python :: 3.11',
   'Programming Language :: Python :: 3.12',
   'Programming Language :: Python :: Implementation :: CPython',
   'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
@@ -27,20 +25,22 @@
 ]
 dependencies = [
   'colorama ~=0.4',  # BSD
   'python-rtmidi ~=1.5',  # MIT
   'python-osc ~=1.7',  # Unlicense
   'pynput ~=1.7',  # LGPL
   'watchdog ~=4.0',  # Apache
-  'PySide6-Essentials ~=6.4',  # LGPL
+  'PySide6_Essentials >6.4, <6.7',  # LGPL Got broken Signal.connect on 6.7
+  'pywin32; platform_system == "Windows"',  # BSD
 ]
 
 [project.optional-dependencies]
 doc = [
   'mkdocs-material',
+  'mkdocstrings',
   'griffe-inherited-docstrings',
 ]
 
 [tool.hatch.build.targets.sdist]
 only-include = ['midiscripter']
 
 [project.gui-scripts]
```

### Comparing `midiscripter-0.1.2/PKG-INFO` & `midiscripter-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: midiscripter
-Version: 0.1.2
+Version: 0.1.3
 Summary: Framework for scripting MIDI, keyboard and Open Sound Control input and output
 Project-URL: Documentation, https://maboroshy.github.io/midi-scripter
 Project-URL: Issues, https://github.com/Maboroshy/midi-scripter/issues
 Project-URL: Source, https://github.com/Maboroshy/midi-scripter
 Author: Maboroshy
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -182,21 +182,23 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Requires-Dist: colorama~=0.4
 Requires-Dist: pynput~=1.7
-Requires-Dist: pyside6-essentials~=6.4
+Requires-Dist: pyside6-essentials<6.7,>6.4
 Requires-Dist: python-osc~=1.7
 Requires-Dist: python-rtmidi~=1.5
+Requires-Dist: pywin32; platform_system == 'Windows'
 Requires-Dist: watchdog~=4.0
 Provides-Extra: doc
 Requires-Dist: griffe-inherited-docstrings; extra == 'doc'
 Requires-Dist: mkdocs-material; extra == 'doc'
+Requires-Dist: mkdocstrings; extra == 'doc'
 Description-Content-Type: text/markdown
 
 # MIDI Scripter
 
 MIDI Scripter is a framework for scripting MIDI, keyboard and Open Sound Control (OSC) input and output with a few lines of Python code.
 
 MIDI Scripter is intended for digital audio workstation (DAW) controls scripting but can also be used for general input conversion and automation. It fits where controller mappings are not enough but rewriting DAW controller integration is too much. 
@@ -218,15 +220,15 @@
 		msg.data1 += 12 * int(octave_selector.selected_item_text)  # modify
 		proxy_output.send(msg)  # route
 
 if __name__ == '__main__':  # combine multiple scripts by importing them
 	start_gui()  # opens helpful customizable GUI
 ```
 
-![Screenshot](/examples/octave_transposer/screenshot.png)
+![Screenshot](https://github.com/Maboroshy/midi-scripter/blob/master/examples/octave_transposer/screenshot.png?raw=true)
 
 [Scripting guide and API documentation available](https://maboroshy.github.io/midi-scripter)
 
 Easy tasks for MIDI Scripter:  
 1. Filter, modify and route MIDI, OSC and keyboard messages in any way.  
 2. Map MIDI, OSC and keyboard to each other.  
 3. Map any Python code to input message.  
@@ -238,15 +240,15 @@
 1. Create and map complex macros involving multiple hardware or virtual MIDI controllers.
 2. Make custom sequencer or MIDI input generator.
 3. Make music education ot trainer GUI application based on MIDI input.
 
 Currently MIDI Scripter is at "beta" development stage. It's fully functional but needs some more testing. It targets only Windows for now but Linux and macOS support will follow.
 
 ## Installation
-1. [Python 3.11+](https://www.python.org/downloads/).
+1. [Python 3.11+](https://www.python.org/downloads/) with "Add python.exe to PATH" option.
 2. [loopMIDI](https://www.tobias-erichsen.de/software/loopmidi.html) for virtual MIDI output ports on Windows.
 3. `pip install midiscripter` in console.
 
 ## Setup
 Run loopMIDI and add virtual ports you want to send MIDI messages. You can enable its autostart option.
 
 Enable virtual MIDI output ports as MIDI inputs in DAW.
```

