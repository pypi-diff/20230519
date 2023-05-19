# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.894.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.895.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.894.tar", last modified: Thu May 18 00:41:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.895.tar", last modified: Fri May 19 03:05:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.894.tar` & `tencentcloud-sdk-python-vod-3.0.895.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   172410 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)    25111 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1175809 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud/vod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/tencentcloud_sdk_python_vod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-18 00:41:45.000000 tencentcloud-sdk-python-vod-3.0.894/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud/vod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   172410 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1183641 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud/vod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 03:05:11.000000 tencentcloud-sdk-python-vod-3.0.895/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vod-3.0.894/README.rst` & `tencentcloud-sdk-python-vod-3.0.895/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.894/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.895/tencentcloud/vod/v20180717/vod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.894/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.895/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.894/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.895/tencentcloud/vod/v20180717/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -617,36 +617,44 @@
         :param Input: 智能分类任务输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiAnalysisTaskClassificationInput`
         :param Output: 智能分类任务输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiAnalysisTaskClassificationOutput`
         :param Progress: 智能分类任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 智能分类任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 智能分类任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiAnalysisTaskClassificationInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiAnalysisTaskClassificationOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -732,36 +740,44 @@
         :param Input: 智能封面任务输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiAnalysisTaskCoverInput`
         :param Output: 智能封面任务输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiAnalysisTaskCoverOutput`
         :param Progress: 智能封面任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 智能封面任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 智能封面任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiAnalysisTaskCoverInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiAnalysisTaskCoverOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -847,36 +863,44 @@
         :param Input: 智能按帧标签任务输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiAnalysisTaskFrameTagInput`
         :param Output: 智能按帧标签任务输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiAnalysisTaskFrameTagOutput`
         :param Progress: 智能按帧标签任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 智能按帧标签任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 智能按帧标签任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiAnalysisTaskFrameTagInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiAnalysisTaskFrameTagOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -962,36 +986,44 @@
         :param Input: 智能精彩片段任务输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiAnalysisTaskHighlightInput`
         :param Output: 智能精彩片段任务输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiAnalysisTaskHighlightOutput`
         :param Progress: 智能精彩片段任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 智能精彩片段任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 智能精彩片段任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiAnalysisTaskHighlightInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiAnalysisTaskHighlightOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1101,36 +1133,44 @@
         :param Input: 智能标签任务输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiAnalysisTaskTagInput`
         :param Output: 智能标签任务输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiAnalysisTaskTagOutput`
         :param Progress: 智能标签任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 智能标签任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 智能标签任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiAnalysisTaskTagInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiAnalysisTaskTagOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1375,38 +1415,46 @@
         :param Message: 错误信息。
         :type Message: str
         :param Input: 语音全文识别任务输入信息。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskAsrFullTextResultInput`
         :param Output: 语音全文识别任务输出信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskAsrFullTextResultOutput`
-        :param Progress: 任务进度，取值范围 [0-100] 。
+        :param Progress: 语音全文识别任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 语音全文识别任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 语音全文识别任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiRecognitionTaskAsrFullTextResultInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiRecognitionTaskAsrFullTextResultOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1571,36 +1619,44 @@
         :param Input: 语音关键词识别任务输入信息。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskAsrWordsResultInput`
         :param Output: 语音关键词识别任务输出信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskAsrWordsResultOutput`
         :param Progress: 语音关键词识别任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 语音关键词识别任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 语音关键词识别任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiRecognitionTaskAsrWordsResultInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiRecognitionTaskAsrWordsResultOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1751,36 +1807,44 @@
         :param Input: 人脸识别任务输入信息。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskFaceResultInput`
         :param Output: 人脸识别任务输出信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskFaceResultOutput`
         :param Progress: 人脸识别任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 人脸识别任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 人脸识别任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiRecognitionTaskFaceResultInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiRecognitionTaskFaceResultOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1945,36 +2009,44 @@
         :param Input: 视频片头片尾识别任务输入信息。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskHeadTailResultInput`
         :param Output: 视频片头片尾识别任务输出信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskHeadTailResultOutput`
         :param Progress: 视频片头片尾识别任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 视频片头片尾识别任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 视频片头片尾识别任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiRecognitionTaskHeadTailResultInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiRecognitionTaskHeadTailResultOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2082,36 +2154,44 @@
         :param Input: 物体识别任务输入信息。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskObjectResultInput`
         :param Output: 物体识别任务输出信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskObjectResultOutput`
         :param Progress: 物体识别任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 物体识别任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 物体识别任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiRecognitionTaskObjectResultInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiRecognitionTaskObjectResultOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2266,36 +2346,44 @@
         :param Input: 文本全文识别任务输入信息。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskOcrFullTextResultInput`
         :param Output: 文本全文识别任务输出信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskOcrFullTextResultOutput`
         :param Progress: 文本全文识别任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 文本全文识别任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 文本全文识别任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiRecognitionTaskOcrFullTextResultInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiRecognitionTaskOcrFullTextResultOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2450,36 +2538,44 @@
         :param Input: 文本关键词识别任务输入信息。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskOcrWordsResultInput`
         :param Output: 文本关键词识别任务输出信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskOcrWordsResultOutput`
         :param Progress: 文本关键词识别任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 文本关键词识别任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 文本关键词识别任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiRecognitionTaskOcrWordsResultInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiRecognitionTaskOcrWordsResultOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2635,36 +2731,44 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskSegmentResultInput`
         :param Output: 视频拆条任务输出信息。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiRecognitionTaskSegmentResultOutput`
         :param Progress: 视频拆条任务进度，取值范围 [0-100] 。
         :type Progress: int
+        :param BeginProcessTime: 视频拆条任务开始执行的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type BeginProcessTime: str
+        :param FinishTime: 视频拆条任务执行完毕的时间，采用 [ISO 日期格式](https://cloud.tencent.com/document/product/266/11732#I)。
+        :type FinishTime: str
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
         self.Progress = None
+        self.BeginProcessTime = None
+        self.FinishTime = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiRecognitionTaskSegmentResultInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiRecognitionTaskSegmentResultOutput()
             self.Output._deserialize(params.get("Output"))
         self.Progress = params.get("Progress")
+        self.BeginProcessTime = params.get("BeginProcessTime")
+        self.FinishTime = params.get("FinishTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3448,34 +3552,38 @@
         :param Message: 错误信息。
         :type Message: str
         :param Input: 音视频审核 Ocr 文字涉及令人不适宜信息的任务输入。
         :type Input: :class:`tencentcloud.vod.v20180717.models.AiReviewPoliticalOcrTaskInput`
         :param Output: 音视频审核 Ocr 文字涉及令人不适宜信息的任务输出。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Output: :class:`tencentcloud.vod.v20180717.models.AiReviewPoliticalOcrTaskOutput`
+        :param Progress: 音视频审核 Ocr 文字涉及令人不适宜信息的任务进度，取值范围 [0-100] 。
+        :type Progress: int
         """
         self.Status = None
         self.ErrCodeExt = None
         self.ErrCode = None
         self.Message = None
         self.Input = None
         self.Output = None
+        self.Progress = None
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.ErrCodeExt = params.get("ErrCodeExt")
         self.ErrCode = params.get("ErrCode")
         self.Message = params.get("Message")
         if params.get("Input") is not None:
             self.Input = AiReviewPoliticalOcrTaskInput()
             self.Input._deserialize(params.get("Input"))
         if params.get("Output") is not None:
             self.Output = AiReviewPoliticalOcrTaskOutput()
             self.Output._deserialize(params.get("Output"))
+        self.Progress = params.get("Progress")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -13630,20 +13738,24 @@
 
     """
 
     def __init__(self):
         r"""
         :param Url: 需要提取水印的媒体 URL。
         :type Url: str
+        :param FileId: 媒体文件 ID。Url 对应的原始媒体文件 ID。
+        :type FileId: str
         """
         self.Url = None
+        self.FileId = None
 
 
     def _deserialize(self, params):
         self.Url = params.get("Url")
+        self.FileId = params.get("FileId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-vod-3.0.894/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.895/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.894'
+__version__ = '3.0.895'
```

### Comparing `tencentcloud-sdk-python-vod-3.0.894/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.895/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.894/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.895/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.894
+Version: 3.0.895
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.894/setup.py` & `tencentcloud-sdk-python-vod-3.0.895/setup.py`

 * *Files identical despite different names*

