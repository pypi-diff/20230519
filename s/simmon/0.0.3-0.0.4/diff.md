# Comparing `tmp/simmon-0.0.3.tar.gz` & `tmp/simmon-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simmon-0.0.3.tar", last modified: Mon May 15 05:05:35 2023, max compression
+gzip compressed data, was "simmon-0.0.4.tar", last modified: Fri May 19 10:29:04 2023, max compression
```

## Comparing `simmon-0.0.3.tar` & `simmon-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 05:05:35.056275 simmon-0.0.3/
--rw-rw-rw-   0        0        0     1086 2023-05-13 12:49:09.000000 simmon-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     6236 2023-05-15 05:05:35.056275 simmon-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5901 2023-05-15 04:55:07.000000 simmon-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 05:05:35.056275 simmon-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      693 2023-05-15 05:05:26.000000 simmon-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 05:05:35.056275 simmon-0.0.3/simmon/
-drwxrwxrwx   0        0        0        0 2023-05-15 05:05:35.056275 simmon-0.0.3/simmon/simmon.egg-info/
--rw-rw-rw-   0        0        0     6236 2023-05-15 05:05:34.000000 simmon-0.0.3/simmon/simmon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-15 05:05:34.000000 simmon-0.0.3/simmon/simmon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 05:05:34.000000 simmon-0.0.3/simmon/simmon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 05:05:34.000000 simmon-0.0.3/simmon/simmon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 05:05:34.000000 simmon-0.0.3/simmon/simmon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    29858 2023-05-13 14:45:40.000000 simmon-0.0.3/simmon/simmon.py
+drwxrwxrwx   0        0        0        0 2023-05-19 10:29:04.324296 simmon-0.0.4/
+-rw-rw-rw-   0        0        0     1086 2023-05-13 12:49:09.000000 simmon-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     6602 2023-05-19 10:29:04.324296 simmon-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6267 2023-05-16 14:22:15.000000 simmon-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 10:29:04.324296 simmon-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      693 2023-05-19 10:28:42.000000 simmon-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 10:29:04.308683 simmon-0.0.4/simmon/
+drwxrwxrwx   0        0        0        0 2023-05-19 10:29:04.324296 simmon-0.0.4/simmon/simmon.egg-info/
+-rw-rw-rw-   0        0        0     6602 2023-05-19 10:29:04.000000 simmon-0.0.4/simmon/simmon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-19 10:29:04.000000 simmon-0.0.4/simmon/simmon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 10:29:04.000000 simmon-0.0.4/simmon/simmon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-19 10:29:04.000000 simmon-0.0.4/simmon/simmon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-19 10:29:04.000000 simmon-0.0.4/simmon/simmon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    43039 2023-05-19 10:23:09.000000 simmon-0.0.4/simmon/simmon.py
```

### Comparing `simmon-0.0.3/LICENSE` & `simmon-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simmon-0.0.3/PKG-INFO` & `simmon-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: simmon
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple simulation monitor
 Author: Roie Zemel
 Keywords: simulation, data tracking
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Logo](https://raw.githubusercontent.com/roiezemel/simmon/main/assets/simmon_expanded_logo.png)
 
 [![PyPI version](https://badge.fury.io/py/simmon.svg)](https://badge.fury.io/py/simmon)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/roiezemel/simmon)
+[![Documentation Status](https://readthedocs.org/projects/simmon/badge/?version=latest)](https://simmon.readthedocs.io/en/latest/?badge=latest)
 
 # A simple monitor for simulations and other numeric processes
 
 ## Overview
 This project provides a simple tool for tracking simulations and 
 other numeric processes. It provides a Monitor class that has 
 all the following functionality:
-- Tracking numeric variables.
-- Plotting the data.
-- An updating live view of the tracked variables.
-- A window of convenience toggles to control the progress
+
+* Tracking numeric variables.
+* Plotting the data.
+* An updating live view of the tracked variables.
+* A window of convenience toggles to control the progress
 of a long-running simulation.
-- Automatically saving all the collected data in a single output directory, including:
-  - .csv files
-  - Plots
-  - A config file with configuration constants
-  - A summary text file
-- Loading an output directory to continue working with a simulation that's been terminated.
+* Automatically saving all the collected data in a single output directory, including:
+  * .csv files
+  * Plots
+  * A config file with configuration constants
+  * A summary text file
+* Loading an output directory to continue working with a simulation that's been terminated.
 
 ## Installation
 Install with `pip`:
 ```commandline
 pip install simmon
 ```
 
 ## Usage
+You can find the documentation of this project [here](https://simmon.readthedocs.io/en/latest/?badge=latest).
 Here's a quick example of the `Monitor` class used to track a moving object simulation:
 
 ```python
 from simmon import Monitor
 
 # create Monitor - this already opens an output directory and a toggle-buttons control window
 mon = Monitor('Example Monitor')
@@ -158,7 +161,8 @@
 mon.plot(mon.trackers[0])  # same data can be plotted
 mon.plot('Things against x')  # even the same titles
 print(mon.dt, mon.its)  # config variables are still there
 ```
 
 ## Contributing
 Please report any bug you might come across. Contributions and enhancements are very welcome!
+Take a look at the [documentation](https://simmon.readthedocs.io/en/latest/?badge=latest) of this project.
```

### Comparing `simmon-0.0.3/README.md` & `simmon-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 ![Logo](https://raw.githubusercontent.com/roiezemel/simmon/main/assets/simmon_expanded_logo.png)
 
 [![PyPI version](https://badge.fury.io/py/simmon.svg)](https://badge.fury.io/py/simmon)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/roiezemel/simmon)
+[![Documentation Status](https://readthedocs.org/projects/simmon/badge/?version=latest)](https://simmon.readthedocs.io/en/latest/?badge=latest)
 
 # A simple monitor for simulations and other numeric processes
 
 ## Overview
 This project provides a simple tool for tracking simulations and 
 other numeric processes. It provides a Monitor class that has 
 all the following functionality:
-- Tracking numeric variables.
-- Plotting the data.
-- An updating live view of the tracked variables.
-- A window of convenience toggles to control the progress
+
+* Tracking numeric variables.
+* Plotting the data.
+* An updating live view of the tracked variables.
+* A window of convenience toggles to control the progress
 of a long-running simulation.
-- Automatically saving all the collected data in a single output directory, including:
-  - .csv files
-  - Plots
-  - A config file with configuration constants
-  - A summary text file
-- Loading an output directory to continue working with a simulation that's been terminated.
+* Automatically saving all the collected data in a single output directory, including:
+  * .csv files
+  * Plots
+  * A config file with configuration constants
+  * A summary text file
+* Loading an output directory to continue working with a simulation that's been terminated.
 
 ## Installation
 Install with `pip`:
 ```commandline
 pip install simmon
 ```
 
 ## Usage
+You can find the documentation of this project [here](https://simmon.readthedocs.io/en/latest/?badge=latest).
 Here's a quick example of the `Monitor` class used to track a moving object simulation:
 
 ```python
 from simmon import Monitor
 
 # create Monitor - this already opens an output directory and a toggle-buttons control window
 mon = Monitor('Example Monitor')
@@ -146,7 +149,8 @@
 mon.plot(mon.trackers[0])  # same data can be plotted
 mon.plot('Things against x')  # even the same titles
 print(mon.dt, mon.its)  # config variables are still there
 ```
 
 ## Contributing
 Please report any bug you might come across. Contributions and enhancements are very welcome!
+Take a look at the [documentation](https://simmon.readthedocs.io/en/latest/?badge=latest) of this project.
```

### Comparing `simmon-0.0.3/setup.py` & `simmon-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="simmon",
-    version="0.0.3",
+    version="0.0.4",
     author="Roie Zemel",
     description="A simple simulation monitor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     py_modules=["simmon"],
     package_dir={'': 'simmon'},
     install_requires=['matplotlib'],
     keywords=["simulation, data tracking"],
     license_files=('LICENSE',)
 )
```

### Comparing `simmon-0.0.3/simmon/simmon.egg-info/PKG-INFO` & `simmon-0.0.4/simmon/simmon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: simmon
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple simulation monitor
 Author: Roie Zemel
 Keywords: simulation, data tracking
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Logo](https://raw.githubusercontent.com/roiezemel/simmon/main/assets/simmon_expanded_logo.png)
 
 [![PyPI version](https://badge.fury.io/py/simmon.svg)](https://badge.fury.io/py/simmon)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/roiezemel/simmon)
+[![Documentation Status](https://readthedocs.org/projects/simmon/badge/?version=latest)](https://simmon.readthedocs.io/en/latest/?badge=latest)
 
 # A simple monitor for simulations and other numeric processes
 
 ## Overview
 This project provides a simple tool for tracking simulations and 
 other numeric processes. It provides a Monitor class that has 
 all the following functionality:
-- Tracking numeric variables.
-- Plotting the data.
-- An updating live view of the tracked variables.
-- A window of convenience toggles to control the progress
+
+* Tracking numeric variables.
+* Plotting the data.
+* An updating live view of the tracked variables.
+* A window of convenience toggles to control the progress
 of a long-running simulation.
-- Automatically saving all the collected data in a single output directory, including:
-  - .csv files
-  - Plots
-  - A config file with configuration constants
-  - A summary text file
-- Loading an output directory to continue working with a simulation that's been terminated.
+* Automatically saving all the collected data in a single output directory, including:
+  * .csv files
+  * Plots
+  * A config file with configuration constants
+  * A summary text file
+* Loading an output directory to continue working with a simulation that's been terminated.
 
 ## Installation
 Install with `pip`:
 ```commandline
 pip install simmon
 ```
 
 ## Usage
+You can find the documentation of this project [here](https://simmon.readthedocs.io/en/latest/?badge=latest).
 Here's a quick example of the `Monitor` class used to track a moving object simulation:
 
 ```python
 from simmon import Monitor
 
 # create Monitor - this already opens an output directory and a toggle-buttons control window
 mon = Monitor('Example Monitor')
@@ -158,7 +161,8 @@
 mon.plot(mon.trackers[0])  # same data can be plotted
 mon.plot('Things against x')  # even the same titles
 print(mon.dt, mon.its)  # config variables are still there
 ```
 
 ## Contributing
 Please report any bug you might come across. Contributions and enhancements are very welcome!
+Take a look at the [documentation](https://simmon.readthedocs.io/en/latest/?badge=latest) of this project.
```

### Comparing `simmon-0.0.3/simmon/simmon.py` & `simmon-0.0.4/simmon/simmon.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,23 +6,36 @@
 import matplotlib
 import matplotlib.pyplot as plt
 from multiprocessing import Process, Queue, Manager
 from tkinter import Tk, Label, ttk
 
 
 class Monitor:
-    """
-    Monitor and track a simulation. This class collects
+    """Monitor and track a simulation. This class collects
     data from a simulation and stores it in a single output directory.
     Provides a live view to track the progress of the simulation and a convenience
     toggle-buttons window.
+
+    :param name: A name for the Monitor. Also used as the output directory name.
+        By default, the output directory is given a name of the form "S#" where # is
+        the biggest number found in super_directory.
+    :type name: str, optional
+    :param super_directory: A path to a super directory, in which the output directory
+        for the Monitor is created. The super directory is created if it doesn't already exist.
+    :type super_directory: str, optional
+    :param enable_output_directory: Whether to create an output directory for the Monitor.
+        If False, then this class acts like QuietMonitor.
+    :type enable_output_directory: bool, optional
+    :param enable_toggles: Whether to open a toggles window for a convenient user control.
+    :type enable_toggles: bool, optional
     """
 
     def __init__(self, name=None, super_directory=None, enable_output_directory=True, enable_toggles=True):
-
+        """Constructor method
+        """
         # create output directories
         if enable_output_directory:
             self.dir_path = _generate_directory(name, super_directory)
             self.data_path = f'{self.dir_path}/data'
             _create_dir_path(self.data_path)
 
         self.titled_trackers = {}
@@ -42,24 +55,32 @@
         # save current time for the summary
         self._t0 = datetime.now()
 
         self.monitor_vars = set()
         self.monitor_vars.update(set(vars(self).keys()))
 
     def tracker(self, ind_var_name, *dep_var_names, title='no_title', autosave=False):
-        """
-        Create a tracker object to track variables.
+        """Create a tracker object to track variables.
         A tracker is associated with one independent variable, and multiple dependent
         variables.
+
         :param ind_var_name: The independent variable name.
+        :type ind_var_name: str
         :param dep_var_names: The dependent variable names.
-        :param title: An optional title. Multiple trackers with the same
-                      title will be plotted together.
-        :param autosave: Enables autosave for the tracker.
+        :type dep_var_names: str
+        :param title: A title for the trackers. Multiple trackers with the same
+            title will be plotted together.
+        :type title: str, optional
+        :param autosave: Enables autosave for the tracker. If True,
+            each update() call appends the data into the output file.
+            This ensures that the data won't be lost in case of
+            an unexpected termination. Default is False.
+        :type autosave: bool, optional
         :return: A tracker object that has an update() method.
+        :rtype: Tracker
         """
         if not getattr(self, 'data_path', False):  # if no files
             dir_path = ''
             autosave = False
         elif title == 'no_title':
             dir_path = self.data_path
         else:
@@ -76,51 +97,59 @@
         else:
             self.titled_trackers[title] = [tracker]
 
         self.trackers.append(tracker)  # add tracker to list as well
         return tracker
 
     def add_toggle(self, name='Toggle', desc='Press to toggle'):
-        """
-        Add a Toggle to the toggles window.
+        """Add a Toggle to the toggles window.
+
         :param name: Toggle name.
+        :type name: str, optional
         :param desc: Toggle description.
+        :type desc: str, optional
         :return: A new Toggle object that has the method toggled().
+        :rtype: Toggle
         """
+        if not hasattr(self, 'live_view_toggle'):
+            raise ReferenceError("The toggles for this Monitor have been disabled.")
+
         toggle = Toggle(self.live_view_toggle, name=name, desc=desc)
         self.toggles.append(toggle)
         return toggle
 
     def close_toggles(self):
-        """
-        Close all toggles.
+        """Close all toggles. No need if finalize() is called.
         """
         for toggle in self.toggles:
             toggle.close()
 
     def plot(self, *args):
-        """
-        Plot all trackers or groups of trackers in a single figure.
-        :param args: either titles, Tracker objects, or iterables of Tracker objects.
-        :return: a matplotlib figure, only if return_figure is True.
+        """Plot trackers or groups of trackers in a single figure.
+        This method accepts multiple arguments representing plots, and shows
+        all plots at once.
+
+        :param args: Either titles, Tracker objects, or iterables of Tracker objects.
+        :type args: str, Tracker, iterable
         """
         # save current backend
         backend = matplotlib.get_backend()
         matplotlib.use('TkAgg')
         if len(args) > 9:  # if more than 9 plots, divide into multiple figures
             _monitor_plot(self, *args[:9])
             self.plot(*args[9:])
         else:
             _monitor_plot(self, *args)
         matplotlib.use(backend)
 
     def open_live_view(self, update_rate=2):
-        """
-        Open a live view of the monitor in a different process.
-        :param update_rate: how many graph updates to perform in a second.
+        """Open a live view of the Monitor in a different process.
+
+        :param update_rate: How many graph updates to perform in a second.
+        :type update_rate: float, optional
         """
         # make self less recursive by removing monitor
         # reference from trackers
         for trackers in self.titled_trackers.values():
             for tracker in trackers:
                 tracker.monitor = None
 
@@ -149,32 +178,33 @@
         self.toggles = toggles
         self.live_view_toggle = live_view_toggle
         self.plot_toggle = plot_toggle
 
     def close_live_view(self):
         """
         Close the live view.
+
         """
         if not self.live_view_queue:  # means that live view is closed
             return
 
         self.live_view_queue.put(None)
         self.live_view_process.join()
         self.live_view_queue = None
         self.live_view_process = None
 
     def finalize(self):
-        """
-        Save all data tracked by this Monitor.
+        """Save all data tracked by this Monitor.
         This includes:
-        - Config data file
+        - Config file
+        - Summary file
         - Tracker .csv files
-        - .pickle files
-        - Graphs
-        Also closes the live view if it remained open.
+        - Plots
+        It also closes the live view and the toggles window.
+
         """
 
         # close live view
         self.close_live_view()
 
         # close toggles
         self.close_toggles()
@@ -207,17 +237,23 @@
         # save config file
         self._save_config_file()
 
         # save summary file
         self._save_summary_file()
 
     def load_from_dir(self, dir_path=None):
-        """
-        Load all monitor data already contained in dir_path.
-        :param dir_path: if provided, this path is used instead of self.dir_path.
+        """Load data stored in a Monitor's output directory.
+        This can be used to resume a terminated monitored process.
+        The data being loaded is:
+        - Config variables.
+        - Tracker objects including titles.
+
+        :param dir_path: The data is loaded
+            from this directory if provided. Otherwise, data is loaded from self.dir_path.
+        :type dir_path: str, optional
         """
         if not dir_path:
             if not getattr(self, 'dir_path', False):  # if no files
                 raise Exception("No directory to load from!")
             dir_path = self.dir_path
 
         data_path = f'{dir_path}/data'
@@ -225,20 +261,20 @@
 
         # load data
         if path.exists(data_path):
             data_content = next(walk(data_path), [()] * 3)
             for title in data_content[1]:  # dir names
                 group_path = f'{data_path}/{title}'
                 for tracker_filename in next(walk(group_path), [()] * 3)[2]:
-                    labels = tracker_filename.replace('+', '').split('-')
+                    labels = tracker_filename.replace('+', '').replace('.csv').split('-')
                     tracker = self.tracker(labels[0], *labels[1:], title=title)
                     _load_to_tracker(tracker, f'{group_path}/{tracker_filename}')
 
             for no_title_filename in data_content[2]:  # file names
-                labels = no_title_filename.replace('+', '').split('-')
+                labels = no_title_filename.replace('+', '').replace('.csv', '').split('-')
                 tracker = self.tracker(labels[0], *labels[1:])
                 _load_to_tracker(tracker, f'{data_path}/{no_title_filename}')
 
         # load config
         if path.exists(config_path):
             with open(config_path, 'r') as file:
                 for line in file.readlines()[3:]:
@@ -249,32 +285,35 @@
                         attr_value = values[1]
                         if attr_value.replace(".", "").replace("-", "").isnumeric():
                             attr_value = float(attr_value)
 
                         vars(self)[attr_name] = attr_value
 
     def _save_config_file(self):
-        """
-        Save attributes added to this object.
+        """Save attributes added to this object.
         These attributes are considered "configurations" and
         are written to a "config.txt" file.
+
         """
         content = "-----------------\n" \
                   "   Config Data   \n" \
                   "-----------------\n"
         for var_name, var in vars(self).items():
             if var_name not in self.monitor_vars:
                 content += f"{var_name}: {str(var)}\n"
 
         with open(self.dir_path + "/config.txt", 'w') as file:
             file.write(content[:-1])
 
     def _save_summary_file(self):
-        """
-        Save a summary of the Monitor.
+        """Save a summary of the Monitor's run.
+        Includes:
+        - The duration in which the Monitor was up.
+        - A summary of the data files in the output directory.
+
         """
         delta = datetime.now() - self._t0
         hours, remainder = divmod(delta.total_seconds(), 3600)
         minutes, seconds = divmod(remainder, 60)
         duration = '{:02}:{:02}:{:02}'.format(int(hours), int(minutes), int(seconds))
 
         content = f"-------------\n" \
@@ -290,28 +329,55 @@
             content += f" - {n_untitled} output file{'s' if n_untitled - 1 else ''} of untitled trackers."
 
         with open(self.dir_path + "/summary.txt", 'w') as file:
             file.write(content)
 
 
 class QuietMonitor(Monitor):
-    """
-    Represents a Monitor with no output files.
+    """Represents a Monitor with no output files.
     It is a traceless Monitor, that can be used
     in cases where the live-view and toggles
     are useful but there's no need for an output directory.
+
+    :param name: An optional name for the Monitor. Can be used to distinguish between multiple
+        running Monitors.
+    :type name: str, optional
+    :param enable_toggles: Whether to open a toggles window for a convenient user control.
+    :type enable_toggles: bool, optional
     """
     def __init__(self, name=None, enable_toggles=True):
         super().__init__(name=name, enable_output_directory=False, enable_toggles=enable_toggles)
 
 
 class Tracker:
-    """
-    Track variables and save them to .csv files.
-    This class is a helper to the Monitor class.
+    """This class is a helper to the Monitor class.
+    It tracks variables and communicates with a Monitor object.
+    Creating a Tracker instance is conventionally meant to be
+    done with tracker() method of Monitor.
+
+    :param monitor: A reference to a Monitor object.
+        This class communicates with the Monitor object
+        and is also referenced from Monitor.
+    :type monitor: Monitor
+    :param _id: A unique ID for the Tracker, used to identify data
+        segments sent to the live view process when active.
+        The live view process receives tuples with new data values
+        along with IDs through a Queue. This way it knows where to store
+        the new information (As it has its own copied Trackers).
+    :type _id: float
+    :param dir_path: A path to the directory in which the tracker should save
+        its data. This only truly happens in save(), or if autosave is enabled.
+    :type dir_path: str
+    :param ind_var_name: The independent variable name this tracker is meant to track.
+    :type ind_var_name: str
+    :param dep_var_names: The dependent variable names that are meant to be tracked.
+    :type dep_var_names: str sequence
+    :param autosave: If True, this means that for each update() call, the Tracker will
+        also update the output file with the new data received.
+    :type autosave: bool
     """
 
     def __init__(self, monitor: Monitor, _id: float, dir_path: str, ind_var_name: str, *dep_var_names, autosave=False):
 
         self._id = _id
         self.dir_path = dir_path
 
@@ -329,18 +395,25 @@
         self.data = []
         self.autosave = autosave
 
         if autosave:
             self.path = dir_path + '/' + _determine_tracker_filename(self, self.dir_path, '.csv')
 
     def update(self, ind_var, *dep_vars):
-        """
-        Update tracker's data.
-        :param ind_var: a current value of the independent variable.
-        :param dep_vars: current values of all dependent variables.
+        """Update tracker's data. If autosave is enabled
+        this data is also appended to the output file associated with this tracker.
+        The data provided here should match the data labels used to create the Tracker:
+        - The number of values should be equal to the number of data labels.
+        - The order of the values should match the order of the data labels, i.e. ind_var, dep_var1, dep_var2 ...
+
+
+        :param ind_var: A new value for the independent variable.
+        :type ind_var: float
+        :param dep_vars: New values for all dependent variables.
+        :type dep_vars: float
         """
         if len(dep_vars) != len(self.dep_var_names):
             raise Exception(f"Amount of data values ({1 + len(dep_vars)}) is "
                             f"different than the amount of data labels ({len(self.dep_var_names) + 1}).")
 
         curr_data = (ind_var, *dep_vars)
         self.data.append(curr_data)
@@ -352,56 +425,98 @@
         # update the live view queue if exists
         if self.monitor.live_view_queue:
             self.monitor.live_view_queue.put((self._id, curr_data))
 
         # refresh monitor toggles
         _refresh_monitor_toggles(self.monitor)
 
-    def save(self, path=None):
-        """
-        Save data to an output file.
+    def save(self, _path=None):
+        """Save data to an output file.
         If autosave is enabled, then default output file
         is removed.
-        :param path: path for the output file, otherwise, determined by
-                     the data labels.
+
+        :param _path: Path to an output file. If not provided, a filename is a constructed
+            out of the data labels.
+        :type _path: str, optional
         """
 
         # determine output file path
-        if not path:
-            path = self.dir_path + '/' + _determine_tracker_filename(self, self.dir_path, '.csv')
+        if not _path:
+            _path = self.dir_path + '/' + _determine_tracker_filename(self, self.dir_path, '.csv')
 
         # write data to output file
-        with open(path, 'w') as out_file:
+        with open(_path, 'w') as out_file:
             content = ""
             for line in self.data:
                 content += ','.join([str(v) for v in line]) + '\n'
             out_file.write(content)
 
         # remove previous output file if existed
         if p := getattr(self, 'path', False):
             remove(p)
 
     def _append_to_out_file(self, line):
+        """This is a helper to the autosave operation.
+        Appends a line to the output file located at self.path.
+        self.path is only declared if autosave is True.
+        If the file is currently denying permission (potentially
+        because the user opened it in another program), it warns the user,
+        blocks and waits until the operation succeeds.
+
+        :param line: A line to append to the output file located at self.path.
+        :type line: str
+        """
         try:
             with open(self.path, 'a') as out_file:
                 out_file.write(line + '\n')
         except PermissionError:
             warnings.warn("Tracker's output file is denying permission."
                           "\nCheck if the file is currently open in another program."
                           "\nThe program is currently blocked until permission "
                           "is granted.")
             # wait and then try again
             time.sleep(1)
             self._append_to_out_file(line)
 
 
 class Toggle:
+    """This class represents a toggle button.
+    It is supposed to be a helper to Monitor, with which
+    you can add toggles through the add_toggle() method.
+    But it can also work independently.
+    This class has two "modes":
+    Each object is either the main_toggle, which
+    means that it's in charge of opening the listening process which opens
+    the window of toggles. Or - it isn't the main toggle, and then it is joined
+    to a main_toggle. The main toggle's process accepts new toggles and adds them to
+    its tkinter window.
+    A 'toggle' is simply a button that can be pressed by the user as many times as they like.
+    Whenever the user presses the button, a count variable is incremented.
+    When the method `toggled()` is then invoked, True is returned if the count value
+    is not zero, and the count gets decremented. Thus, the method `toggled()` returns
+    True for every toggle made by the user.
+    Additionally, Toggle has a toggle_count member that keeps track of all toggles
+    made so far and "discovered" (i.e. `toggled()` returned True for them).
+    When closing a toggle, its button gets disabled but still appears as long as other toggles
+    are enabled. When all toggles joined in the same window are closed, then the window and listening
+    process are closed.
+
+    :param main_toggle: A main toggle that's in charge of opening the listening process,
+        which then creates a window and accepts other toggles. If None, then this object
+        would be a main toggle itself.
+    :type main_toggle: Toggle, None
+    :param name: A name for the Toggle. The name appears on the button.
+    :type name: str, optional
+    :param desc: A description for the Toggle. The description appears above the button.
+    :type desc: str, optional
+    :param window_title: A title for the toggles window. This is relevant if this
+        toggle is the main_toggle, as it opens the process that opens the window.
+    :type window_title: str, optional
     """
-    A helper class for Monitor that represents a toggle button.
-    """
+
     def __init__(self, main_toggle, name='Toggle', desc="Press to toggle", window_title="Toggle(s)"):
         self.toggle_count = 0
 
         if not main_toggle:
             self.main = True
 
             self.id = 0
@@ -421,38 +536,72 @@
 
             self.__in_q = main_toggle.__in_q
             self._send(1)  # signal to add a toggle
             self._send(name)
             self._send(desc)
 
     def toggled(self):
+        """Returns True for every toggle made by the user.
+        Each time a user presses the toggle, a count is incremented.
+        This method returns True if the count is bigger than 0, and decrements the count.
+
+        :return: True if the button has been toggled. False if it hasn't.
+        :rtype: bool
+        """
         if self.counts[self.id] > 0:
             self.toggle_count += 1
             self.counts[self.id] -= 1
             return True
         return False
 
     def close(self):
+        """Closes this toggle. If other toggles
+        in the window are still enabled, this toggle's button
+        will still appear but will become disabled. When all
+        toggles in the window are closed, then the window is closed as well.
+
+        """
         self._send(2)
         self._send(self.id)
 
     def _send(self, data):
+        """Used to send data to the listening process through
+        the instructions Queue.
+
+        :param data: Any data to be sent to the process.
+        """
         self.__in_q.put(data)
 
 
 # -----------------
 # UTILITY FUNCTIONS
 # -----------------
 def _live_view_process(monitor: Monitor, data_q: Queue, update_rate):
-    """
-    This is the live view process.
+    """This is the live view process.
     It creates and updates the live view figure.
-    :param monitor: a monitor clone object (pickled and un-pickled).
-    :param data_q: a data queue to send data to the process.
-    :param update_rate: how many updates per second.
+    This process receives a copy of the Monitor object, as well
+    as a Queue for communication and an update rate.
+    When started, the process still doesn't show anything. When a Tracker
+    in the MAIN process gets updated with new values (aka via tracker.update()),
+    it then sends the new values to this process through the Queue structure, along
+    with the Tracker's ID. Only then does the live view starts showing its updating plot.
+    This is done so that only currently-updating trackers are plotted in the live view.
+    If another tracker will later get updated as well, it will also be plotted and added to the
+    live view figure.
+    The live view only checks the Queue and updates the plots every
+    once in a while, according to the update_rate, and in the rest of the time - it sleeps.
+    This continues until the main process signals this process to stop. It does so
+    by putting None in the Queue.
+
+    :param monitor: A monitor clone object (pickled and un-pickled).
+    :type monitor: Monitor
+    :param data_q: A data queue for sending new values to the process.
+    :type data_q: multiprocessing.Queue
+    :param update_rate: How many updates to perform per second.
+    :type update_rate: float
     """
     plt.ion()
     backend = matplotlib.get_backend()
     matplotlib.use('TkAgg')
 
     figure = None
     active = True
@@ -507,49 +656,68 @@
         time.sleep(1 / update_rate)
 
     matplotlib.use(backend)
     plt.ioff()
 
 
 def _custom_pause_live_view(interval):
+    """This is a custom pause used for a proper update of
+    the live view figure. This is a solution taken from Stack Overflow.
+
+    :param interval: A pause interval.
+    :type interval: float
+    """
     backend = plt.rcParams['backend']
     if backend in matplotlib.rcsetup.interactive_bk:
         fig_manager = matplotlib._pylab_helpers.Gcf.get_active()
         if fig_manager is not None:
             canvas = fig_manager.canvas
             if canvas.figure.stale:
                 canvas.draw()
             canvas.start_event_loop(interval)
             return
 
 
 def _redraw_live_view(monitor, prev_figure, trackers):
-    """
-    In case new trackers are added to the live view,
-    a new figure is created with this function.
-    :param monitor: the monitor.
-    :param prev_figure: the previous figure.
-    :param trackers: the updated list of trackers.
-    :return: new figure and a list of axes objects.
+    """Helper to the live view process.
+    Whenever new trackers get updated, their plots
+    should be added to the live view figure (see _live_view_process). In this case, a new figure
+    needs to be created.
+
+    :param monitor: The monitor clone containing the tracker objects.
+    :type monitor: Monitor
+    :param prev_figure: The previous figure.
+    :type prev_figure: matplotlib.Figure
+    :param trackers: The updated list of trackers to be plotted.
+    :type trackers: iterable
+    :return: A new figure and a list of axes objects.
+    :rtype: tuple
     """
     if prev_figure:
         plt.close()
 
     figure, axs = _monitor_plot(monitor, *trackers, return_figure_and_axs=True)
     figure.canvas.manager.set_window_title('Monitor (live-view mode)')
     plt.show(block=False)
     return figure, axs
 
 
 def _update_live_view_axes(new_data, tracker, axes):
-    """
-    Update a live view axes according to a new data update.
-    :param new_data: a tuple of new data values.
-    :param tracker: a tracker that stores all the data for the axes lines.
-    :param axes: the axes of the plot.
+    """Helper to the live view process.
+    Update a single live-view axes with a single tracker's plot.
+    This function takes the tracker being plotted, the axes on which it's done,
+    and the new values added to the data - in order to update the plot with the new values.
+
+    :param new_data: A tuple of new data values.
+    :type new_data: tuple
+    :param tracker: The tracker whose plot needs to get updated.
+        This tracker MUST include the updated values already.
+    :type tracker: Tracker
+    :param axes: The axes of the plot.
+    :type axes: matplotlib.Axes
     """
 
     # update x and y values
     xs = [d[0] for d in tracker.data]
     i = 1
     for line in axes.get_lines():
         ys = [d[i] for d in tracker.data]
@@ -575,17 +743,26 @@
 
     # update x and y limits
     axes.set_xlim(x_min, x_max)
     axes.set_ylim(y_min, y_max)
 
 
 def _refresh_monitor_toggles(monitor):
-    """
-    Check if monitor's main toggles have been toggled.
-    :param monitor: a monitor.
+    """Helper to handle the default toggles of Monitor.
+    When a Monitor is created, some toggles are added to it
+    by default. These toggles then listen for user presses and
+    remember them.
+    But someone has to take care of what to do when they're
+    toggled. This function is called in every tracker update
+    of the monitor (see Tracker.update()). It checks if any of the default monitor toggles
+    has been toggled, and if so, it operates accordingly.
+    For example, it opens the live-view if the live-view toggle has been pressed.
+
+    :param monitor: The monitor whose default toggles would be checked.
+    :type monitor: Monitor
     """
     # if live view toggle toggled
     if getattr(monitor, 'live_view_toggle', False) and monitor.live_view_toggle.toggled():
         if monitor.live_view_toggle.toggle_count % 2:
             monitor.open_live_view()
         else:
             monitor.close_live_view()
@@ -604,20 +781,29 @@
                     groups[tr.ind_var_name] = [tr]
             titles.extend(groups.values())
 
         monitor.plot(*titles)
 
 
 def _monitor_plot(monitor, *args, return_figure_and_axs=False):
-    """
-    Plot all trackers or groups of trackers in a single figure.
-    :param args: either titles, Tracker objects, or iterables of Tracker objects.
-    :param return_figure_and_axs: if True, a matplotlib figure is returned
-                                  instead of being displayed, along with an array of axes objects.
-    :return: (optionally) a matplotlib figure, and an array of axs.
+    """Helper to Monitor plot.
+    This functions receives a Monitor object, and arguments specifying
+    what plots to make, and creates a matplotlib figure with all of these plots.
+    It then either shows this figure in a user-interface window, or returns the figure
+    and axs to the caller without opening the UI.
+
+    For an explanation of what arguments should be passed with *args, see Monitor.plot().
+
+    :param args: Either titles, Tracker objects, or iterables of Tracker objects.
+    :type args: str, Tracker, iterable
+    :param return_figure_and_axs: If True, a matplotlib figure is returned
+        instead of being displayed, along with an array of axes objects.
+    :type return_figure_and_axs: bool, optional
+    :return: (optionally) A matplotlib figure, and an array of axs.
+    :rtype: tuple
     """
     if not len(args):
         if return_figure_and_axs:
             return plt.figure(), []
         return
 
     # create a figure for the plot
@@ -675,18 +861,21 @@
         return figure, axs
 
     # else, display figure
     plt.show()
 
 
 def _plot_trackers(axes, trackers):
-    """
-    Plot a group of trackers' data.
-    :param axes: a matplotlib axes.
-    :param trackers: a list of trackers.
+    """Helper to _monitor_plot.
+    This function shows the graphs of a group of trackers in a single plot.
+
+    :param axes: An axes for the plot.
+    :type axes: matplotlib.Axes
+    :param trackers: A list of trackers.
+    :type trackers: iterable
     """
     # plot all graphs
     for tracker in trackers:
         # raise exception if object is not a Tracker object
         if type(tracker) != Tracker:
             raise ValueError(f"Cannot plot an object of type {type(tracker)}."
                              f" The iterable passed to _plot_trackers() must only contain"
@@ -694,34 +883,54 @@
 
         xs = [line[0] for line in tracker.data]
         for i in range(len(tracker.dep_var_names)):
             ys = [line[i + 1] for line in tracker.data]
             axes.plot(xs, ys, label=tracker.dep_var_names[i])
 
     # set axis labels
-    if len(trackers) == 1 and len(trackers[0].dep_var_names) == 1:
+    if len(trackers) == 1 and len((tr := next(iter(trackers))).dep_var_names) == 1:
         # then there is only a single line
-        axes.set_xlabel(trackers[0].ind_var_name.capitalize())
-        axes.set_ylabel(trackers[0].dep_var_names[0].capitalize())
+        axes.set_xlabel(tr.ind_var_name.capitalize())
+        axes.set_ylabel(tr.dep_var_names[0].capitalize())
 
     else:
         # then there are multiple lines
         x_labels = set([tracker.ind_var_name for tracker in trackers])
         axes.set_xlabel(', '.join(x_labels).capitalize())
         axes.legend()
 
 
 def _toggle_window(in_q, _counts, name, desc, window_title):
-    """
-    This process creates toggle buttons and listens to toggles.
-    :param in_q: instruction queue.
-    :param _counts: counts array-like.
-    :param name: (main) toggle name.
-    :param desc: (main) toggle description.
-    :param window_title: a window title.
+    """Helper to Toggle class.
+    This is the listening process of the Toggles window.
+    This process initially creates a tkinter window, and adds a single
+    toggle button according to its arguments.
+    It then listens to user toggles, and also receives signals from the main
+    process through an instructions-queue.
+    These instructions are of two types:
+    1. Add a new toggle. This is followed with information about a new
+    toggle button to be added to the window. For an explanation
+    of how and why toggles are added in this way, see Toggle.
+    2. Close a toggle button. This comes with the ID of the Toggle
+    button to close. When a toggle is closed, its
+    button gets disabled, but it is not removed from the window. When all toggles
+    are closed, then the window is closed and this process terminates.
+
+    :param in_q: An instructions-queue used to receive instructions from
+        the main process.
+    :type in_q: multiprocessing.Queue
+    :param _counts: An array-like of counts used to keep track of toggles
+        made for each Toggle.
+    :type _counts: numpy.ndarray, list
+    :param name: The name of the initial main-toggle.
+    :type name: str
+    :param desc: Description for the main-toggle.
+    :type desc: str
+    :param window_title: A window title.
+    :type window_title: str
     """
     window = Tk()
     window.configure(bg='white')
     window.title(window_title)
 
     window.rowconfigure(0, weight=1)
     window.rowconfigure(1, weight=1)
@@ -787,32 +996,71 @@
 
     check_signal()
 
     window.mainloop()
 
 
 def _determine_tracker_filename(tracker, dir_path, ending):
+    """Used to determine the filename associated with a Tracker object.
+    This filename is simply a combination of the Tracker's data labels.
+    If the filename already exist in the output directory, '+'s are added
+    to the name to make it unique.
+    This function is used for both output data files, and output plot image files.
+
+    :param tracker: A Tracker for which a name should be determined.
+    :type tracker: Tracker
+    :param dir_path: The path to the output directory in which
+        the file will be saved.
+    :type dir_path: str
+    :param ending: A file ending, such as '.csv' or '.png'.
+    :type ending: str
+    :return: A filename for the Tracker's output.
+    :rtype: str
+    """
     name = '-'.join([tracker.ind_var_name] + tracker.dep_var_names) + ending
     while name in next(walk(dir_path), (None, None, []))[2]:
         name = "+" + name
     return name.replace(':', '-')
 
 
-def _load_to_tracker(tracker, path):
+def _load_to_tracker(tracker, _path):
+    """Loads data from an output .csv file into
+    a Tracker object.
+
+    :param tracker: A tracker object to load the data into.
+    :type tracker: Tracker
+    :param _path: Path to data file.
+    :type _path: str
     """
-    Load a tracker object from a path.
-    :param tracker: a tracker object to load the data into.
-    :param path: path to data file.
-    """
-    with open(path, 'r') as file:
+    with open(_path, 'r') as file:
         for line in file.readlines():
             tracker.data.append(tuple([float(d) for d in line.replace('\n', '').split(',')]))
 
 
 def _generate_directory(dir_name, super_directory):
+    """Generates an output directory for a Monitor.
+    This function receives dir_name and super_directory, either can
+    potentially be None.
+    If super_directory is None, it defaults to a path such as sim_records/today's-date.
+    If dir_name is None, then the directory is given a generic name such as "S#", where #
+    is one more than the highest number that appears in super_directory.
+
+    The output directory is a combination of the two:
+    super_directory/dir_name.
+
+    If any of the directories along the path don't already exist, they are created.
+
+    :param dir_name: A directory name.
+    :type dir_name: str, None
+    :param super_directory: A super (outer) directory.
+    :type super_directory: str, None
+    :return: The constructed path of the generated directory.
+    :rtype: str
+    """
+
     if not super_directory:
         super_directory = f'sim_records/{str(date.today())}'
 
     _create_dir_path(super_directory)
 
     if not dir_name:
         # determine directory name
@@ -839,8 +1087,14 @@
 
     # create directory if it doesn't exist
     _create_dir_path(dir_path)
     return dir_path
 
 
 def _create_dir_path(dir_path):
+    """Provided with a path to a directory, this
+    function creates any directory along the path that doesn't already exist.
+
+    :param dir_path: A path to a directory.
+    :type dir_path: str
+    """
     Path(dir_path).mkdir(parents=True, exist_ok=True)
```

