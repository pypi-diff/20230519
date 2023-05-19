# Comparing `tmp/speedtab-0.1.3.0.tar.gz` & `tmp/speedtab-0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.3.0.tar", max compression
+gzip compressed data, was "speedtab-0.1.3.1.tar", max compression
```

## Comparing `speedtab-0.1.3.0.tar` & `speedtab-0.1.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-05-16 16:02:58.325475 speedtab-0.1.3.0/pyproject.toml
--rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.3.0/speedtab/__init__.py
--rw-r--r--   0        0        0    45758 2023-05-16 16:01:38.620493 speedtab-0.1.3.0/speedtab/client.py
--rw-r--r--   0        0        0     5857 2022-10-11 09:11:17.745858 speedtab-0.1.3.0/speedtab/enums.py
--rw-r--r--   0        0        0     1744 2022-08-23 18:18:16.848628 speedtab-0.1.3.0/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-05-16 16:03:56.700500 speedtab-0.1.3.0/setup.py
--rw-r--r--   0        0        0      808 2023-05-16 16:03:56.701500 speedtab-0.1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-05-19 11:17:12.096613 speedtab-0.1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.3.1/speedtab/__init__.py
+-rw-r--r--   0        0        0    45415 2023-05-19 11:33:22.981049 speedtab-0.1.3.1/speedtab/client.py
+-rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.3.1/speedtab/enums.py
+-rw-r--r--   0        0        0     1730 2023-05-19 11:23:08.076916 speedtab-0.1.3.1/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-05-19 11:46:14.721776 speedtab-0.1.3.1/setup.py
+-rw-r--r--   0        0        0      808 2023-05-19 11:46:14.721776 speedtab-0.1.3.1/PKG-INFO
```

### Comparing `speedtab-0.1.3.0/pyproject.toml` & `speedtab-0.1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.3.0"
+version = "0.1.3.1"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.3.0/speedtab/client.py` & `speedtab-0.1.3.1/speedtab/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import re
 from collections.abc import Iterable
 from datetime import datetime, date
-from enum import Enum
 from itertools import zip_longest
 from typing import Union
 
-import pandas as pd
 import numpy as np
+import pandas as pd
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 
 from speedtab.enums import MergeType, BorderStyle, HorizontalAlignment, VerticalAlignment, WrapStrategy, ShareRole, \
-    ChartType, StackedType, LegendPosition, AxisPosition, BooleanConditionTypes
+    ChartType, StackedType, LegendPosition, AxisPosition, BooleanConditionTypes, BorderSides
 from speedtab.formats import Color, Border, Number, BaseNumberFormat
 
 SCOPES = ['https://www.googleapis.com/auth/spreadsheets', 'https://www.googleapis.com/auth/drive', 'https://www.googleapis.com/auth/drive.file']
-BORDER_SIDES = ('top', 'bottom', 'left', 'right', 'innerHorizontal', 'innerVertical')
 SHIFT_DIM = {
     'startRowIndex': 0,
     'startColumnIndex': 0,
     'endRowIndex': 1,
     'endColumnIndex': 1,
 }
 
@@ -102,15 +100,15 @@
         return max(map(depth, l)) + 1
     else:
         return 0
 
 
 class BooleanCondition:
     def __init__(self, type: BooleanConditionTypes, value):
-        self.type = type.value
+        self.type = type
         self.value = value
 
     def boolean_condition(self):
         return {
             'booleanRule': {
                 'condition': {
                     'type': self.type,
@@ -333,15 +331,15 @@
                             'startColumnIndex': data_start_cell[1] + column,
                             'endColumnIndex': data_start_cell[1] + column + 1,
                         }
                     ]
                 }
             },
             'targetAxis': 'LEFT_AXIS',
-            'type': chart_type_left.value,
+            'type': chart_type_left,
         } for column in left_columns] + [{
             'series': {
                 'sourceRange': {
                     'sources': [
                         {
                             'sheetId': self.sheet_id if not data_sheet_name else self.base.sheets.get(data_sheet_name).get('sheetId'),
                             'startRowIndex': data_start_cell[0],
@@ -349,26 +347,26 @@
                             'startColumnIndex': data_start_cell[1] + column,
                             'endColumnIndex': data_start_cell[1] + column + 1,
                         }
                     ]
                 }
             },
             'targetAxis': 'RIGHT_AXIS',
-            'type': chart_type_right.value,
+            'type': chart_type_right,
         } for column in right_columns]
 
         self._task_queue.append(Task('chart', self._increment_task(), self.sheet_id, {
             'addChart': {
                 'chart': {
                     'spec': {
                         'title': title,
                         'basicChart': {
                             'chartType': 'COMBO',
-                            'stackedType': stacked_type.value,
-                            'legendPosition': legend_position.value,
+                            'stackedType': stacked_type,
+                            'legendPosition': legend_position,
                             'axis': [
                                 {
                                     'position': 'BOTTOM_AXIS',
                                     'title': x_axis_name,
                                 },
                                 {
                                     'position': 'LEFT_AXIS',
@@ -460,42 +458,42 @@
                             'endRowIndex': data_start_cell[0] + nrows + 1 if nrows is not None else None,
                             'startColumnIndex': data_start_cell[1] + column,
                             'endColumnIndex': data_start_cell[1] + column + 1,
                         }
                     ]
                 }
             },
-            'targetAxis': axis.value
+            'targetAxis': axis
         } for column, axis in zip_longest(columns, target_axis, fillvalue=target_axis[0])]
 
         self._task_queue.append(Task('chart', self._increment_task(), self.sheet_id, {
             'addChart': {
                 'chart': {
                     'spec': {
                         'title': title,
                         'basicChart': {
-                            'chartType': chart_type.value,
-                            'stackedType': stacked_type.value,
-                            'legendPosition': legend_position.value,
+                            'chartType': chart_type,
+                            'stackedType': stacked_type,
+                            'legendPosition': legend_position,
                             'axis': [
                                 {
                                     'position': 'BOTTOM_AXIS',
                                     'title': x_axis_name,
                                 },
                                 {
-                                    'position': AxisPosition.LEFT_AXIS.value,
+                                    'position': AxisPosition.LEFT_AXIS,
                                     'title': y_left_axis_name,
                                     'viewWindowOptions': {
                                         'viewWindowMode': 'EXPLICIT',
                                         'viewWindowMin': y_left_axis_min,
                                         'viewWindowMax': y_left_axis_max,
                                     },
                                 },
                                 {
-                                    'position': AxisPosition.RIGHT_AXIS.value,
+                                    'position': AxisPosition.RIGHT_AXIS,
                                     'title': y_right_axis_name,
                                     'viewWindowOptions': {
                                         'viewWindowMode': 'EXPLICIT',
                                         'viewWindowMin': y_right_axis_min,
                                         'viewWindowMax': y_right_axis_max,
                                     },
                                 },
@@ -610,15 +608,15 @@
             }
         }, self.work_zone))
         return self
 
     def merge_cells(self, merge_type: MergeType = MergeType.MERGE_ALL):
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'mergeCells': {
-                    'mergeType': merge_type.value,
+                    'mergeType': merge_type,
                     'range': self.work_zone
                 }}, self.work_zone))
         return self
 
     def read_cell_details(self):
         return (self.base.connect_v4.spreadsheets()
         .get(spreadsheetId=self.base.spreadsheet_id,
@@ -656,32 +654,35 @@
                     },
                     'fields': 'userEnteredFormat, userEnteredValue',
                     'rows': copied_data
                 }}, self.work_zone))
         return self
 
     def set_background_color(self, color: Color = Color((255, 255, 255))):
-        color = color.value if isinstance(color, Enum) else color
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'repeatCell': {
                     'range': self.work_zone,
                     'cell': {
                         'userEnteredFormat': {
                             'backgroundColor': color.color
                         }},
                     'fields': 'userEnteredFormat(backgroundColor)',
                 }}, self.work_zone))
         return self
 
     def set_borders(self, border_style: BorderStyle = BorderStyle.SOLID,
                     border_width: int = 1,
                     color: Color = Color((0, 0, 0)),
-                    border_sides: list = BORDER_SIDES,
+                    border_sides: list = BorderSides,
                     ):
-        color = color.value if isinstance(color, Enum) else color
+        if depth(border_sides) == 2:
+            border_sides = set(sum(border_sides, ()))
+        elif depth(border_sides) == 1:
+            border_sides = set(border_sides)
+
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'updateBorders': {
                     'range': self.work_zone,
                     **dict((x, Border(border_style, border_width, color).__dict__) for x in border_sides),
                 }}, self.work_zone))
         return self
 
@@ -696,15 +697,14 @@
                 },
                 'fields': 'gridProperties.frozenRowCount, gridProperties.frozenColumnCount'
             }
         }, self.work_zone))
         return self
 
     def set_num_format(self, default_format: BaseNumberFormat = Number):
-        default_format = default_format.value if isinstance(default_format, Enum) else default_format
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'repeatCell': {
                     'range': self.work_zone,
                     **default_format.__dict__,
                 }}, self.work_zone))
         return self
 
@@ -747,38 +747,37 @@
                         bold: bool = None,
                         italic: bool = None,
                         strikethrough: bool = None,
                         underline: bool = None,
                         font_family: str = None,
                         text_color: Color = None):
 
-        text_color = text_color.value if isinstance(text_color, Enum) else text_color
         list_of_inputs = ', '.join(
             [f'textFormat.{s}' for s, x in
              zip(('fontFamily', 'fontSize', 'bold', 'italic', 'strikethrough', 'underline', 'foregroundColor'),
                  (font_family, font_size, bold, italic, strikethrough, underline, text_color)) if x is not None]
             + [s for s, x in zip(('horizontalAlignment', 'verticalAlignment', 'wrapStrategy'),
                                  (horizontal_alignment, vertical_alignment, wrap_strategy)) if x is not None])
 
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'repeatCell': {
                     'range': self.work_zone,
                     'cell': {
                         'userEnteredFormat': {
-                            'horizontalAlignment': horizontal_alignment.value if horizontal_alignment is not None or False else None,
-                            'verticalAlignment': vertical_alignment.value if vertical_alignment is not None or False else None,
-                            'wrapStrategy': wrap_strategy.value if wrap_strategy is not None or False else None,
+                            'horizontalAlignment': horizontal_alignment if horizontal_alignment not in (None, False) else None,
+                            'verticalAlignment': vertical_alignment if vertical_alignment not in (None, False) else None,
+                            'wrapStrategy': wrap_strategy if wrap_strategy not in (None, False) else None,
                             'textFormat': {
-                                'foregroundColor': text_color.color if text_color is not None or False else None,
-                                'fontFamily': font_family if font_family is not None or False else None,
-                                'fontSize': font_size if font_size is not None or False else None,
-                                'bold': bold if bold is not None or False else None,
-                                'italic': italic if italic is not None or False else None,
-                                'strikethrough': strikethrough if strikethrough is not None or False else None,
-                                'underline': underline if underline is not None or False else None,
+                                'foregroundColor': text_color.color if text_color not in (None, False) else None,
+                                'fontFamily': font_family if font_family not in (None, False) else None,
+                                'fontSize': font_size if font_size not in (None, False) else None,
+                                'bold': bold if bold not in (None, False) else None,
+                                'italic': italic if italic not in (None, False) else None,
+                                'strikethrough': strikethrough if strikethrough not in (None, False) else None,
+                                'underline': underline if underline not in (None, False) else None,
                             }}},
                     'fields': f'userEnteredFormat({list_of_inputs})',
                 }}, self.work_zone))
         return self
 
     def unmerge_cells(self):
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
@@ -959,27 +958,27 @@
                                        removeParents=previous_parents, fields='id, parents').execute()
 
     def share_spreadsheet_with_domain(self, ss: SpreedSheet, domain, role: ShareRole):
         self.connect_v3.permissions().create(**{
             'fileId': ss.spreadsheet_id,
             'body': {
                 'type': 'domain',
-                'role': role.value,
+                'role': role,
                 'domain': domain,
                 'allowFileDiscovery': True,
             },
             'fields': 'id',
         }).execute()
 
     def share_spreadsheet_with_user(self, ss: SpreedSheet, user: str, role: ShareRole):
         self.connect_v3.permissions().create(**{
             'fileId': ss.spreadsheet_id,
             'body': {
                 'type': 'user',
-                'role': role.value,
+                'role': role,
                 'emailAddress': user,
             },
             'fields': 'id',
         }).execute()
 
     def get_spreadsheet(self, spreadsheet_id):
         ss = SpreedSheet(spreadsheet_id=spreadsheet_id, token_path=self.token_path,
```

### Comparing `speedtab-0.1.3.0/speedtab/enums.py` & `speedtab-0.1.3.1/speedtab/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,79 +1,77 @@
-from enum import Enum
-
 from speedtab.formats import Color, Number, Dollar, Percent, Date, Time, DateTime, Scientific
 
 
-class BorderStyle(Enum):
+class BorderStyle:
     SOLID = 'SOLID'
     SOLID_MEDIUM = 'SOLID_MEDIUM'
     SOLID_THICK = 'SOLID_THICK'
     DOTTED = 'DOTTED'
     DASHED = 'DASHED'
     DOUBLE = 'DOUBLE'
 
 
-class MergeType(Enum):
+class MergeType:
     MERGE_ALL = 'MERGE_ALL'
     MERGE_COLUMNS = 'MERGE_COLUMNS'
     MERGE_ROWS = 'MERGE_ROWS'
 
 
-class HorizontalAlignment(Enum):
+class HorizontalAlignment:
     LEFT = 'LEFT'
     CENTER = 'CENTER'
     RIGHT = 'RIGHT'
 
 
-class VerticalAlignment(Enum):
+class VerticalAlignment:
     TOP = 'TOP'
     MIDDLE = 'MIDDLE'
     BOTTOM = 'BOTTOM'
 
 
-class WrapStrategy(Enum):
+class WrapStrategy:
     OVERFLOW_CELL = 'OVERFLOW_CELL'
     LEGACY_WRAP = 'LEGACY_WRAP'
     CLIP = 'CLIP'
     WRAP = 'WRAP'
 
 
-class ShareRole(Enum):
+class ShareRole:
     READER = 'reader'
     WRITER = 'writer'
 
 
-class ChartType(Enum):
+class ChartType:
     BAR = 'BAR'
     LINE = 'LINE'
     AREA = 'AREA'
     COLUMN = 'COLUMN'
     SCATTER = 'SCATTER'
 
 
-class StackedType(Enum):
+class StackedType:
     STACKED = 'STACKED'
     PERCENT_STACKED = 'PERCENT_STACKED'
     NONE = None
 
 
-class LegendPosition(Enum):
+class LegendPosition:
     BOTTOM_LEGEND = 'BOTTOM_LEGEND'
     LEFT_LEGEND = 'LEFT_LEGEND'
     RIGHT_LEGEND = 'RIGHT_LEGEND'
     TOP_LEGEND = 'TOP_LEGEND'
     NO_LEGEND = 'NO_LEGEND'
 
 
-class AxisPosition(Enum):
+class AxisPosition:
     LEFT_AXIS = 'LEFT_AXIS'
     RIGHT_AXIS = 'RIGHT_AXIS'
 
 
-class BooleanConditionTypes(Enum):
+class BooleanConditionTypes:
     NUMBER_GREATER = 'NUMBER_GREATER'
     NUMBER_GREATER_THAN_EQ = 'NUMBER_GREATER_THAN_EQ'
     NUMBER_LESS = 'NUMBER_LESS'
     NUMBER_LESS_THAN_EQ = 'NUMBER_LESS_THAN_EQ'
     NUMBER_EQ = 'NUMBER_EQ'
     NUMBER_NOT_EQ = 'NUMBER_NOT_EQ'
     NUMBER_BETWEEN = 'NUMBER_BETWEEN'
@@ -99,15 +97,15 @@
     NOT_BLANK = 'NOT_BLANK'
     CUSTOM_FORMULA = 'CUSTOM_FORMULA'
     BOOLEAN = 'BOOLEAN'
     TEXT_NOT_EQ = 'TEXT_NOT_EQ'
     DATE_NOT_EQ = 'DATE_NOT_EQ'
 
 
-class DefaultColors(Enum):
+class DefaultColors:
     BLACK = Color('#000000')
     DARK_GREY4 = Color('#434343')
     DARK_GREY3 = Color('#666666')
     DARK_GREY2 = Color('#999999')
     DARK_GREY1 = Color('#b7b7b7')
     GREY = Color('#cccccc')
     LIGHT_GREY1 = Color('#d9d9d9')
@@ -182,18 +180,30 @@
     LIGHT_MAGENTA2 = Color('#d5a6bd')
     LIGHT_MAGENTA1 = Color('#c27ba0')
     DARK_MAGENTA1 = Color('#a64d79')
     DARK_MAGENTA2 = Color('#741b47')
     DARK_MAGENTA3 = Color('#4c1130')
 
 
-class ReadyFormats(Enum):
+class ReadyFormats:
     NUMBER = Number()
     DECIMAL = Number('0.00')
     DOLLAR = Dollar()
     PRETTY_DOLLAR = Dollar('_($* #,##0.00_);_($* -#,##0.00;_($* "-"??_);_(@_)')
     PERCENT = Percent()
     DECIMAL_PERCENT = Percent('0.00%')
     DATE = Date()
     TIME = Time()
     DATETIME = DateTime()
-    SCIENTIFIC = Scientific()
+    SCIENTIFIC = Scientific()
+
+
+class BorderSides:
+    ALL_BORDERS = ('top', 'bottom', 'left', 'right', 'innerHorizontal', 'innerVertical')
+    INNER_BORDERS = ('innerHorizontal', 'innerVertical')
+    OUTER_BORDERS = ('top', 'bottom', 'left', 'right')
+    TOP_BORDER = ('top',)
+    BOTTOM_BORDER = ('bottom',)
+    LEFT_BORDER = ('left',)
+    RIGHT_BORDER = ('right',)
+    HORIZONTAL_BORDER = ('innerHorizontal',)
+    VERTICAL_BORDER = ('innerVertical',)
```

### Comparing `speedtab-0.1.3.0/speedtab/formats.py` & `speedtab-0.1.3.1/speedtab/formats.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class Color:
     def __init__(self, input: Union[str, tuple] = ()):
         if isinstance(input, str):
             input = tuple(int(input.lstrip('#')[i:i + 2], 16) for i in (0, 2, 4))
         self.color = dict([(key, color / 255) for key, color in zip(('red', 'green', 'blue'), input + (0,) * 3)])
 
 
-class BaseNumberFormat(ABC):#TODO: __all__
+class BaseNumberFormat(ABC):
     def __init__(self, type, pattern):
         self.fields = 'userEnteredFormat(numberFormat)'
         self.cell = {'userEnteredFormat': {'numberFormat': {'type': type, 'pattern': pattern}}}
 
 
 class Number(BaseNumberFormat):
     def __init__(self, pattern: str = '0'):
```

### Comparing `speedtab-0.1.3.0/setup.py` & `speedtab-0.1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.3.0',
+    'version': '0.1.3.1',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.3.0/PKG-INFO` & `speedtab-0.1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.3.0
+Version: 0.1.3.1
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

