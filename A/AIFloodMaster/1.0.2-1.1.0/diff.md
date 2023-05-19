# Comparing `tmp/AIFloodMaster-1.0.2.tar.gz` & `tmp/AIFloodMaster-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIFloodMaster-1.0.2.tar", last modified: Wed May 10 01:44:02 2023, max compression
+gzip compressed data, was "AIFloodMaster-1.1.0.tar", last modified: Fri May 19 03:11:26 2023, max compression
```

## Comparing `AIFloodMaster-1.0.2.tar` & `AIFloodMaster-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 01:44:02.425474 AIFloodMaster-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-10 01:44:02.263792 AIFloodMaster-1.0.2/AIFloodMaster.egg-info/
--rw-rw-rw-   0        0        0      250 2023-05-10 01:44:01.000000 AIFloodMaster-1.0.2/AIFloodMaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2023-05-10 01:44:02.000000 AIFloodMaster-1.0.2/AIFloodMaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 01:44:01.000000 AIFloodMaster-1.0.2/AIFloodMaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 01:44:02.000000 AIFloodMaster-1.0.2/AIFloodMaster.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 01:44:02.265770 AIFloodMaster-1.0.2/FloodMaster/
--rw-rw-rw-   0        0        0        0 2023-05-09 09:44:03.000000 AIFloodMaster-1.0.2/FloodMaster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:44:02.314944 AIFloodMaster-1.0.2/FloodMaster/controllers/
--rw-rw-rw-   0        0        0        0 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/controllers/__init__.py
--rw-rw-rw-   0        0        0     7443 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/controllers/agent.py
--rw-rw-rw-   0        0        0     1854 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/controllers/controller.py
--rw-rw-rw-   0        0        0     4346 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/controllers/env.py
--rw-rw-rw-   0        0        0     4044 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/controllers/processor.py
--rw-rw-rw-   0        0        0     1095 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/controllers/space.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:44:02.315867 AIFloodMaster-1.0.2/FloodMaster/delegators/
--rw-rw-rw-   0        0        0        0 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/delegators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:44:02.344669 AIFloodMaster-1.0.2/FloodMaster/forecasters/
--rw-rw-rw-   0        0        0    23185 2023-05-09 09:49:04.000000 AIFloodMaster-1.0.2/FloodMaster/forecasters/LstmPredictor.py
--rw-rw-rw-   0        0        0      262 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/forecasters/__init__.py
--rw-rw-rw-   0        0        0     3271 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/forecasters/predictor.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:44:02.420441 AIFloodMaster-1.0.2/FloodMaster/utils/
--rw-rw-rw-   0        0        0    17852 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/utils/CategoryEncoder.py
--rw-rw-rw-   0        0        0      164 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/utils/DataAnalyzer.py
--rw-rw-rw-   0        0        0     8739 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/utils/DataLoader.py
--rw-rw-rw-   0        0        0    10997 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/utils/DataPreprocessor.py
--rw-rw-rw-   0        0        0     5210 2023-03-09 03:43:11.000000 AIFloodMaster-1.0.2/FloodMaster/utils/DataScaler.py
--rw-rw-rw-   0        0        0      393 2023-05-09 09:23:43.000000 AIFloodMaster-1.0.2/FloodMaster/utils/__init__.py
--rw-rw-rw-   0        0        0      250 2023-05-10 01:44:02.424477 AIFloodMaster-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1985 2023-05-09 02:32:15.000000 AIFloodMaster-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 01:44:02.426587 AIFloodMaster-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      818 2023-05-09 08:50:04.000000 AIFloodMaster-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 03:11:26.288577 AIFloodMaster-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-05-19 03:11:26.089465 AIFloodMaster-1.1.0/AIFloodMaster.egg-info/
+-rw-rw-rw-   0        0        0     1204 2023-05-19 03:11:25.000000 AIFloodMaster-1.1.0/AIFloodMaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2023-05-19 03:11:25.000000 AIFloodMaster-1.1.0/AIFloodMaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 03:11:25.000000 AIFloodMaster-1.1.0/AIFloodMaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-19 03:11:25.000000 AIFloodMaster-1.1.0/AIFloodMaster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 03:11:26.093495 AIFloodMaster-1.1.0/FloodMaster/
+-rw-rw-rw-   0        0        0        0 2023-05-09 09:44:03.000000 AIFloodMaster-1.1.0/FloodMaster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 03:11:26.161581 AIFloodMaster-1.1.0/FloodMaster/controllers/
+drwxrwxrwx   0        0        0        0 2023-05-19 03:11:26.198287 AIFloodMaster-1.1.0/FloodMaster/controllers/PySwmmDdpgRTC/
+-rw-rw-rw-   0        0        0    11787 2023-05-16 09:21:53.000000 AIFloodMaster-1.1.0/FloodMaster/controllers/PySwmmDdpgRTC/DdpgAgent.py
+-rw-rw-rw-   0        0        0     9709 2023-05-17 01:38:45.000000 AIFloodMaster-1.1.0/FloodMaster/controllers/PySwmmDdpgRTC/DdpgController.py
+-rw-rw-rw-   0        0        0    10408 2023-05-16 09:49:41.000000 AIFloodMaster-1.1.0/FloodMaster/controllers/PySwmmDdpgRTC/DdpgEnv.py
+-rw-rw-rw-   0        0        0      257 2023-05-18 07:18:10.000000 AIFloodMaster-1.1.0/FloodMaster/controllers/__init__.py
+-rw-rw-rw-   0        0        0     7443 2023-03-09 03:43:11.000000 AIFloodMaster-1.1.0/FloodMaster/controllers/agent.py
+-rw-rw-rw-   0        0        0     2562 2023-05-16 10:08:10.000000 AIFloodMaster-1.1.0/FloodMaster/controllers/controller.py
+-rw-rw-rw-   0        0        0     4270 2023-05-16 09:35:56.000000 AIFloodMaster-1.1.0/FloodMaster/controllers/env.py
+-rw-rw-rw-   0        0        0     4044 2023-03-09 03:43:11.000000 AIFloodMaster-1.1.0/FloodMaster/controllers/processor.py
+-rw-rw-rw-   0        0        0     1095 2023-03-09 03:43:11.000000 AIFloodMaster-1.1.0/FloodMaster/controllers/space.py
+drwxrwxrwx   0        0        0        0 2023-05-19 03:11:26.202053 AIFloodMaster-1.1.0/FloodMaster/delegators/
+-rw-rw-rw-   0        0        0        0 2023-03-09 03:43:11.000000 AIFloodMaster-1.1.0/FloodMaster/delegators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 03:11:26.228306 AIFloodMaster-1.1.0/FloodMaster/forecasters/
+-rw-rw-rw-   0        0        0    23214 2023-05-16 07:14:41.000000 AIFloodMaster-1.1.0/FloodMaster/forecasters/LstmPredictor.py
+-rw-rw-rw-   0        0        0      262 2023-05-18 07:02:45.000000 AIFloodMaster-1.1.0/FloodMaster/forecasters/__init__.py
+-rw-rw-rw-   0        0        0     3417 2023-05-16 07:14:24.000000 AIFloodMaster-1.1.0/FloodMaster/forecasters/predictor.py
+drwxrwxrwx   0        0        0        0 2023-05-19 03:11:26.287088 AIFloodMaster-1.1.0/FloodMaster/utils/
+-rw-rw-rw-   0        0        0    17852 2023-03-09 03:43:11.000000 AIFloodMaster-1.1.0/FloodMaster/utils/CategoryEncoder.py
+-rw-rw-rw-   0        0        0      164 2023-03-09 03:43:11.000000 AIFloodMaster-1.1.0/FloodMaster/utils/DataAnalyzer.py
+-rw-rw-rw-   0        0        0     6365 2023-05-16 05:45:04.000000 AIFloodMaster-1.1.0/FloodMaster/utils/DataFilters.py
+-rw-rw-rw-   0        0        0     8739 2023-03-09 03:43:11.000000 AIFloodMaster-1.1.0/FloodMaster/utils/DataLoader.py
+-rw-rw-rw-   0        0        0    10997 2023-03-09 03:43:11.000000 AIFloodMaster-1.1.0/FloodMaster/utils/DataPreprocessor.py
+-rw-rw-rw-   0        0        0     5210 2023-03-09 03:43:11.000000 AIFloodMaster-1.1.0/FloodMaster/utils/DataScaler.py
+-rw-rw-rw-   0        0        0      458 2023-05-15 08:30:23.000000 AIFloodMaster-1.1.0/FloodMaster/utils/__init__.py
+-rw-rw-rw-   0        0        0     1204 2023-05-19 03:11:26.288080 AIFloodMaster-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2065 2023-05-15 01:00:48.000000 AIFloodMaster-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 03:11:26.289074 AIFloodMaster-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1169 2023-05-19 01:22:21.000000 AIFloodMaster-1.1.0/setup.py
```

### Comparing `AIFloodMaster-1.0.2/AIFloodMaster.egg-info/SOURCES.txt` & `AIFloodMaster-1.1.0/AIFloodMaster.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,21 @@
 FloodMaster/__init__.py
 FloodMaster/controllers/__init__.py
 FloodMaster/controllers/agent.py
 FloodMaster/controllers/controller.py
 FloodMaster/controllers/env.py
 FloodMaster/controllers/processor.py
 FloodMaster/controllers/space.py
+FloodMaster/controllers/PySwmmDdpgRTC/DdpgAgent.py
+FloodMaster/controllers/PySwmmDdpgRTC/DdpgController.py
+FloodMaster/controllers/PySwmmDdpgRTC/DdpgEnv.py
 FloodMaster/delegators/__init__.py
 FloodMaster/forecasters/LstmPredictor.py
 FloodMaster/forecasters/__init__.py
 FloodMaster/forecasters/predictor.py
 FloodMaster/utils/CategoryEncoder.py
 FloodMaster/utils/DataAnalyzer.py
+FloodMaster/utils/DataFilters.py
 FloodMaster/utils/DataLoader.py
 FloodMaster/utils/DataPreprocessor.py
 FloodMaster/utils/DataScaler.py
 FloodMaster/utils/__init__.py
```

### Comparing `AIFloodMaster-1.0.2/FloodMaster/controllers/agent.py` & `AIFloodMaster-1.1.0/FloodMaster/controllers/agent.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.2/FloodMaster/controllers/controller.py` & `AIFloodMaster-1.1.0/FloodMaster/controllers/controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,76 +10,97 @@
 
 class ABCController(metaclass=ABCMeta):
     """
     实时控制模型的统一接口类。
     """
 
     @abstractmethod
-    def compile(self, env: object, agent: object, processor: object, confs: dict):
+    def init(self, env: object, agent: object, processor: object, confs: dict):
         """
         初始化模型，配置模型结构。
 
         Args
         ----
-        + agent(`Agent`): 强化学习引擎;
         + env(`Env`): 强化学习环境;
-        + confs(dict): 模型配置。
+        + agent(`Agent`): 强化学习引擎;
+        + confs(dict): 强化学习调度模型配置。
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def train(self, confs: dict):
+    def fit(self, confs: dict) -> dict:
         """
         批训练模型。
 
         Args
         ----
-        + confs(dict): 模型训练配置信息，包括训练次数、批次大小，日志等级等。
+        + confs(dict): 模型训练配置信息，包括训练次数、批次大小等。
+
+        Returns
+        ----
+        返回模型训练过程信息, 例如准确度和收敛信息等。
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def step(self, observation: object) -> object:
+    def step(self, observation: object) -> tuple:
         """
         步进模型。
 
         Args
         ----
         + observation(object): 当前环境观察状态；
 
         Returns
         ----
-        actions(object)下一步动作。
+        返回模型当前状态(当前观测状态, 下一步执行的动作, 当前评估结果, 当前奖励).
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def run(self) -> object:
+    def run(self) -> dict:
         """
         在环境中运行模型直到环境结束。
 
         Returns
         ----
-        actions(object)所有采用的动作。
+        返回模型全程状态，内容包括：
+        {
+            "obervations": [], # 全程观测状态
+            "actions": [],     # 所有执行的动作
+            "metrics": [],     # 所有评估结果
+            "rewards": []      # 所有奖励
+        }
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def evaluate(self) -> dict:
+    def reset(self, confs: dict):
         """
-        评估(测试)模型。
+        重置模型, 如果没有重配置则恢复到初始状态。
 
         Args
         ----
+        + confs(dict): 强化学习调度模型配置。
+        """
+        raise NotImplementedError()
 
-        Returns
-        ----
-        返回各标签的各项评估结果。
+    @property
+    def configs(self):
+        """
+        模型的配置信息。
         """
         raise NotImplementedError()
 
-    @abstractmethod
-    def reset(self):
+    @property
+    def actions(self):
+        """
+        模型采用的动作组。
+        """
+        raise NotImplementedError()
+
+    @property
+    def observations(self):
         """
-        重置模型。
+        模型观察的状态组。
         """
         raise NotImplementedError()
```

### Comparing `AIFloodMaster-1.0.2/FloodMaster/controllers/env.py` & `AIFloodMaster-1.1.0/FloodMaster/controllers/env.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,23 +39,14 @@
         + observation(object), 智能体观察的当前环境状态；
         + reward(float), 执行动作后获得的奖励值；
         + done(bool), 当前回合是否结束；
         + info(dict), 辅助诊断信息;
         """
         raise NotImplementedError()
 
-    def setup(self, observation: object):
-        """设置当前环境状态。
-
-        Args
-        ----
-        + observation(object): 外部指定的环境状态;        
-        """
-        raise NotImplementedError()
-
     @abstractmethod
     def reset(self) -> object:
         """重置环境状态并返回初始观察。
 
         Returns
         ----
         Observation(object): 环境状态空间的初始观察(初始奖励设为 0)。
@@ -91,15 +82,15 @@
         Returns
         ----
         环境中随机数生成器使用的种子的列表。
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def configure(self):
+    def setup(self, *args, **kwargs):
         """提供环境运行时配置。
 
         配置中应该包含环境如何运行的相关信息/数据（比如远程服务器地址，数据路径等），
         但是同时不能影响环境语义。
         """
         raise NotImplementedError()
 
@@ -133,12 +124,19 @@
     @property
     def layers(self) -> list:
         """环境模型所有隐藏层列表。
         如果模型使用多个内部模型实现，则以连接列表的形式返回。
         """
         raise NotImplementedError()
 
+    @property
+    def configs(self) -> dict:
+        """
+        获取环境配置。
+        """
+        raise NotImplementedError()
+
     def __del__(self):
         self.close()
 
     def __str__(self):
         return '<{} instance>'.format(type(self).__name__)
```

### Comparing `AIFloodMaster-1.0.2/FloodMaster/controllers/processor.py` & `AIFloodMaster-1.1.0/FloodMaster/controllers/processor.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.2/FloodMaster/controllers/space.py` & `AIFloodMaster-1.1.0/FloodMaster/controllers/space.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.2/FloodMaster/forecasters/LstmPredictor.py` & `AIFloodMaster-1.1.0/FloodMaster/forecasters/LstmPredictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,14 +220,15 @@
             y_samples,
             # shuffle=False,
             epochs=self._confs['epochs'],
             batch_size=self._confs['batch_size'],
             validation_split=self._confs['validation_split'],
             callbacks=[earlystop],
             verbose=self._confs['verbose'])
+        return self._history
 
     def get_fit_history(self) -> dict:
         """获取模型训练过程中的准确率和损失过程。
 
         该方法返回模型最近一次训练过程中训练集和验证集上的准确率和损失过程。
         如果模型未经过训练，则模型返回 `None`。
```

### Comparing `AIFloodMaster-1.0.2/FloodMaster/forecasters/predictor.py` & `AIFloodMaster-1.1.0/FloodMaster/forecasters/predictor.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,35 +20,40 @@
     2. 方式二，
     加载(load) -> 预报(predict).
 
     3. 方式三，
     加载(load) -> 训练(fit) -> 评估(evaluate) -> 保存(save).
 
     """
+
     @abstractmethod
     def compile(self, confs: dict):
         """
         初始化模型，配置模型结构。
 
         Args
         ----
         + confs(dict): 模型配置基本信息, 包括特征IDs、标签IDs、采样步长、预报步长等。
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def fit(self, train_x: np.array, train_y: np.array, confs: dict):
+    def fit(self, train_x: np.array, train_y: np.array, confs: dict) -> dict:
         """
         加载训练数据集，训练模型。
 
         Args
         ----
         + train_x(np.array): 原始二维数据集的特征向量(sample_size*feature_size);
         + train_y(np.array): 原始二维数据集的标签向量(sample_size*label_size);
         + confs(dict): 模型训练配置信息，包括训练次数、批次大小，日志等级等。
+
+        Returns
+        ----
+        返回模型训练过程信息, 例如训练集和验证集上各项指标的准确率和损失。
         """
         raise NotImplementedError()
 
     @abstractmethod
     def predict(self, pred_x: np.array) -> np.array:
         """
         预报数据标签向量。
```

### Comparing `AIFloodMaster-1.0.2/FloodMaster/utils/CategoryEncoder.py` & `AIFloodMaster-1.1.0/FloodMaster/utils/CategoryEncoder.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.2/FloodMaster/utils/DataLoader.py` & `AIFloodMaster-1.1.0/FloodMaster/utils/DataLoader.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.2/FloodMaster/utils/DataPreprocessor.py` & `AIFloodMaster-1.1.0/FloodMaster/utils/DataPreprocessor.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.2/FloodMaster/utils/DataScaler.py` & `AIFloodMaster-1.1.0/FloodMaster/utils/DataScaler.py`

 * *Files identical despite different names*

### Comparing `AIFloodMaster-1.0.2/README.md` & `AIFloodMaster-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 
 *贵仁 - 智能雨洪管理模型*
 
 随着人工智能技术的发展，“AI+“成为诸多传统业务场景智能化升级的新需求，当然也包括水利水务行业。目前，公司已经基本建立了涵盖水文、一二维水力、水质的较为完整的数字仿真模型体系（简称GRMS），并为公司的一系列项目提供了稳定、有力的技术支撑。
 
 但是随着业务领域的加深和拓展，不断新增的业务需求，如智能预报、智能调度、污染溯源等，都对我们的技术服务能力提出了更高更新的要求。
 
-面对行业的需求升级和技术革新，基于最新的工业级人工智能框架“tensorflow2.x“、结合贵仁多年深耕水利水务行业的技术积累，我们研发了新一代的、针对雨洪场景的智能预报调度模型——贵仁智能雨洪管理模型（简称GRAFM）。
+面对行业的需求升级和技术革新，基于最新的工业级人工智能框架“tensorflow2.x“、结合贵仁多年深耕水利水务行业的技术积累，我们研发了新一代的、针对雨洪场景的智能预报调度模型——贵仁智能雨洪管理模型（GR - AIFloodMaster）。
 
 ---------------------------------------------------------------------------------
 
 ## 项目结构
 
 ```
 AI-Flood-Master Project Structure:
 
 +-- /
 |   +-- bin/                : 项目可执行文件以及脚本等
 |   +-- confs/              : 项目配置，包括环境路径、日志配置等
-|   +-- cores/              : 核心代码，
+|   +-- FloodMaster/        : 核心代码，
 |   |   +-- controllers/    : 雨洪工程调度方案
 |   |   +-- delegators/     ：雨洪模型代理方案
 |   |   +-- forecasters/    ：雨洪智能预报方案
 |   |   +-- routes/         : 在线服务封装接口
+|   +-- dist/               : 项目打包发布，
 |   +-- data/               : 项目数据，
-|   +-- db/                 : 项目数据库，
+|   +-- db/                 : 项目数据库(暂未启用)，
 |   +-- docs/               : 项目文档，
 |   +-- tests/              : 测试代码，
 |   +-- setup.py            : 项目打包发布方案
-|   +-- app.py              ：项目部署方案
+|   +-- app.py              ：项目在线部署方案
 ```
 
 ---------------------------------------------------------------------------------
 
 ## 如何使用
```

