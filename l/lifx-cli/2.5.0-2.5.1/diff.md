# Comparing `tmp/lifx_cli-2.5.0.tar.gz` & `tmp/lifx_cli-2.5.1.tar.gz`

## Comparing `lifx_cli-2.5.0.tar` & `lifx_cli-2.5.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/requirements.txt
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/__init__.py
--rwxr-xr-x   0        0        0     2098 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/auth.py
--rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/colors.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/effects.py
--rwxr-xr-x   0        0        0    11522 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/lifx.py
--rwxr-xr-x   0        0        0     2599 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/lights.py
--rwxr-xr-x   0        0        0     1349 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/src/lifx/scenes.py
--rwxr-xr-x   0        0        0     1038 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/tests/lifx_cli_test.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/tests/requirements.txt
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/LICENSE
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 lifx_cli-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/requirements.txt
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/__init__.py
+-rwxr-xr-x   0        0        0     2098 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/auth.py
+-rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/colors.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/effects.py
+-rwxr-xr-x   0        0        0    12261 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/lifx.py
+-rwxr-xr-x   0        0        0     3149 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/lights.py
+-rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/scenes.py
+-rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/tests/lifx_cli_test.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/tests/requirements.txt
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/LICENSE
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/PKG-INFO
```

### Comparing `lifx_cli-2.5.0/.github/workflows/pylint.yml` & `lifx_cli-2.5.1/.github/workflows/pylint.yml`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
       run: |
         python -m pip install --upgrade pip
         pip install pylint
         pip install -r requirements.txt
         pip install -e .
     - name: Analysing the code with pylint
       run: |
-        pylint $(git ls-files '*.py') --fail-under=9.0
+        pylint $(git ls-files '*.py') --fail-under=9.50
```

### Comparing `lifx_cli-2.5.0/.github/workflows/python-publish.yml` & `lifx_cli-2.5.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.0/src/lifx/auth.py` & `lifx_cli-2.5.1/src/lifx/auth.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.0/src/lifx/colors.py` & `lifx_cli-2.5.1/src/lifx/colors.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.0/src/lifx/effects.py` & `lifx_cli-2.5.1/src/lifx/effects.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
             'Performs a breathe effect by slowly fading between the given colors.'],
            ['Pulse',
             'Performs a pulse effect by quickly flashing between the given colors. ']]
 EFFECTS_NOTICE = "Note: The CLI can only control effects stored on your light's firmware."
 
 
 class Effects:
+    """Control LIFX effects."""
     def __init__(self):
         self.auth = Auth()
         self.auth_headers = self.auth.auth()
 
     @staticmethod
     def list_effects():
         """List effects currently supported by the CLI."""
```

### Comparing `lifx_cli-2.5.0/src/lifx/lifx.py` & `lifx_cli-2.5.1/src/lifx/lifx.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,65 +2,124 @@
 """
 Author: Wes Henderson
 Control your lights with the unofficial LIFX CLI. This CLI uses the
 LIFX HTTP endpoints to configure your lights.
 https://api.developer.lifx.com/reference/introduction
 """
 import argparse
+import sys
 from src.lifx.auth import Auth
 from src.lifx.colors import Colors
 from src.lifx.effects import Effects
 from src.lifx.lights import Lights
 from src.lifx.scenes import Scenes
 
-auth = Auth()
-
 LOGO = """
 ██      ██ ███████ ██   ██      ██████ ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ██      ██ █████     ███       ██      ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ███████ ██ ██      ██   ██      ██████ ███████ ██
 
 """
 
 
+def colors_sub_command(args):
+    """Control the actions for the 'colors' sub-command."""
+    colors = Colors()
+
+    if isinstance(args, list):
+        list_colors = args[0]
+        provided_color = args[1]
+    else:
+        list_colors = args.list_colors
+        provided_color = args.colors
+
+    if list_colors:
+        colors.color_information()
+
+    if provided_color:
+        colors.validate_color(provided_color)
+
+
+def effects_sub_command(args=None):
+    """Control the actions for the 'effects' sub-command."""
+    effects = Effects()
+
+    if isinstance(args, list):
+        list_effects = args[0]
+        light_id = args[1]
+        group = args[2]
+        color = args[3]
+        breathe = args[4]
+        pulse = args[5]
+        stop = args[6]
+    else:
+        list_effects = args.list_effects
+        light_id = args.light_id
+        group = args.group
+        color = args.color
+        breathe = args.breathe
+        pulse = args.pulse
+        stop = args.stop
+
+    if list_effects:
+        effects.list_effects()
+    elif not light_id:
+        print("Must specify a light/group ID.")
+        sys.exit(4)
+    if breathe:
+        effects.breathe_effect(light_id, group, color)
+    elif pulse:
+        effects.pulse_effect(light_id, group, color)
+    elif stop:
+        effects.stop_effect(light_id, group)
+
+
 def lights_sub_command(args=None):
     """Control the actions for the 'lights' sub-command."""
     light = Lights()
 
     if isinstance(args, list):
         devices = args[0]
         light_id = args[1]
         toggle = args[2]
         group = args[3]
-        state = args[4]
-        color = args[5]
-        power = args[6]
-        brightness = args[7]
-        infrared = args[8]
-        duration = args[9]
+        clean_duration = args[4]
+        state = args[5]
+        color = args[6]
+        power = args[7]
+        brightness = args[8]
+        infrared = args[9]
+        duration = args[10]
     else:
         devices = args.list_devices
         light_id = args.light_id
         toggle = args.toggle
         group = args.group
+        clean_duration = args.clean_duration
         state = args.state
         color = args.color
         power = args.power
         brightness = args.brightness
         infrared = args.infrared
         duration = args.duration
 
     if devices:
         light.get()
+    elif not light_id:
+        print("Must specify a light/group ID.")
+        sys.exit(2)
 
     if toggle:
         light.toggle(light_id, group)
 
+    if clean_duration:
+        light.clean(light_id, group, clean_duration)
+
     if state:
         state_attributes = {'power': power,
                             'brightness': brightness,
                             'duration': duration,
                             'infrared': infrared}
         light.set_state(light_id, group, color, state_attributes)
 
@@ -74,70 +133,25 @@
         scene_id = args[1]
     else:
         scenes = args.list_scenes
         scene_id = args.scene_id
 
     if scenes:
         scene.get()
+    elif not scene_id:
+        print("Must specify a scene ID.")
+        sys.exit(3)
 
     if scene_id:
         scene.activate(scene_id)
 
 
-def effects_sub_command(args=None):
-    """Control the actions for the 'effects' sub-command."""
-    effects = Effects()
-
-    if isinstance(args, list):
-        list_effects = args[0]
-        light_id = args[1]
-        group = args[2]
-        color = args[3]
-        breathe = args[4]
-        pulse = args[5]
-        stop = args[6]
-    else:
-        list_effects = args.list_effects
-        light_id = args.light_id
-        group = args.group
-        color = args.color
-        breathe = args.breathe
-        pulse = args.pulse
-        stop = args.stop
-
-    if list_effects:
-        effects.list_effects()
-    if breathe:
-        effects.breathe_effect(light_id, group, color)
-    elif pulse:
-        effects.pulse_effect(light_id, group, color)
-    elif stop:
-        effects.stop_effect(light_id, group)
-
-
-def colors_sub_command(args):
-    """Control the actions for the 'colors' sub-command."""
-    colors = Colors()
-
-    if isinstance(args, list):
-        list_colors = args[0]
-        provided_color = args[1]
-    else:
-        list_colors = args.list_colors
-        provided_color = args.colors
-
-    if list_colors:
-        colors.color_information()
-
-    if provided_color:
-        colors.validate_color(provided_color)
-
-
 def main():
     """Main entrypoint for the LIFX CLI."""
+    auth = Auth()
     print(LOGO)
     # Create the parser
     description = 'Control LIFX devices via the CLI!'
     epilog = 'Run `lifx --configure` to setup authentication.'
     job_options = argparse.ArgumentParser(description=description, epilog=epilog)
 
     # Add the arguments
@@ -176,14 +190,20 @@
                                action='store_true',
                                help='Specify whether or not the target is a group.')
     light_command.add_argument('-s',
                                '--state',
                                default=False,
                                action='store_true',
                                help='Set the state for the specified light.')
+    light_command.add_argument('-n',
+                               '--clean',
+                               default=False,
+                               dest='clean_duration',
+                               action='store',
+                               help='Turn on Clean mode for N seconds.')
     light_command.add_argument('-c',
                                '--color',
                                default='green',
                                action='store',
                                help='Use the specified color. [Default: green]')
     light_command.add_argument('-p',
                                '--power',
@@ -246,15 +266,15 @@
                                 default=False,
                                 action='store_true',
                                 help='Specify whether or not the target is a group.')
     effect_command.add_argument('-c',
                                 '--color',
                                 default=[],
                                 action='append',
-                                help='Specify the color; multiple -c options alternate colors.')
+                                help='Set the color; add multiple -c options to alternate colors.')
     effect_command.add_argument('--breathe',
                                 default=False,
                                 action='store_true',
                                 help='Effects: Breathe')
     effect_command.add_argument('--pulse',
                                 default=False,
                                 action='store_true',
@@ -284,26 +304,26 @@
 
     args = job_options.parse_args()
 
     # Configure authentication.
     if args.configure:
         auth.configure()
 
+    # The 'colors' sub-command.
+    if args.command == 'colors':
+        colors_sub_command(args)
+
+    # The 'effects' sub-command.
+    if args.command == 'effects':
+        effects_sub_command(args)
+
     # The 'lights' sub-command.
     if args.command == 'lights':
         lights_sub_command(args)
 
     # The 'scenes' sub-command.
     if args.command == 'scenes':
         scenes_sub_command(args)
 
-    # The 'effects' sub-command.
-    if args.command == 'effects':
-        effects_sub_command(args)
-
-    # The 'colors' sub-command.
-    if args.command == 'colors':
-        colors_sub_command(args)
-
 
 if __name__ == '__main__':
     main()
```

### Comparing `lifx_cli-2.5.0/src/lifx/lights.py` & `lifx_cli-2.5.1/src/lifx/lights.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,21 +26,21 @@
             print(f"HTTP request failed. State code: {response.status_code}")
             sys.exit(30)
 
         response = json.loads(response.content)
 
         devices = []
 
-        for key in range(len(response)):
-            label = response[key]["label"]
-            ident = response[key]["id"]
-            power = response[key]["power"]
-            connected = response[key]["connected"]
-            group = response[key]["group"]["name"]
-            group_id = response[key]["group"]["id"]
+        for _, value in enumerate(response):
+            label = value["label"]
+            ident = value["id"]
+            power = value["power"]
+            connected = value["connected"]
+            group = value["group"]["name"]
+            group_id = value["group"]["id"]
 
             devices += [[label, ident, power, connected, group, group_id]]
 
         devices.sort()
         print(tabulate(devices, headers=["Name", "ID", "State", "Connected", "Group", "Group ID"]))
 
     def toggle(self, light_id, group):
@@ -76,7 +76,27 @@
         response = put(url, data=payload, headers=self.auth_headers, timeout=5)
 
         if response.status_code != 207:
             print(f"HTTP request failed. State code: {response.status_code}")
             sys.exit(32)
         else:
             sys.exit(0)
+
+    def clean(self, light_id, group, duration):
+        """Switches a light to clean mode. Requires the device ID."""
+
+        if group:
+            light_id = f'group_id:{light_id}'
+
+        payload = {
+            "stop": "False",
+            "duration": f"{duration}",
+        }
+
+        url = f"{API}/lights/{light_id}/clean"
+        response = post(url, data=payload, headers=self.auth_headers, timeout=5)
+
+        if response.status_code != 207:
+            print(f"HTTP request failed. State code: {response.status_code}")
+            sys.exit(33)
+        else:
+            sys.exit(0)
```

### Comparing `lifx_cli-2.5.0/src/lifx/scenes.py` & `lifx_cli-2.5.1/src/lifx/scenes.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,16 @@
             print(f"HTTP request failed. State code: {response.status_code}")
             sys.exit(40)
 
         response = json.loads(response.content)
 
         scenes = []
 
-        for key in range(len(response)):
-            scenes += [[response[key]["name"], response[key]["uuid"]]]
+        for _, value in enumerate(response):
+            scenes += [[value["name"], value["uuid"]]]
 
         scenes.sort()
         print(tabulate(scenes, headers=["Name", "ID"]))
 
     def activate(self, scene_id):
         """Activates the specified scene. Requires scene UUID."""
```

### Comparing `lifx_cli-2.5.0/tests/lifx_cli_test.py` & `lifx_cli-2.5.1/tests/lifx_cli_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 #!/usr/bin/env python3
+"""Tests for lifx-cli."""
 import pytest
 import src.lifx.lifx
 
 
 def test_colors(capsys):
+    """Test the colors sub-command."""
     cli_args = [False, 'blue']
     src.lifx.lifx.colors_sub_command(cli_args)
     out, err = capsys.readouterr()
     assert "Saturation" in out
     assert err == ""
 
 
-def test_effects(capsys):
+def test_effects():
+    """Test the effects sub-command (lights will flash purple as Wes' home."""
     cli_args = [False, '917e85258fa3c3fe15816a04db6a9a15', True, ['purple'], True, False, False]
     with pytest.raises(SystemExit) as pytest_wrapped_e:
         src.lifx.lifx.effects_sub_command(cli_args)
     assert pytest_wrapped_e.type == SystemExit
     assert pytest_wrapped_e.value.code == 0
 
 
 def test_lights(capsys):
-    cli_args = [True, False, False, False, False, False, False, False, False, False]
+    """Test the lights sub-command."""
+    cli_args = [True, False, False, False, False, False, False, False, False, False, False]
     src.lifx.lifx.lights_sub_command(cli_args)
     out, err = capsys.readouterr()
     assert "d073d568d053" in out
     assert err == ""
 
 
 def test_scenes(capsys):
+    """Test the scenes sub-command."""
     cli_args = [True, False]
     src.lifx.lifx.scenes_sub_command(cli_args)
     out, err = capsys.readouterr()
     assert "9371a59c-6ee7-4ced-a3d3-b25d9fc08aad" in out
     assert err == ""
```

### Comparing `lifx_cli-2.5.0/.gitignore` & `lifx_cli-2.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.0/LICENSE` & `lifx_cli-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.0/README.md` & `lifx_cli-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.0/pyproject.toml` & `lifx_cli-2.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lifx-cli"
-version = "2.5.0"
+version = "2.5.1"
 authors = [{name="Wes Henderson", email="info@necrux.com"}]
 description = "The Unofficial LIFX CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   'requests',
   'tabulate',
```

### Comparing `lifx_cli-2.5.0/PKG-INFO` & `lifx_cli-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifx-cli
-Version: 2.5.0
+Version: 2.5.1
 Summary: The Unofficial LIFX CLI
 Project-URL: Homepage, https://github.com/necrux/lifx-cli
 Project-URL: Bug Tracker, https://github.com/necrux/lifx-cli/issues
 Author-email: Wes Henderson <info@necrux.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

