# Comparing `tmp/lightweight_charts-1.0.4.tar.gz` & `tmp/lightweight_charts-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightweight_charts-1.0.4.tar", last modified: Wed May 17 11:47:22 2023, max compression
+gzip compressed data, was "lightweight_charts-1.0.5.tar", last modified: Thu May 18 22:31:05 2023, max compression
```

## Comparing `lightweight_charts-1.0.4.tar` & `lightweight_charts-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-17 11:47:22.426091 lightweight_charts-1.0.4/
--rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.4/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)     5915 2023-05-17 11:47:22.425666 lightweight_charts-1.0.4/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     5569 2023-05-16 14:49:40.000000 lightweight_charts-1.0.4/README.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-17 11:47:22.422606 lightweight_charts-1.0.4/lightweight_charts/
--rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.4/lightweight_charts/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     8733 2023-05-17 11:37:01.000000 lightweight_charts-1.0.4/lightweight_charts/chart.py
--rw-r--r--   0 louis      (501) staff       (20)    23893 2023-05-17 11:40:17.000000 lightweight_charts-1.0.4/lightweight_charts/js.py
--rw-r--r--   0 louis      (501) staff       (20)   141259 2023-05-09 19:50:25.000000 lightweight_charts-1.0.4/lightweight_charts/pkg.py
--rw-r--r--   0 louis      (501) staff       (20)     1761 2023-05-17 11:00:03.000000 lightweight_charts-1.0.4/lightweight_charts/pywebview.py
--rw-r--r--   0 louis      (501) staff       (20)     1753 2023-05-16 22:24:50.000000 lightweight_charts-1.0.4/lightweight_charts/util.py
--rw-r--r--   0 louis      (501) staff       (20)     1949 2023-05-17 11:44:38.000000 lightweight_charts-1.0.4/lightweight_charts/widgets.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-17 11:47:22.425083 lightweight_charts-1.0.4/lightweight_charts.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)     5915 2023-05-17 11:47:22.000000 lightweight_charts-1.0.4/lightweight_charts.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      434 2023-05-17 11:47:22.000000 lightweight_charts-1.0.4/lightweight_charts.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-17 11:47:22.000000 lightweight_charts-1.0.4/lightweight_charts.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-17 11:47:22.000000 lightweight_charts-1.0.4/lightweight_charts.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-17 11:47:22.000000 lightweight_charts-1.0.4/lightweight_charts.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-17 11:47:22.426281 lightweight_charts-1.0.4/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-17 11:46:48.000000 lightweight_charts-1.0.4/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-18 22:31:05.310106 lightweight_charts-1.0.5/
+-rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.5/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)     5915 2023-05-18 22:31:05.309531 lightweight_charts-1.0.5/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     5569 2023-05-16 14:49:40.000000 lightweight_charts-1.0.5/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-18 22:31:05.305142 lightweight_charts-1.0.5/lightweight_charts/
+-rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.5/lightweight_charts/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     9887 2023-05-18 22:28:08.000000 lightweight_charts-1.0.5/lightweight_charts/chart.py
+-rw-r--r--   0 louis      (501) staff       (20)    30005 2023-05-18 22:28:08.000000 lightweight_charts-1.0.5/lightweight_charts/js.py
+-rw-r--r--   0 louis      (501) staff       (20)   141259 2023-05-09 19:50:25.000000 lightweight_charts-1.0.5/lightweight_charts/pkg.py
+-rw-r--r--   0 louis      (501) staff       (20)     2535 2023-05-18 22:28:08.000000 lightweight_charts-1.0.5/lightweight_charts/pywebview.py
+-rw-r--r--   0 louis      (501) staff       (20)     2133 2023-05-18 22:28:08.000000 lightweight_charts-1.0.5/lightweight_charts/util.py
+-rw-r--r--   0 louis      (501) staff       (20)     1940 2023-05-18 22:28:08.000000 lightweight_charts-1.0.5/lightweight_charts/widgets.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-18 22:31:05.308864 lightweight_charts-1.0.5/lightweight_charts.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)     5915 2023-05-18 22:31:05.000000 lightweight_charts-1.0.5/lightweight_charts.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      434 2023-05-18 22:31:05.000000 lightweight_charts-1.0.5/lightweight_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-18 22:31:05.000000 lightweight_charts-1.0.5/lightweight_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-18 22:31:05.000000 lightweight_charts-1.0.5/lightweight_charts.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-18 22:31:05.000000 lightweight_charts-1.0.5/lightweight_charts.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-18 22:31:05.310319 lightweight_charts-1.0.5/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-18 22:01:10.000000 lightweight_charts-1.0.5/setup.py
```

### Comparing `lightweight_charts-1.0.4/LICENSE` & `lightweight_charts-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.4/PKG-INFO` & `lightweight_charts-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightweight_charts
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `lightweight_charts-1.0.4/README.md` & `lightweight_charts-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.4/lightweight_charts/chart.py` & `lightweight_charts-1.0.5/lightweight_charts/chart.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import pandas as pd
 import multiprocessing as mp
 from uuid import UUID
 from datetime import datetime
-from typing import Union
+from typing import Union, Literal
 
 from lightweight_charts.pywebview import _loop
 from lightweight_charts.util import LINE_TYPE, POSITION, SHAPE, CROSSHAIR_MODE, PRICE_SCALE_MODE
 
 
 class Line:
     def __init__(self, chart, line_id):
@@ -27,32 +27,33 @@
         :param series: labels: date/time, price
         """
         self._chart._go('_update_line_data', self.id, series)
 
 
 class Chart:
     def __init__(self, volume_enabled: bool = True, width: int = 800, height: int = 600, x: int = None, y: int = None,
-                 on_top: bool = False, debug: bool = False):
+                 on_top: bool = False, debug: bool = False, sub: bool = False, inner_width=1, inner_height=1):
         self.debug = debug
         self.volume_enabled = volume_enabled
         self.width = width
         self.height = height
         self.x = x
         self.y = y
         self.on_top = on_top
+        self.inner_width = inner_width
+        self.inner_height = inner_height
 
+        if sub:
+            return
         self._q = mp.Queue()
         self._result_q = mp.Queue()
         self._exit = mp.Event()
-
-        try:
-            self._process = mp.Process(target=_loop, args=(self,), daemon=True)
-            self._process.start()
-        except:
-            pass
+        self._process = mp.Process(target=_loop, args=(self,), daemon=True)
+        self._process.start()
+        self.id = self._result_q.get()
 
     def _go(self, func, *args): self._q.put((func, args))
 
     def _go_return(self, func, *args):
         self._q.put((func, args))
         return self._result_q.get()
 
@@ -157,22 +158,23 @@
         """
         :param mode: Chart price scale mode.
         :param title: Last price label text.
         :param right_padding: How many bars of empty space to the right of the last bar.
         """
         self._go('config', mode, title, right_padding)
 
-    def time_scale(self, time_visible: bool = True, seconds_visible: bool = False):
+    def time_scale(self, visible: bool = True, time_visible: bool = True, seconds_visible: bool = False):
         """
         Options for the time scale of the chart.
+        :param visible: Time scale visibility control.
         :param time_visible: Time visibility control.
         :param seconds_visible: Seconds visibility control
         :return:
         """
-        self._go('time_scale', time_visible, seconds_visible)
+        self._go('time_scale', visible, time_visible, seconds_visible)
 
     def layout(self, background_color: str = None, text_color: str = None, font_size: int = None,
                font_family: str = None):
         """
         Global layout options for the chart.
         """
         self._go('layout', background_color, text_color, font_size, font_family)
@@ -223,7 +225,33 @@
 
     def subscribe_click(self, function: object):
         """
         Subscribes the given function to a chart 'click' event.
         The event returns a dictionary containing the bar object at the time clicked.
         """
         self._go('subscribe_click', function)
+
+    def create_subchart(self, volume_enabled: bool = True, position: Literal['left', 'right', 'top', 'bottom'] = 'left',
+                         width: float = 0.5, height: float = 0.5, sync: bool | UUID = False):
+        c_id = self._go_return('create_sub_chart', volume_enabled, position, width, height, sync)
+        return SubChart(self, c_id)
+
+
+class SubChart(Chart):
+    def __init__(self, parent, c_id):
+        self._parent = parent._parent if isinstance(parent, SubChart) else parent
+
+        super().__init__(sub=True)
+
+        self.id = c_id
+        self._q = self._parent._q
+        self._result_q = self._parent._result_q
+
+    def _go(self, func, *args):
+        func = 'SUB'+func
+        args = (self.id,) + args
+        super()._go(func, *args)
+
+    def _go_return(self, func, *args):
+        func = 'SUB' + func
+        args = (self.id,) + args
+        return super()._go_return(func, *args)
```

### Comparing `lightweight_charts-1.0.4/lightweight_charts/js.py` & `lightweight_charts-1.0.5/lightweight_charts/js.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
-import uuid
+from uuid import UUID, uuid4
 from datetime import timedelta, datetime
-from typing import Dict, Union
+from typing import Dict, Union, Literal
 
 from lightweight_charts.pkg import LWC_3_5_0
 from lightweight_charts.util import LINE_TYPE, POSITION, SHAPE, CROSSHAIR_MODE, _crosshair_mode, _line_type, \
-    MissingColumn, _js_bool, _price_scale_mode, PRICE_SCALE_MODE, _position, _shape, IDGen
+    MissingColumn, _js_bool, _price_scale_mode, PRICE_SCALE_MODE, _position, _shape, IDGen, _valid_color
 
 
 class Line:
     def __init__(self, lwc, line_id, color, width):
         self._lwc = lwc
         self.loaded = False
         self.id = line_id
@@ -29,52 +29,59 @@
         :param series: labels: date/time, price
         """
         self._lwc._update_line_data(self.id, series)
 
 
 class API:
     def __init__(self):
-        self.click_func = None
+        self.click_funcs = {}
 
     def onClick(self, data):
+        click_func = self.click_funcs[data['id']]
         if isinstance(data['time'], int):
             data['time'] = datetime.fromtimestamp(data['time'])
         else:
             data['time'] = datetime(data['time']['year'], data['time']['month'], data['time']['day'])
-        self.click_func(data) if self.click_func else None
+        click_func(data) if click_func else None
 
 
 class LWC:
-    def __init__(self, volume_enabled):
+    def __init__(self, volume_enabled, inner_width=1, inner_height=1):
+        self.id = uuid4()
         self.js_queue = []
         self.loaded = False
-        self._html = HTML
+
         self._rand = IDGen()
+        self._chart_var = 'chart'
 
         self._js_api = API()
+        self._js_api_code = ''
 
         self.volume_enabled = volume_enabled
+        self.inner_width = inner_width
+        self.inner_height = inner_height
+        self._html = HTML.replace('__INNER_WIDTH__', str(self.inner_width)).replace('__INNER_HEIGHT__', str(self.inner_height))
+
         self.last_bar = None
         self.interval = None
-        self._lines: Dict[uuid.UUID, Line] = {}
+        self._lines: Dict[UUID, Line] = {}
+        self._subcharts: Dict[UUID, LWC] = {self.id: self}
 
         self.background_color = '#000000'
         self.volume_up_color = 'rgba(83,141,131,0.8)'
         self.volume_down_color = 'rgba(200,127,130,0.8)'
 
     def _on_js_load(self): pass
 
     def _stored(self, func, *args, **kwargs):
         if self.loaded:
             return False
         self.js_queue.append((func, args, kwargs))
         return True
 
-    def _click_func_code(self, string): self._html = self._html.replace('// __onClick__', string)
-
     def _set_last_bar(self, bar: pd.Series): self.last_bar = bar
 
     def _set_interval(self, df: pd.DataFrame):
         df['time'] = pd.to_datetime(df['time'])
         intervals = df['time'].diff()
         counts = intervals.value_counts()
         self.interval = counts.index[0]
@@ -119,19 +126,19 @@
                 raise MissingColumn("Volume enabled, but 'volume' column was not found.")
 
             volume = df.drop(columns=['open', 'high', 'low', 'close'])
             volume = volume.rename(columns={'volume': 'value'})
             volume['color'] = self.volume_down_color
             volume.loc[df['close'] > df['open'], 'color'] = self.volume_up_color
 
-            self.run_script(f'chart.volumeSeries.setData({volume.to_dict(orient="records")})')
+            self.run_script(f'{self._chart_var}.volumeSeries.setData({volume.to_dict(orient="records")})')
             bars = df.drop(columns=['volume'])
 
         bars = bars.to_dict(orient='records')
-        self.run_script(f'chart.series.setData({bars})')
+        self.run_script(f'{self._chart_var}.series.setData({bars})')
 
     def update(self, series, from_tick=False):
         """
         Updates the data from a bar;
         if series['time'] is the same time as the last bar, the last bar will be overwritten.\n
         :param series: columns: date/time, open, high, low, close, volume (if volume enabled).
         """
@@ -143,19 +150,19 @@
         if self.volume_enabled:
             if 'volume' not in series:
                 raise MissingColumn("Volume enabled, but 'volume' column was not found.")
 
             volume = series.drop(['open', 'high', 'low', 'close'])
             volume = volume.rename({'volume': 'value'})
             volume['color'] = self.volume_up_color if series['close'] > series['open'] else self.volume_down_color
-            self.run_script(f'chart.volumeSeries.update({volume.to_dict()})')
+            self.run_script(f'{self._chart_var}.volumeSeries.update({volume.to_dict()})')
             series = series.drop(['volume'])
 
         dictionary = series.to_dict()
-        self.run_script(f'chart.series.update({dictionary})')
+        self.run_script(f'{self._chart_var}.series.update({dictionary})')
 
     def update_from_tick(self, series):
         """
         Updates the data from a tick.\n
         :param series: columns: date/time, price, volume (if volume enabled).
         """
         if self._stored('update_from_tick', series):
@@ -180,33 +187,32 @@
         self.update(bar, from_tick=True)
 
     def create_line(self, color: str = 'rgba(214, 237, 255, 0.6)', width: int = 2):
         """
         Creates and returns a Line object.)\n
         :return a Line object used to set/update the line.
         """
-        line_id = uuid.uuid4()
+        line_id = uuid4()
         self._lines[line_id] = Line(self, line_id, color, width)
         return self._lines[line_id]
 
     def _set_line_data(self, line_id, df: pd.DataFrame):
         if self._stored('_set_line_data', line_id, df):
             return None
-
         line = self._lines[line_id]
 
         if not line.loaded:
             var = self._rand.generate()
             self.run_script(f'''
             let lineSeries{var} = {{
                     color: '{line.color}',
                     lineWidth: {line.width},
                     }};
             let line{var} = {{
-                series: chart.chart.addLineSeries(lineSeries{var}),
+                series: {self._chart_var}.chart.addLineSeries(lineSeries{var}),
                 id: '{line_id}',
             }};
             lines.push(line{var})
                 ''')
             line.loaded = True
         df = self._df_datetime_format(df)
         self.run_script(f'''
@@ -225,56 +231,61 @@
         lines.forEach(function (line) {{
             if ('{line_id}' === line.id) {{
                 line.series.update({series.to_dict()})
             }}
         }})''')
 
     def marker(self, time: datetime = None, position: POSITION = 'below', shape: SHAPE = 'arrow_up',
-               color: str = '#2196F3', text: str = '', m_id: uuid.UUID = None) -> uuid.UUID:
+               color: str = '#2196F3', text: str = '', m_id: UUID = None) -> UUID:
         """
         Creates a new marker.\n
         :param time: The time that the marker will be placed at. If no time is given, it will be placed at the last bar.
         :param position: The position of the marker.
         :param color: The color of the marker (rgb, rgba or hex).
         :param shape: The shape of the marker.
         :param text: The text to be placed with the marker.
         :return: The UUID of the marker placed.
         """
+        _valid_color(color)
         if not m_id:
-            m_id = uuid.uuid4()
+            m_id = uuid4()
         if self._stored('marker', time, position, shape, color, text, m_id):
             return m_id
 
-        time = self.last_bar['time'] if not time else self._datetime_format(time)
+        try:
+            time = self.last_bar['time'] if not time else self._datetime_format(time)
+        except TypeError:
+            raise TypeError('Chart marker created before data was set.')
+        time = time if isinstance(time, float) else f"'{time}'"
 
         self.run_script(f"""
                 markers.push({{
-                    time: '{time}',
+                    time: {time},
                     position: '{_position(position)}',
                     color: '{color}', shape: '{_shape(shape)}',
                     text: '{text}',
                     id: '{m_id}'
                     }});
-                chart.series.setMarkers(markers)""")
+                {self._chart_var}.series.setMarkers(markers)""")
         return m_id
 
-    def remove_marker(self, m_id: uuid.UUID):
+    def remove_marker(self, m_id: UUID):
         """
-        Removes the marker with the given uuid.\n
+        Removes the marker with the given UUID.\n
         """
         if self._stored('remove_marker', m_id):
             return None
 
         self.run_script(f'''
-                       markers.forEach(function (marker) {{
-                           if ('{m_id}' === marker.id) {{
-                               markers.splice(markers.indexOf(marker), 1)
-                               chart.series.setMarkers(markers)
-                               }}
-                           }});''')
+               markers.forEach(function (marker) {{
+                   if ('{m_id}' === marker.id) {{
+                       markers.splice(markers.indexOf(marker), 1)
+                       {self._chart_var}.series.setMarkers(markers)
+                       }}
+                   }});''')
 
     def horizontal_line(self, price: Union[float, int], color: str = 'rgb(122, 146, 202)', width: int = 1,
                         style: LINE_TYPE = 'solid', text: str = '', axis_label_visible=True):
         """
         Creates a horizontal line at the given price.\n
         """
         if self._stored('horizontal_line', price, color, width, style, text, axis_label_visible):
@@ -287,112 +298,111 @@
                    color: '{color}',
                    lineWidth: {width},
                    lineStyle: LightweightCharts.LineStyle.{style},
                    axisLabelVisible: {'true' if axis_label_visible else 'false'},
                    title: '{text}',
                }};
                let line{var} = {{
-                   line: chart.series.createPriceLine(priceLine{var}),
+                   line: {self._chart_var}.series.createPriceLine(priceLine{var}),
                    price: {price},
                }};
                horizontal_lines.push(line{var})""")
 
     def remove_horizontal_line(self, price: Union[float, int]):
         """
         Removes a horizontal line at the given price.
         """
         if self._stored('remove_horizontal_line', price):
             return None
 
         self.run_script(f'''
                horizontal_lines.forEach(function (line) {{
                if ({price} === line.price) {{
-                   chart.series.removePriceLine(line.line);
+                   {self._chart_var}.series.removePriceLine(line.line);
                    horizontal_lines.splice(horizontal_lines.indexOf(line), 1)
                    }}
                }});''')
 
     def config(self, mode: PRICE_SCALE_MODE = None, title: str = None, right_padding: float = None):
         """
         :param mode: Chart price scale mode.
         :param title: Last price label text.
         :param right_padding: How many bars of empty space to the right of the last bar.
         """
         if self._stored('config', mode, title, right_padding):
             return None
 
-        self.run_script(f'chart.chart.timeScale().scrollToPosition({right_padding}, false)') if right_padding else None
-        self.run_script(f'chart.series.applyOptions({{title: "{title}"}})') if title else None
+        self.run_script(f'{self._chart_var}.chart.timeScale().scrollToPosition({right_padding}, false)') if right_padding else None
+        self.run_script(f'{self._chart_var}.series.applyOptions({{title: "{title}"}})') if title else None
         self.run_script(
-            f"chart.chart.priceScale().applyOptions({{mode: LightweightCharts.PriceScaleMode.{_price_scale_mode(mode)}}})") if mode else None
+            f"{self._chart_var}.chart.priceScale().applyOptions({{mode: LightweightCharts.PriceScaleMode.{_price_scale_mode(mode)}}})") if mode else None
 
-    def time_scale(self, time_visible: bool = True, seconds_visible: bool = False):
+    def time_scale(self, visible: bool = True, time_visible: bool = True, seconds_visible: bool = False):
         """
         Options for the time scale of the chart.
+        :param visible: Time scale visibility control.
         :param time_visible: Time visibility control.
-        :param seconds_visible: Seconds visibility control
+        :param seconds_visible: Seconds visibility control.
         :return:
         """
-        if self._stored('time_scale', time_visible, seconds_visible):
+        if self._stored('time_scale', visible, time_visible, seconds_visible):
             return None
 
+        time_scale_visible = f'visible: {_js_bool(visible)},'
         time = f'timeVisible: {_js_bool(time_visible)},'
-        seconds = f'secondsVisible: {_js_bool(seconds_visible)}'
+        seconds = f'secondsVisible: {_js_bool(seconds_visible)},'
         self.run_script(f'''
-           chart.chart.applyOptions({{
+           {self._chart_var}.chart.applyOptions({{
                timeScale: {{
+               {time_scale_visible if visible is not None else ''}
                {time if time_visible is not None else ''}
                {seconds if seconds_visible is not None else ''}
                }}
            }})''')
 
     def layout(self, background_color: str = None, text_color: str = None, font_size: int = None,
                font_family: str = None):
         """
         Global layout options for the chart.
         """
         if self._stored('layout', background_color, text_color, font_size, font_family):
             return None
 
         self.background_color = background_color if background_color else self.background_color
-        args = f"'{self.background_color}'", f"'{text_color}'", f"{font_size}", f"'{font_family}'",
-        for key, arg in zip(('backgroundColor', 'textColor', 'fontSize', 'fontFamily'), args):
-            if not arg:
-                continue
-            self.run_script(f"""
-                  chart.chart.applyOptions({{
-                     layout: {{
-                          {key}: {arg}
-                     }} 
-                  }})""")
+        self.run_script(f"""
+            document.body.style.backgroundColor = '{self.background_color}'
+            {self._chart_var}.chart.applyOptions({{
+            layout: {{
+                {f'backgroundColor: "{background_color}",' if background_color else ''}
+                {f'textColor: "{text_color}",' if text_color else ''}
+                {f'fontSize: {font_size},' if font_size else ''}
+                {f'fontFamily: "{font_family}",' if font_family else ''}
+            }}}})""")
 
     def candle_style(self, up_color: str = 'rgba(39, 157, 130, 100)', down_color: str = 'rgba(200, 97, 100, 100)',
                      wick_enabled: bool = True, border_enabled: bool = True, border_up_color: str = '',
                      border_down_color: str = '', wick_up_color: str = '', wick_down_color: str = ''):
         """
         Candle styling for each of its parts.
         """
         if self._stored('candle_style', up_color, down_color, wick_enabled, border_enabled,
                         border_up_color, border_down_color, wick_up_color, wick_down_color):
             return None
 
-        params = None, 'upColor', 'downColor', 'wickVisible', 'borderVisible', 'borderUpColor', 'borderDownColor',\
-                 'wickUpColor', 'wickDownColor'
-        for param, key_arg in zip(params, locals().items()):
-            key, arg = key_arg
-            if isinstance(arg, bool):
-                arg = _js_bool(arg)
-            if key == 'self' or arg is None:
-                continue
-            else:
-                arg = f"'{arg}'"
-            self.run_script(
-                f"""chart.series.applyOptions({{
-                    {param}: {arg},
-                    }})""")
+        self.run_script(f"""
+            {self._chart_var}.series.applyOptions({{
+                {f'upColor: "{up_color}",' if up_color else ''}
+                {f'downColor: "{down_color}",' if down_color else ''}
+                {f'wickVisible: {_js_bool(wick_enabled)},' if wick_enabled else ''}
+                {f'borderVisible: {_js_bool(border_enabled)},' if border_enabled else ''}
+                {f'borderUpColor: "{border_up_color}",' if border_up_color else ''}
+                {f'borderDownColor: "{border_down_color}",' if border_down_color else ''}
+                {f'wickUpColor: "{wick_up_color}",' if wick_up_color else ''}
+                {f'wickDownColor: "{wick_down_color}",' if wick_down_color else ''}
+            }})""")
 
     def volume_config(self, scale_margin_top: float = 0.8, scale_margin_bottom: float = 0.0,
                       up_color='rgba(83,141,131,0.8)', down_color='rgba(200,127,130,0.8)'):
         """
         Configure volume settings.\n
         Numbers for scaling must be greater than 0 and less than 1.\n
         Volume colors must be applied prior to setting/updating the bars.\n
@@ -402,21 +412,19 @@
         :param down_color: Volume color for downward direction (rgb, rgba or hex)
         """
         if self._stored('volume_config', scale_margin_top, scale_margin_bottom, up_color, down_color):
             return None
 
         self.volume_up_color = up_color if up_color else self.volume_up_color
         self.volume_down_color = down_color if down_color else self.volume_down_color
-        top = f'top: {scale_margin_top},'
-        bottom = f'bottom: {scale_margin_bottom},'
         self.run_script(f'''
-        chart.volumeSeries.priceScale().applyOptions({{
+        {self._chart_var}.volumeSeries.priceScale().applyOptions({{
             scaleMargins: {{
-            {top if top else ''}
-            {bottom if bottom else ''}
+            top: {scale_margin_top},
+            bottom: {scale_margin_bottom},
             }}
         }})''')
 
     def crosshair(self, mode: CROSSHAIR_MODE = 'normal', vert_width: int = 1, vert_color: str = None,
                   vert_style: LINE_TYPE = None, vert_label_background_color: str = None, horz_width: int = 1,
                   horz_color: str = None, horz_style: LINE_TYPE = None, horz_label_background_color: str = None):
         """
@@ -427,35 +435,34 @@
             return None
 
         args = f"LightweightCharts.CrosshairMode.{_crosshair_mode(mode)}", \
                f"{vert_width}}}", f"'{vert_color}'}}", f"LightweightCharts.LineStyle.{_line_type(vert_style)}}}",\
                f"'{vert_label_background_color}'}}", \
                f"{horz_width}}}", f"'{horz_color}'}}", f"LightweightCharts.LineStyle.{_line_type(horz_style)}}}",\
                f"'{horz_label_background_color}'}}"
-
         for key, arg in zip(
                 ('mode', 'vertLine: {width', 'vertLine: {color', 'vertLine: {style', 'vertLine: {labelBackgroundColor',
                  'horzLine: {width', 'horzLine: {color', 'horzLine: {style', 'horzLine: {labelBackgroundColor'), args):
             if 'None' in arg:
                 continue
             self.run_script(f'''
-            chart.chart.applyOptions({{
+            {self._chart_var}.chart.applyOptions({{
                 crosshair: {{
                     {key}: {arg}
             }}}})''')
 
     def watermark(self, text: str, font_size: int = 44, color: str = 'rgba(180, 180, 200, 0.5)'):
         """
         Adds a watermark to the chart.
         """
         if self._stored('watermark', text, font_size, color):
             return None
 
         self.run_script(f'''
-          chart.chart.applyOptions({{
+          {self._chart_var}.chart.applyOptions({{
               watermark: {{
                   visible: true,
                   fontSize: {font_size},
                   horzAlign: 'center',
                   vertAlign: 'center',
                   color: '{color}',
                   text: '{text}',
@@ -466,35 +473,168 @@
                font_size: int = None, font_family: str = None):
         """
         Configures the legend of the chart.
         """
         if self._stored('legend', visible, ohlc, percent, color, font_size, font_family):
             return None
 
-        scripts = f'legendToggle = {_js_bool(visible)}; legend.innerText = ""', f'legendOHLCVisible = {_js_bool(ohlc)}',\
-                  f'legendPercentVisible = {_js_bool(percent)}', f'legend.style.color = {color}', \
-                  f'legend.style.fontSize = "{font_size}px"', f'legend.style.fontFamily = "{font_family}"'
-        for script, arg in zip(scripts, (visible, ohlc, percent, color, font_size, font_family)):
-            if arg is None:
-                continue
-            self.run_script(script)
+        if visible:
+            self.run_script(f'''
+            {f"{self._chart_var}.legend.style.color = '{color}'" if color else ''}
+            {f"{self._chart_var}.legend.style.fontSize = {font_size}" if font_size else ''}
+            {f"{self._chart_var}.legend.style.fontFamily = '{font_family}'" if font_family else ''}
+            
+            {self._chart_var}.chart.subscribeCrosshairMove((param) => {{   
+                if (param.time){{
+                    const data = param.seriesPrices.get({self._chart_var}.series);
+                    if (!data) {{return}}
+                    let percentMove = ((data.close-data.open)/data.open)*100
+                    let ohlc = `open: ${{legendItemFormat(data.open)}} 
+                                | high: ${{legendItemFormat(data.high)}} 
+                                | low: ${{legendItemFormat(data.low)}}
+                                | close: ${{legendItemFormat(data.close)}} `
+                    let percent = `| daily: ${{percentMove >= 0 ? '+' : ''}}${{percentMove.toFixed(2)}} %`
+                    let finalString = ''
+                    {'finalString += ohlc' if ohlc else ''}
+                    {'finalString += percent' if percent else ''}
+                    {self._chart_var}.legend.innerHTML = finalString
+                }}
+                else {{
+                    {self._chart_var}.legend.innerHTML = ''
+                }}
+            }});''')
 
     def subscribe_click(self, function: object):
         if self._stored('subscribe_click', function):
             return None
 
-        self._js_api.click_func = function
-        self.run_script('isSubscribed = true')
+        self._js_api.click_funcs[str(self.id)] = function
+        var = self._rand.generate()
+        self.run_script(f'''
+            {self._chart_var}.chart.subscribeClick((param) => {{
+                if (!param.point) {{return}}
+                let prices{var} = param.seriesPrices.get({self._chart_var}.series);
+                let data{var} = {{
+                    time: param.time,
+                    open: prices{var}.open,
+                    high: prices{var}.high,
+                    low: prices{var}.low,
+                    close: prices{var}.close,
+                    id: '{self.id}'
+                    }}
+                {self._js_api_code}(data{var})
+                }})''')
+
+    def create_sub_chart(self, volume_enabled: bool = True, position: Literal['left', 'right', 'top', 'bottom'] = 'left',
+                         width: float = 0.5, height: float = 0.5, sync: bool | UUID = False):
+        subchart = SubChart(self, volume_enabled, position, width, height, sync)
+        self._subcharts[subchart.id] = subchart
+        return subchart
+
+    def _pywebview_sub_chart(self, volume_enabled, position, width, height, sync, parent=None):
+        subchart = PyWebViewSubChart(self if not parent else parent, volume_enabled, position, width, height, sync)
+        self._subcharts[subchart.id] = subchart
+        return subchart.id
+
+
+class SubChart(LWC):
+    def __init__(self, parent, volume_enabled, position, width, height, sync):
+        super().__init__(volume_enabled, width, height)
+        self._chart = parent._chart if isinstance(parent, SubChart) else parent
+        self._parent = parent
+
+        self._rand = self._chart._rand
+        self._chart_var = self._rand.generate()
+        self._js_api = self._chart._js_api
+        self._js_api_code = self._chart._js_api_code
+
+        self.position = position
+
+        self._create_panel(sync)
+
+    def _stored(self, func, *args, **kwargs):
+        if self._chart.loaded:
+            return False
+        self._chart.js_queue.append((f'SUB{func}', (self.id,)+args, kwargs))
+        return True
+
+    def run_script(self, script): self._chart.run_script(script)
+
+    def _create_panel(self, sync):
+        if self._stored('_create_panel', sync):
+            return None
+
+        parent_div = 'chartsDiv' if self._parent._chart_var == 'chart' else self._parent._chart_var+'div'
+
+        sub_sync = ''
+        if sync:
+            sync_parent_var = self._chart._subcharts[sync]._chart_var if isinstance(sync, UUID) else self._parent._chart_var
+            sub_sync = f'''
+                {sync_parent_var}.chart.timeScale().subscribeVisibleLogicalRangeChange((timeRange) => {{
+                    {self._chart_var}.chart.timeScale().setVisibleLogicalRange(timeRange)
+                }});
+            '''
+        self.run_script(f'''
+            var {self._chart_var}div = document.createElement('div')
+            //{self._chart_var}div.style.position = 'relative'
+            {self._chart_var}div.style.float = "{self.position}"
+            
+            //chartsDiv.style.display = 'inline-block'
+            chartsDiv.style.float = 'left'
+            
+            var {self._chart_var} = {{}}
+            {self._chart_var}.scale= {{
+                width: {self.inner_width},
+                height: {self.inner_height}
+            }}
+            {self._chart_var}.chart = makeChart(window.innerWidth*{self._chart_var}.scale.width,
+                                        window.innerHeight*{self._chart_var}.scale.height, {self._chart_var}div)
+            {self._chart_var}.series = makeCandlestickSeries({self._chart_var}.chart)
+            {self._chart_var}.volumeSeries = makeVolumeSeries({self._chart_var}.chart)
+    
+            {self._chart_var}.legend = document.createElement('div')
+            {self._chart_var}.legend.style.position = 'absolute'
+            {self._chart_var}.legend.style.zIndex = 1000
+            {self._chart_var}.legend.style.width = '{(self.inner_width*100)-8}vw'
+            {self._chart_var}.legend.style.top = '10px'
+            {self._chart_var}.legend.style.left = '10px'
+            {self._chart_var}.legend.style.fontFamily = 'Monaco'
+            {self._chart_var}.legend.style.fontSize = '11px'
+            {self._chart_var}.legend.style.color = 'rgb(191, 195, 203)'
+            {self._chart_var}div.appendChild({self._chart_var}.legend)
+            
+            {parent_div}.parentNode.insertBefore({self._chart_var}div, {parent_div}.nextSibling)
+            charts.push({self._chart_var})
+            
+            {self._chart_var}.chart.priceScale('').applyOptions({{
+             scaleMargins: {{
+                top: 0.8,
+                bottom: 0,
+                }}
+            }});
+            {sub_sync}
+            ''')
+
+
+class PyWebViewSubChart(SubChart):
+    def create_sub_chart(self, volume_enabled: bool = True, position: Literal['left', 'right', 'top', 'bottom'] = 'left',
+                         width: float = 0.5, height: float = 0.5, sync: bool | UUID = False):
+        return self._chart._pywebview_sub_chart(volume_enabled, position, width, height, sync, parent=self)
+
+    def create_line(self, color: str = 'rgba(214, 237, 255, 0.6)', width: int = 2):
+        return super().create_line(color, width).id
 
 
 SCRIPT = """
+document.body.style.backgroundColor = '#000000'
 
 const markers = []
 const horizontal_lines = []
 const lines = []
+const charts = []
 
 const up = 'rgba(39, 157, 130, 100)'
 const down = 'rgba(200, 97, 100, 100)'
 
 
 function makeChart(width, height, div) {
     return LightweightCharts.createChart(div, {
@@ -553,106 +693,73 @@
     },
     priceScaleId: '',
 });
 }
 
 const chartsDiv = document.createElement('div')
 
+var chart = {}
+
 chart.chart = makeChart(window.innerWidth, window.innerHeight, chartsDiv)
 chart.series = makeCandlestickSeries(chart.chart)
 chart.volumeSeries = makeVolumeSeries(chart.chart)
+chart.scale = {
+    width: __INNER_WIDTH__,
+    height: __INNER_HEIGHT__
+}
             
 document.body.appendChild(chartsDiv)
 
-const legend = document.createElement('div')
-legend.style.display = 'block'
-legend.style.position = 'absolute'
-legend.style.zIndex = 1000
-legend.style.width = '98vw'
-legend.style.top = '10px'
-legend.style.left = '10px'
-legend.style.fontFamily = 'Monaco'
-
-legend.style.fontSize = '11px'
-legend.style.color = 'rgb(191, 195, 203)'
-
-document.body.appendChild(legend)
+chart.legend = document.createElement('div')
+chart.legend.style.position = 'absolute'
+chart.legend.style.zIndex = 1000
+chart.legend.style.width = `${(chart.scale.width*100)-8}vw`
+chart.legend.style.top = '10px'
+chart.legend.style.left = '10px'
+chart.legend.style.fontFamily = 'Monaco'
+chart.legend.style.fontSize = '11px'
+chart.legend.style.color = 'rgb(191, 195, 203)'
+document.body.appendChild(chart.legend)
 
 chart.chart.priceScale('').applyOptions({
     scaleMargins: {
         top: 0.8,
         bottom: 0,
     }
 });
 
 window.addEventListener('resize', function() {
     let width = window.innerWidth;
     let height = window.innerHeight;
-    chart.chart.resize(width, height)
+    chart.chart.resize(width*chart.scale.width, height*chart.scale.height)
+    
+    charts.forEach(function (subchart) {{
+        subchart.chart.resize(width*subchart.scale.width, height*subchart.scale.height)
+        }});
+    
 });
 
 function legendItemFormat(num) {
     return num.toFixed(2).toString().padStart(8, ' ')
 }
-let legendToggle = false
-let legendOHLCVisible = true
-let legendPercentVisible = true
-chart.chart.subscribeCrosshairMove((param) => {
-    if (param.time){
-        const data = param.seriesPrices.get(chart.series);
-        if (!data || legendToggle === false) {return}
-        const percentMove = ((data.close-data.open)/data.open)*100
-        //legend.style.color = percentMove >= 0 ? up : down
-        
-        let ohlc = `open: ${legendItemFormat(data.open)} 
-                    | high: ${legendItemFormat(data.high)} 
-                    | low: ${legendItemFormat(data.low)} 
-                    | close: ${legendItemFormat(data.close)} `
-        let percent = `| daily: ${percentMove >= 0 ? '+' : ''}${percentMove.toFixed(2)} %`
-        
-        let finalString = ''
-        if (legendOHLCVisible) {
-            finalString += ohlc
-        }
-        if (legendPercentVisible) {
-            finalString += percent
-        }
-        legend.innerHTML = finalString
-    }
-    else {
-        legend.innerHTML = ''
-    }
-});
-let isSubscribed = false
-function clickHandler(param) {
-    if (!param.point || !isSubscribed) {return}
-    let prices = param.seriesPrices.get(chart.series);
-    let data = {
-        time: param.time,
-        open: prices.open,
-        high: prices.high,
-        low: prices.low,
-        close: prices.close,
-    }
-    // __onClick__
 
-}
-chart.chart.subscribeClick(clickHandler)
 """
 
 HTML = f"""
 <!DOCTYPE html>
 <html lang="">
 <head>
     <title>lightweight-charts-python</title>
     <script>{LWC_3_5_0}</script>
     <meta name="viewport" content ="width=device-width, initial-scale=1">
     <style>
     body {{
         margin: 0;
+        padding: 0;
+        overflow: hidden;
     }}
     </style>
 </head>
 <body>
 <div id="chart"></div>
 <script>
 {SCRIPT}
```

### Comparing `lightweight_charts-1.0.4/lightweight_charts/pkg.py` & `lightweight_charts-1.0.5/lightweight_charts/pkg.py`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.4/lightweight_charts/util.py` & `lightweight_charts-1.0.5/lightweight_charts/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,29 @@
         super().__init__(message)
         self.msg = message
 
     def __str__(self):
         return f'{self.msg}'
 
 
+class ColorError(ValueError):
+    def __init__(self, message):
+        super().__init__(message)
+        self.msg = message
+
+    def __str__(self):
+        return f'{self.msg}'
+
+
+def _valid_color(string):
+    if string[:3] == 'rgb' or string[:4] == 'rgba' or string[0] == '#':
+        return True
+    raise ColorError('Colors must be in the format of either rgb, rgba or hex.')
+
+
 LINE_TYPE = Literal['solid', 'dotted', 'dashed', 'large_dashed', 'sparse_dotted']
 
 POSITION = Literal['above', 'below', 'inside']
 
 SHAPE = Literal['arrow_up', 'arrow_down', 'circle', 'square']
 
 CROSSHAIR_MODE = Literal['normal', 'magnet']
```

### Comparing `lightweight_charts-1.0.4/lightweight_charts/widgets.py` & `lightweight_charts-1.0.5/lightweight_charts/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             self.webview: wx.html2.WebView = wx.html2.WebView.New(parent)
         except NameError:
             raise ModuleNotFoundError('wx.html2 was not found, and must be installed to use WxChart.')
 
         super().__init__(volume_enabled)
 
         self.webview.AddScriptMessageHandler('wx_msg')
-        self._click_func_code('window.wx_msg.postMessage(data)')
+        self._js_api_code = 'window.wx_msg.postMessage'
         self.webview.Bind(wx.html2.EVT_WEBVIEW_SCRIPT_MESSAGE_RECEIVED, lambda e: self._js_api.onClick(eval(e.GetString())))
 
         self.webview.Bind(wx.html2.EVT_WEBVIEW_LOADED, self._on_js_load)
         self.webview.SetPage(self._html, '')
 
     def run_script(self, script): self.webview.RunScript(script)
```

### Comparing `lightweight_charts-1.0.4/lightweight_charts.egg-info/PKG-INFO` & `lightweight_charts-1.0.5/lightweight_charts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightweight-charts
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `lightweight_charts-1.0.4/setup.py` & `lightweight_charts-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='lightweight_charts',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     python_requires='>=3.9',
     install_requires=[
         'pandas',
         'pywebview',
     ],
     author='louisnw',
```

