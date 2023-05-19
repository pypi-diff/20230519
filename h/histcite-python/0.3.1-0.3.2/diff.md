# Comparing `tmp/histcite-python-0.3.1.tar.gz` & `tmp/histcite-python-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.3.1.tar", last modified: Thu May 18 03:26:52 2023, max compression
+gzip compressed data, was "histcite-python-0.3.2.tar", last modified: Fri May 19 16:49:22 2023, max compression
```

## Comparing `histcite-python-0.3.1.tar` & `histcite-python-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:26:52.786145 histcite-python-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-18 03:26:41.000000 histcite-python-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-05-18 03:26:52.786145 histcite-python-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-18 03:26:41.000000 histcite-python-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:26:52.782145 histcite-python-0.3.1/histcite/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-18 03:26:41.000000 histcite-python-0.3.1/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-18 03:26:41.000000 histcite-python-0.3.1/histcite/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-18 03:26:41.000000 histcite-python-0.3.1/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-18 03:26:41.000000 histcite-python-0.3.1/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-18 03:26:41.000000 histcite-python-0.3.1/histcite/parse_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-05-18 03:26:41.000000 histcite-python-0.3.1/histcite/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-18 03:26:41.000000 histcite-python-0.3.1/histcite/recognize_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:26:52.786145 histcite-python-0.3.1/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-05-18 03:26:52.000000 histcite-python-0.3.1/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-18 03:26:52.000000 histcite-python-0.3.1/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 03:26:52.000000 histcite-python-0.3.1/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-18 03:26:52.000000 histcite-python-0.3.1/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 03:26:52.000000 histcite-python-0.3.1/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 03:26:52.000000 histcite-python-0.3.1/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 03:26:52.786145 histcite-python-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-18 03:26:41.000000 histcite-python-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 03:26:52.786145 histcite-python-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-18 03:26:41.000000 histcite-python-0.3.1/tests/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-18 03:26:41.000000 histcite-python-0.3.1/tests/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-18 03:26:41.000000 histcite-python-0.3.1/tests/test_parse_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:49:22.769626 histcite-python-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-19 16:49:10.000000 histcite-python-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-19 16:49:22.769626 histcite-python-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-05-19 16:49:10.000000 histcite-python-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:49:22.769626 histcite-python-0.3.2/histcite/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/parse_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/recognize_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:49:22.769626 histcite-python-0.3.2/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:49:22.769626 histcite-python-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-19 16:49:10.000000 histcite-python-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:49:22.769626 histcite-python-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-19 16:49:10.000000 histcite-python-0.3.2/tests/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-19 16:49:10.000000 histcite-python-0.3.2/tests/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-19 16:49:10.000000 histcite-python-0.3.2/tests/test_parse_reference.py
```

### Comparing `histcite-python-0.3.1/LICENSE` & `histcite-python-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.1/PKG-INFO` & `histcite-python-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -27,38 +27,48 @@
 
 最近更新：
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
-- 生成包含文献、作者、机构、期刊、关键词等分析单元的统计数据；  
+- 生成统计数据，其中包括文献、作者、机构、文献来源、作者关键词等；  
+- 发现不在本地文献集中、但被本地文献集引用较多的文献；
 
 术语说明：
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
 - `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
-- `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
+- `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
 - `Recs`， 记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
+工具对比：
+| 对比项 | histcite-python | histcite pro |
+| :-: | :-: | :-: |
+| 是否开源 | 是 | 否 |
+| 是否跨平台 | 是 | 否，仅限 Windows |
+| 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
+| 是否提供前端界面 | 否 | 是 |
+| 引文网络图 | 矢量图，比较清晰 | 位图，比较粗糙 |
+
 ## 快速开始
 ```console
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
-| `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段； |
-| `CSSCI` | 从 `CSSCI数据库` 正常导出即可； |
-| `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。取消勾选 `Truncate to optimize for Excel`； |
+| `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
+| `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
+| `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
 >⚠️ 文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
@@ -66,15 +76,15 @@
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
 $ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
 $ histcite -f /Users/.../downloads/dataset -t wos -n 100
 ```
-结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
+>注：结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
 对应的文献节点信息：
 
@@ -117,29 +127,23 @@
 with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
     f.write(graph_dot_file)
 
 # 保存引文网络图节点文件
 graph_node_file = graph.generate_graph_node_file()
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
->⚠️ `generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。  
-⚠️ 没有边的节点不会出现在引文网络图中，文献节点数量可能会低于 `doc_indices` 的数量。
+>注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
 
-## 工具对比：
-| 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
-| :-: | :-: | :-: |
-| 是否跨平台 | 是 | 否，仅限 Windows |
-| 是否开源 | 是 | 否 |
-| 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
-| 是否提供前端界面 | 否 | 是 |
-| 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
-
-## Q&A
+## 实现细节
 |  | Web of Science | CSSCI | Scopus|
 | --- | --- | --- | --- |
 | 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作 `和 `题名` 进行判断 | 通过 `一作 `和 `题名` 进行判断 |
 | 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
 
+## Q&A
+1、为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
+答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。
+
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
 - [x] 支持 `Scopus` 题录数据
 - [ ] 支持 `PubMed` 题录数据
```

### Comparing `histcite-python-0.3.1/README.md` & `histcite-python-0.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,38 +4,48 @@
 
 最近更新：
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
-- 生成包含文献、作者、机构、期刊、关键词等分析单元的统计数据；  
+- 生成统计数据，其中包括文献、作者、机构、文献来源、作者关键词等；  
+- 发现不在本地文献集中、但被本地文献集引用较多的文献；
 
 术语说明：
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
 - `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
-- `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
+- `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
 - `Recs`， 记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
+工具对比：
+| 对比项 | histcite-python | histcite pro |
+| :-: | :-: | :-: |
+| 是否开源 | 是 | 否 |
+| 是否跨平台 | 是 | 否，仅限 Windows |
+| 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
+| 是否提供前端界面 | 否 | 是 |
+| 引文网络图 | 矢量图，比较清晰 | 位图，比较粗糙 |
+
 ## 快速开始
 ```console
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
-| `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段； |
-| `CSSCI` | 从 `CSSCI数据库` 正常导出即可； |
-| `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。取消勾选 `Truncate to optimize for Excel`； |
+| `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
+| `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
+| `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
 >⚠️ 文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
@@ -43,15 +53,15 @@
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
 $ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
 $ histcite -f /Users/.../downloads/dataset -t wos -n 100
 ```
-结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
+>注：结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
 对应的文献节点信息：
 
@@ -94,29 +104,23 @@
 with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
     f.write(graph_dot_file)
 
 # 保存引文网络图节点文件
 graph_node_file = graph.generate_graph_node_file()
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
->⚠️ `generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。  
-⚠️ 没有边的节点不会出现在引文网络图中，文献节点数量可能会低于 `doc_indices` 的数量。
+>注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
 
-## 工具对比：
-| 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
-| :-: | :-: | :-: |
-| 是否跨平台 | 是 | 否，仅限 Windows |
-| 是否开源 | 是 | 否 |
-| 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
-| 是否提供前端界面 | 否 | 是 |
-| 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
-
-## Q&A
+## 实现细节
 |  | Web of Science | CSSCI | Scopus|
 | --- | --- | --- | --- |
 | 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作 `和 `题名` 进行判断 | 通过 `一作 `和 `题名` 进行判断 |
 | 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
 
+## Q&A
+1、为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
+答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。
+
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
 - [x] 支持 `Scopus` 题录数据
-- [ ] 支持 `PubMed` 题录数据
+- [ ] 支持 `PubMed` 题录数据
```

### Comparing `histcite-python-0.3.1/histcite/cli.py` & `histcite-python-0.3.2/histcite/cli.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.1/histcite/compute_metrics.py` & `histcite-python-0.3.2/histcite/compute_metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,54 +26,59 @@
             df = df.reset_index(drop=True)
         
         if 'LCS' in use_cols and 'TC' in use_cols:
             grouped_df = df.groupby(col).agg({col: 'count', 'LCS': 'sum', 'TC': 'sum'})
             grouped_df = grouped_df.rename(columns={col: 'Recs', 'LCS': 'TLCS', 'TC': 'TGCS'})
         elif 'LCS' in use_cols and 'TC' not in use_cols:
             grouped_df = df.groupby(col).agg({col: 'count', 'LCS': 'sum'})
-            grouped_df = grouped_df.rename(columns={col: 'Recs', 'LCS': 'TLCS'})
+            grouped_df.rename(columns={col: 'Recs', 'LCS': 'TLCS'}, inplace=True)
         elif 'LCS' not in use_cols and 'TC' not in use_cols:
             grouped_df = df.groupby(col).agg({col: 'count'}).rename(columns={col: 'Recs'})
         else:
             raise ValueError('Invalid columns list')
+
+        if col == 'Author full names':
+            grouped_df.index = grouped_df.index.str.replace(r'\(\d+\)','',regex=True)
         return grouped_df.sort_values('Recs', ascending=False)
-    
+
     def _generate_author_table(self):
-        if self.source_type in ['wos','scopus']:
+        if self.source_type == 'wos':
             use_cols = ['AU','LCS','TC']
         elif self.source_type == 'cssci':
             use_cols = ['AU','LCS']
+        elif self.source_type == 'scopus':
+            use_cols = ['Author full names','LCS','TC']
         else:
             raise ValueError('Invalid source type')
-        return self.__generate_table(use_cols,'AU','; ')
+        return self.__generate_table(use_cols,use_cols[0],'; ')
     
     def _generate_keywords_table(self):
         if self.source_type in ['wos','scopus']:
             use_cols = ['DE','LCS','TC']
         elif self.source_type == 'cssci':
             use_cols = ['DE','LCS']
         else:
             raise ValueError('Invalid source type')
         return self.__generate_table(use_cols,'DE','; ',True)
     
     def _generate_institution_table(self):
-        if self.source_type == 'wos':
+        if self.source_type in ['wos','scopus']:
             use_cols = ['C3','LCS','TC']
         elif self.source_type == 'cssci':
             use_cols = ['C3','LCS']
         else:
             raise ValueError('Invalid source type')
         return self.__generate_table(use_cols,'C3','; ')
     
     def _generate_records_table(self):
         """生成文献简表"""
         if self.source_type in ['wos','scopus']:
-            use_cols = ['AU','TI','SO','PY','LCS','TC','LCR','NR','file source']
+            use_cols = ['AU','TI','SO','PY','LCS','TC','LCR','NR','source file']
         elif self.source_type == 'cssci':
-            use_cols = ['AU','TI','SO','PY','LCS','LCR','NR','file source']
+            use_cols = ['AU','TI','SO','PY','LCS','LCR','NR','source file']
         else:
             raise ValueError('Invalid source type')
         records_table = self.docs_table[use_cols]
         if self.source_type in ['wos','scopus']:
             records_table = records_table.rename(columns={'TC':'GCS','NR':'GCR'})
         return records_table
```

### Comparing `histcite-python-0.3.1/histcite/network_graph.py` & `histcite-python-0.3.2/histcite/network_graph.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.1/histcite/process_file.py` & `histcite-python-0.3.2/histcite/process_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         df['BP'] = df['BP'].apply(pd.to_numeric,errors='coerce')
         df['VL'] = df['VL'].apply(pd.to_numeric,errors='coerce')
         df = df.astype({'BP':'int64[pyarrow]', 'VL':'int64[pyarrow]'})
         
         # 提取一作
         first_au = df['AU'].apply(ProcessWosFile.extract_first_author)
         df.insert(1,'first_AU',first_au)
-        df['file source'] = file_name
+        df['source file'] = file_name
         return df
     
     def _read_cssci_file(self,file_name:str)->pd.DataFrame:
         """读取cssci文本文件"""
         file_path = os.path.join(self.folder_path,file_name)
         with open(file_path,'r') as f:
             text = f.read()
@@ -101,26 +101,26 @@
         df.columns = ['TI','AU','FU','SO','first_org','C3','first_AU','PY&VL&BP&EP','DE','CR']
         df['AU'] = df['AU'].str.replace('/','; ')
         df['DE'] = df['DE'].str.replace('/','; ')
         df['PY'] = df['PY&VL&BP&EP'].str.extract(r'^(\d{4}),',expand=False)
         df['C3'] = df['C3'].apply(ProcessCssciFile.process_org)
         df['CR'] = df['CR'].str.replace('\n','; ')
         df['NR'] = df['CR'].str.count('; ')
-        df['file source'] = file_name
+        df['source file'] = file_name
         return df
     
     def _read_scopus_file(self,file_name:str)->pd.DataFrame:
         """读取scopus表单"""
-        use_cols = ['Authors','Title','Year','Source title','Volume','Issue','Cited by','DOI','Affiliations','Author Keywords','References','Document Type','EID']
+        use_cols = ['Authors','Author full names','Title','Year','Source title','Volume','Issue','Cited by','DOI','Affiliations','Author Keywords','References','Document Type','EID']
         file_path = os.path.join(self.folder_path,file_name)
         df = ReadFile._read_csv(file_path,use_cols)
-        df.columns = ['AU','TI','PY','SO','VL','IS','TC','DI','C3','DE','CR','DT','EID']
+        df.columns = ['AU','Author full names','TI','PY','SO','VL','IS','TC','DI','C3','DE','CR','DT','EID']
         df['NR'] = df['CR'].str.count('; ')
         df['first_AU'] = ProcessScopusFile.extract_first_author(df['AU'])
-        df['file source'] = file_name
+        df['source file'] = file_name
         return df
     
     def concat_table(self):
         """合并多个dataframe"""
         if len(self.file_name_list)>1:
             if self.source_type=='wos':
                 docs_table = pd.concat([self._read_wos_file(file_name) for file_name in self.file_name_list],ignore_index=True,copy=False)
```

### Comparing `histcite-python-0.3.1/histcite/recognize_reference.py` & `histcite-python-0.3.2/histcite/recognize_reference.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.1/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.3.2/histcite_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -27,38 +27,48 @@
 
 最近更新：
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
-- 生成包含文献、作者、机构、期刊、关键词等分析单元的统计数据；  
+- 生成统计数据，其中包括文献、作者、机构、文献来源、作者关键词等；  
+- 发现不在本地文献集中、但被本地文献集引用较多的文献；
 
 术语说明：
 - `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
 - `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
-- `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
+- `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
 - `Recs`， 记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
+工具对比：
+| 对比项 | histcite-python | histcite pro |
+| :-: | :-: | :-: |
+| 是否开源 | 是 | 否 |
+| 是否跨平台 | 是 | 否，仅限 Windows |
+| 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
+| 是否提供前端界面 | 否 | 是 |
+| 引文网络图 | 矢量图，比较清晰 | 位图，比较粗糙 |
+
 ## 快速开始
 ```console
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
-| `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段； |
-| `CSSCI` | 从 `CSSCI数据库` 正常导出即可； |
-| `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。取消勾选 `Truncate to optimize for Excel`； |
+| `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
+| `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
+| `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
 >⚠️ 文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
@@ -66,15 +76,15 @@
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
 $ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
 $ histcite -f /Users/.../downloads/dataset -t wos -n 100
 ```
-结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
+>注：结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
 对应的文献节点信息：
 
@@ -117,29 +127,23 @@
 with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
     f.write(graph_dot_file)
 
 # 保存引文网络图节点文件
 graph_node_file = graph.generate_graph_node_file()
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
->⚠️ `generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。  
-⚠️ 没有边的节点不会出现在引文网络图中，文献节点数量可能会低于 `doc_indices` 的数量。
+>注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
 
-## 工具对比：
-| 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
-| :-: | :-: | :-: |
-| 是否跨平台 | 是 | 否，仅限 Windows |
-| 是否开源 | 是 | 否 |
-| 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
-| 是否提供前端界面 | 否 | 是 |
-| 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
-
-## Q&A
+## 实现细节
 |  | Web of Science | CSSCI | Scopus|
 | --- | --- | --- | --- |
 | 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作 `和 `题名` 进行判断 | 通过 `一作 `和 `题名` 进行判断 |
 | 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
 
+## Q&A
+1、为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
+答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。
+
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
 - [x] 支持 `Scopus` 题录数据
 - [ ] 支持 `PubMed` 题录数据
```

### Comparing `histcite-python-0.3.1/histcite_python.egg-info/SOURCES.txt` & `histcite-python-0.3.2/histcite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.1/setup.py` & `histcite-python-0.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="histcite-python",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.3.1",
+    version="0.3.2",
     description="A Python interface to histcite.",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["histcite","web of science","citation network"],
     license="MIT",
     url="https://github.com/doublessay/histcite-python",
     packages=["histcite"],
```

### Comparing `histcite-python-0.3.1/tests/test_compute_metrics.py` & `histcite-python-0.3.2/tests/test_compute_metrics.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.1/tests/test_network_graph.py` & `histcite-python-0.3.2/tests/test_network_graph.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.1/tests/test_parse_reference.py` & `histcite-python-0.3.2/tests/test_parse_reference.py`

 * *Files identical despite different names*

