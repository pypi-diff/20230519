# Comparing `tmp/dataverse-sdk-0.1.1.tar.gz` & `tmp/dataverse-sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse-sdk-0.1.1.tar", last modified: Wed Jan 18 08:09:21 2023, max compression
+gzip compressed data, was "dataverse-sdk-0.1.2.tar", last modified: Fri May 19 03:20:05 2023, max compression
```

## Comparing `dataverse-sdk-0.1.1.tar` & `dataverse-sdk-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 yhchen     (501) staff       (20)        0 2023-01-18 08:09:21.831041 dataverse-sdk-0.1.1/
--rw-r--r--   0 yhchen     (501) staff       (20)     4985 2023-01-18 08:09:21.829548 dataverse-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 yhchen     (501) staff       (20)     4745 2023-01-16 04:45:42.000000 dataverse-sdk-0.1.1/README.md
-drwxr-xr-x   0 yhchen     (501) staff       (20)        0 2023-01-18 08:09:21.807533 dataverse-sdk-0.1.1/dataverse_sdk/
--rw-r--r--   0 yhchen     (501) staff       (20)      825 2023-01-13 07:15:56.000000 dataverse-sdk-0.1.1/dataverse_sdk/__init__.py
-drwxr-xr-x   0 yhchen     (501) staff       (20)        0 2023-01-18 08:09:21.817970 dataverse-sdk-0.1.1/dataverse_sdk/apis/
--rw-r--r--   0 yhchen     (501) staff       (20)        0 2022-11-15 08:35:29.000000 dataverse-sdk-0.1.1/dataverse_sdk/apis/__init__.py
--rw-r--r--   0 yhchen     (501) staff       (20)     8120 2023-01-16 04:46:37.000000 dataverse-sdk-0.1.1/dataverse_sdk/apis/backend.py
--rw-r--r--   0 yhchen     (501) staff       (20)    13824 2023-01-13 10:44:35.000000 dataverse-sdk-0.1.1/dataverse_sdk/client.py
--rw-r--r--   0 yhchen     (501) staff       (20)     1550 2022-11-22 04:07:57.000000 dataverse-sdk-0.1.1/dataverse_sdk/connections.py
--rw-r--r--   0 yhchen     (501) staff       (20)      587 2022-11-22 04:07:57.000000 dataverse-sdk-0.1.1/dataverse_sdk/constants.py
-drwxr-xr-x   0 yhchen     (501) staff       (20)        0 2023-01-18 08:09:21.821184 dataverse-sdk-0.1.1/dataverse_sdk/exceptions/
--rw-r--r--   0 yhchen     (501) staff       (20)        0 2022-11-15 08:35:29.000000 dataverse-sdk-0.1.1/dataverse_sdk/exceptions/__init__.py
--rw-r--r--   0 yhchen     (501) staff       (20)       49 2022-11-22 04:07:57.000000 dataverse-sdk-0.1.1/dataverse_sdk/exceptions/client.py
-drwxr-xr-x   0 yhchen     (501) staff       (20)        0 2023-01-18 08:09:21.825895 dataverse-sdk-0.1.1/dataverse_sdk/schemas/
--rw-r--r--   0 yhchen     (501) staff       (20)        0 2022-11-18 03:15:32.000000 dataverse-sdk-0.1.1/dataverse_sdk/schemas/__init__.py
--rw-r--r--   0 yhchen     (501) staff       (20)     3011 2023-01-13 07:15:56.000000 dataverse-sdk-0.1.1/dataverse_sdk/schemas/api.py
--rw-r--r--   0 yhchen     (501) staff       (20)     7077 2023-01-13 10:49:04.000000 dataverse-sdk-0.1.1/dataverse_sdk/schemas/client.py
--rw-r--r--   0 yhchen     (501) staff       (20)     1164 2022-11-24 07:22:56.000000 dataverse-sdk-0.1.1/dataverse_sdk/schemas/common.py
-drwxr-xr-x   0 yhchen     (501) staff       (20)        0 2023-01-18 08:09:21.827769 dataverse-sdk-0.1.1/dataverse_sdk/utils/
--rw-r--r--   0 yhchen     (501) staff       (20)        0 2022-11-24 06:59:50.000000 dataverse-sdk-0.1.1/dataverse_sdk/utils/__init__.py
--rw-r--r--   0 yhchen     (501) staff       (20)      371 2022-11-22 04:07:57.000000 dataverse-sdk-0.1.1/dataverse_sdk/utils/utils.py
-drwxr-xr-x   0 yhchen     (501) staff       (20)        0 2023-01-18 08:09:21.814693 dataverse-sdk-0.1.1/dataverse_sdk.egg-info/
--rw-r--r--   0 yhchen     (501) staff       (20)     4985 2023-01-18 08:09:21.000000 dataverse-sdk-0.1.1/dataverse_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yhchen     (501) staff       (20)      629 2023-01-18 08:09:21.000000 dataverse-sdk-0.1.1/dataverse_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yhchen     (501) staff       (20)        1 2023-01-18 08:09:21.000000 dataverse-sdk-0.1.1/dataverse_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yhchen     (501) staff       (20)       18 2023-01-18 08:09:21.000000 dataverse-sdk-0.1.1/dataverse_sdk.egg-info/requires.txt
--rw-r--r--   0 yhchen     (501) staff       (20)       14 2023-01-18 08:09:21.000000 dataverse-sdk-0.1.1/dataverse_sdk.egg-info/top_level.txt
--rw-r--r--   0 yhchen     (501) staff       (20)       38 2023-01-18 08:09:21.831443 dataverse-sdk-0.1.1/setup.cfg
--rw-r--r--   0 yhchen     (501) staff       (20)      613 2023-01-16 01:58:34.000000 dataverse-sdk-0.1.1/setup.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.431266 dataverse-sdk-0.1.2/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5378 2023-05-19 03:20:05.431139 dataverse-sdk-0.1.2/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5138 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.2/README.md
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.428684 dataverse-sdk-0.1.2/dataverse_sdk/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/__init__.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.429538 dataverse-sdk-0.1.2/dataverse_sdk/apis/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/apis/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     9053 2023-05-19 03:16:44.000000 dataverse-sdk-0.1.2/dataverse_sdk/apis/backend.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    16063 2023-05-19 03:16:44.000000 dataverse-sdk-0.1.2/dataverse_sdk/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1550 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/connections.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      587 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/constants.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.429968 dataverse-sdk-0.1.2/dataverse_sdk/exceptions/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/exceptions/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       49 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/exceptions/client.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.430665 dataverse-sdk-0.1.2/dataverse_sdk/schemas/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/schemas/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     3036 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.2/dataverse_sdk/schemas/api.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     7709 2023-05-19 03:16:44.000000 dataverse-sdk-0.1.2/dataverse_sdk/schemas/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1164 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/schemas/common.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.430924 dataverse-sdk-0.1.2/dataverse_sdk/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      371 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.2/dataverse_sdk/utils/utils.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-19 03:20:05.429311 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5378 2023-05-19 03:20:05.000000 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2023-05-19 03:20:05.000000 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2023-05-19 03:20:05.000000 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       18 2023-05-19 03:20:05.000000 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/requires.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2023-05-19 03:20:05.000000 dataverse-sdk-0.1.2/dataverse_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2023-05-19 03:20:05.431304 dataverse-sdk-0.1.2/setup.cfg
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      613 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.2/setup.py
```

### Comparing `dataverse-sdk-0.1.1/PKG-INFO` & `dataverse-sdk-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 
@@ -46,20 +46,31 @@
 
 Once you've initialized a DataverseClient, you can interact with Dataverse from the initialized object.
 
 ## Examples
 
 The following sections provide examples for the most common DataVerse tasksm including:
 
+* [List Projects](#list-projects)
 * [Create Project](#create-project)
 * [Get Project](#get-project)
 * [Create Dataset](#create-dataset)
 * [Get Dataset](#get-dataset)
 
 
+### List Projects
+The `list_projects` method will list all projects of the given sites.
+
+
+```Python
+projects = client.list_projects(current_user = True,
+                                exclude_sensor_type=SensorType.LIDAR,
+                                image_type= OntologyImageType._2D_BOUNDING_BOX)
+
+```
 ### Create Project
 
 The `create_project` method will create project on the connected site with the defined ontology and sensors.
 
 ```Python
 ontology = Ontology(
     name="test ot",
@@ -111,14 +122,15 @@
     "data_source": DataSource.Azure/Datasource.AWS,
     "storage_url": "storage/url",
     "container_name": "azure container name",
     "data_folder": "datafolder/to/vai_anno",
     "sas_token": "azure sas token",
     "name": "Dataset 1",
     "type": DatasetType.ANNOTATED_DATA,
+    "annotations": ["groundtruth"]
     "generate_metadata": False,
     "render_pcd": False,
     "annotation_format": AnnotationFormat.VISION_AI,
     "sequential": False,
     "sensors": project.sensors,
 }
 dataset = project.create_dataset(**dataset_data)
@@ -132,19 +144,20 @@
     "storage_url" : "",
     "container_name": "",
     "sas_token":"",
     "data_folder": "/path/to/your_localdir",
     "name": "Dataset Local Upload",
     "type": DatasetType.ANNOTATED_DATA,
     "generate_metadata": False,
+    "auto_tagging": ["weather"],
     "render_pcd": False,
     "annotation_format": AnnotationFormat.VISION_AI,
     "sequential": False,
     "sensors": project.sensors,
-    "extra_annotations" :['model_name']  #optional
+    "annotations" :['model_name']
 }
 dataset = project.create_dataset(**dataset_data)
 ```
 
 ## Get Dataset
 
 The `get_dataset` method retrieves the dataset info from the connected site. The `id` parameter is the unique interger ID of the dataset, not its "name" property.
```

### Comparing `dataverse-sdk-0.1.1/README.md` & `dataverse-sdk-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -36,20 +36,31 @@
 
 Once you've initialized a DataverseClient, you can interact with Dataverse from the initialized object.
 
 ## Examples
 
 The following sections provide examples for the most common DataVerse tasksm including:
 
+* [List Projects](#list-projects)
 * [Create Project](#create-project)
 * [Get Project](#get-project)
 * [Create Dataset](#create-dataset)
 * [Get Dataset](#get-dataset)
 
 
+### List Projects
+The `list_projects` method will list all projects of the given sites.
+
+
+```Python
+projects = client.list_projects(current_user = True,
+                                exclude_sensor_type=SensorType.LIDAR,
+                                image_type= OntologyImageType._2D_BOUNDING_BOX)
+
+```
 ### Create Project
 
 The `create_project` method will create project on the connected site with the defined ontology and sensors.
 
 ```Python
 ontology = Ontology(
     name="test ot",
@@ -101,14 +112,15 @@
     "data_source": DataSource.Azure/Datasource.AWS,
     "storage_url": "storage/url",
     "container_name": "azure container name",
     "data_folder": "datafolder/to/vai_anno",
     "sas_token": "azure sas token",
     "name": "Dataset 1",
     "type": DatasetType.ANNOTATED_DATA,
+    "annotations": ["groundtruth"]
     "generate_metadata": False,
     "render_pcd": False,
     "annotation_format": AnnotationFormat.VISION_AI,
     "sequential": False,
     "sensors": project.sensors,
 }
 dataset = project.create_dataset(**dataset_data)
@@ -122,19 +134,20 @@
     "storage_url" : "",
     "container_name": "",
     "sas_token":"",
     "data_folder": "/path/to/your_localdir",
     "name": "Dataset Local Upload",
     "type": DatasetType.ANNOTATED_DATA,
     "generate_metadata": False,
+    "auto_tagging": ["weather"],
     "render_pcd": False,
     "annotation_format": AnnotationFormat.VISION_AI,
     "sequential": False,
     "sensors": project.sensors,
-    "extra_annotations" :['model_name']  #optional
+    "annotations" :['model_name']
 }
 dataset = project.create_dataset(**dataset_data)
 ```
 
 ## Get Dataset
 
 The `get_dataset` method retrieves the dataset info from the connected site. The `id` parameter is the unique interger ID of the dataset, not its "name" property.
```

### Comparing `dataverse-sdk-0.1.1/dataverse_sdk/__init__.py` & `dataverse-sdk-0.1.2/dataverse_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.1/dataverse_sdk/apis/backend.py` & `dataverse-sdk-0.1.2/dataverse_sdk/apis/backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import json
 import logging
 from typing import Optional, Union
+from urllib.parse import urlencode
 
 import requests
 from requests import sessions
 from requests.adapters import HTTPAdapter, Retry
 
 logger = logging.getLogger(__name__)
 
@@ -162,32 +163,57 @@
         resp = self.send_request(
             url=f"{self.host}/api/projects/{project_id}",
             method="get",
             headers=self.headers,
         )
         return resp.json()
 
+    def list_projects(
+        self,
+        current_user: Optional[bool] = True,
+        exclude_sensor_type: Optional[str] = None,
+        image_type: Optional[str] = None,
+        **kwargs,
+    ) -> list:
+        if current_user:
+            kwargs["current_user"] = current_user
+        if exclude_sensor_type is not None:
+            kwargs["exclude_sensor_type"] = exclude_sensor_type.value
+        if image_type is not None:
+            kwargs["ontology__image_type"] = image_type.value
+        resp = self.send_request(
+            url=f"{self.host}/api/projects/basic/?{urlencode(kwargs)}",
+            method="get",
+            headers=self.headers,
+        )
+        return resp.json()["results"]
+
     def create_dataset(
         self,
         name: str,
         data_source: str,
         project_id: int,
         sensor_ids: list[int],
         type: str,
         annotation_format: str,
         storage_url: str,
         data_folder: str,
         sequential: bool = False,
         generate_metadata: bool = False,
+        auto_tagging: Optional[list] = None,
         render_pcd: bool = False,
         container_name: Optional[str] = None,
         sas_token: Optional[str] = None,
         description: Optional[str] = None,
-        extra_annotations: Optional[list[str]] = None,
+        annotations: Optional[list[str]] = None,
     ) -> dict:
+        if auto_tagging is None:
+            auto_tagging = []
+        if annotations is None:
+            annotations = []
         resp = self.send_request(
             url=f"{self.host}/api/datasets/",
             method="post",
             headers=self.headers,
             data={
                 "name": name,
                 "project_id": project_id,
@@ -197,17 +223,18 @@
                 "container_name": container_name,
                 "data_folder": data_folder,
                 "sas_token": sas_token,
                 "type": type,
                 "sequential": sequential,
                 "annotation_format": annotation_format,
                 "generate_metadata": generate_metadata,
+                "auto_tagging": auto_tagging,
                 "render_pcd": render_pcd,
                 "description": description if description else "",
-                "extra_annotations": extra_annotations if extra_annotations else [],
+                "annotations": annotations if annotations else [],
             },
         )
         return resp.json()
 
     def get_dataset(self, dataset_id: int):
         resp = self.send_request(
             url=f"{self.host}/api/datasets/{dataset_id}/",
@@ -220,15 +247,14 @@
     def upload_files(
         self,
         dataset_id: int,
         container_name: str,
         is_finished: bool,
         file_dict: dict[str, bytes],
     ):
-
         file_dict["json"] = (
             None,
             json.dumps(
                 {
                     "dataset_id": dataset_id,
                     "container_name": container_name,
                     "is_finished": is_finished,
@@ -242,15 +268,14 @@
             method="post",
             headers={"Authorization": self.headers["Authorization"]},
             files=file_dict,
         )
         return resp
 
     def update_dataset(self, dataset_id: int, **kwargs):
-
         resp = self.send_request(
             url=f"{self.host}/api/datasets/{dataset_id}/",
             method="patch",
             headers=self.headers,
             data=kwargs,
         )
         return resp
```

### Comparing `dataverse-sdk-0.1.1/dataverse_sdk/client.py` & `dataverse-sdk-0.1.2/dataverse_sdk/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     AttributeAPISchema,
     DatasetAPISchema,
     OntologyAPISchema,
     ProjectAPISchema,
     ProjectTagAPISchema,
 )
 from .schemas.client import Dataset, DataSource, Ontology, Project, ProjectTag, Sensor
-from .schemas.common import AnnotationFormat, DatasetType
+from .schemas.common import AnnotationFormat, DatasetType, OntologyImageType, SensorType
 from .utils.utils import get_filepaths
 
 
 class DataverseClient:
     def __init__(
         self,
         host: DataverseHost,
@@ -57,15 +57,14 @@
     def _init_api_client(
         self,
         email: Optional[str] = None,
         password: Optional[str] = None,
         access_token: Optional[str] = None,
         refresh_token: Optional[str] = None,
     ) -> None:
-
         try:
             self._api_client = BackendAPI(
                 host=self.host,
                 email=email,
                 password=password,
                 access_token=access_token,
                 refresh_token=refresh_token,
@@ -171,14 +170,52 @@
 
         try:
             project_data: dict = client._api_client.create_project(**raw_project_data)
         except Exception as e:
             raise ClientConnectionError(f"Failed to create the project: {e}")
         return Project.create(project_data)
 
+    def list_projects(
+        self,
+        current_user: bool = True,
+        exclude_sensor_type: Optional[SensorType] = None,
+        image_type: Optional[OntologyImageType] = None,
+    ) -> list:
+        """list projects in dataverse (with given filter query params)
+
+        Parameters
+        ----------
+        current_user : bool, optional
+            only show the projects of current user, by default True
+        exclude_sensor_type : Optional[SensorType], optional
+            exclude the projects with the given sensor type, by default None
+        image_type : Optional[OntologyImageType], optional
+            only include the projects with the given image type, by default None
+
+        Returns
+        -------
+        list
+            list of projects [{'id': 5, 'name': 'Kitti Sequential Project'}, {'id': 6, 'name': 'project2'}]
+
+        Raises
+        ------
+        ClientConnectionError
+            raise error if there is any error occurs when calling backend APIs.
+        """
+
+        try:
+            project_list: list = self._api_client.list_projects(
+                current_user=current_user,
+                exclude_sensor_type=exclude_sensor_type,
+                image_type=image_type,
+            )
+        except Exception as e:
+            raise ClientConnectionError(f"Failed to get the projects: {e}")
+        return project_list
+
     def get_project(self, project_id: int):
         """Get project detail by project-id
 
         Parameters
         ----------
         project_id : int
             project-id in db
@@ -240,16 +277,18 @@
         sensors: list[Sensor],
         type: DatasetType,
         annotation_format: AnnotationFormat,
         storage_url: str,
         data_folder: str,
         container_name: Optional[str] = None,
         sas_token: Optional[str] = None,
+        annotations: Optional[list] = None,
         sequential: bool = False,
         generate_metadata: bool = False,
+        auto_tagging: Optional[list] = None,
         render_pcd: bool = False,
         description: Optional[str] = None,
         client: Optional["DataverseClient"] = None,
         **kwargs,
     ) -> Dataset:
         """Create Dataset
 
@@ -271,18 +310,22 @@
             storage url for cloud
         data_folder : str
             data folder of the storage
         container_name : Optional[str], optional
             container name for Azure, by default None
         sas_token : Optional[str], optional
             SAStoken for Azure, by default None
+        annotations: list, optional
+            list of annotation folder name (should be groundtruth or $model_name)
         sequential : bool, optional
             sequential or not., by default False
         generate_metadata : bool, optional
             generate meta data or not, by default False
+        auto_tagging: list
+            generate auto_tagging with target models (weather/scene/timeofday)
         description : Optional[str], optional
             description of the dataset, by default None
         render_pcd : bool, optional
             render pcd preview image or not, be default False
         client : Optional[DataverseClient]
             the client to be used to create the dataset, will use the default client if it's None
 
@@ -298,33 +341,44 @@
             raise exception if there is any error occurs when composing request body.
         ClientConnectionError
             raise exception if there is any error occurs when calling backend APIs.
         """
         if data_source not in DataSource:
             raise ValueError(f"Data source ({data_source}) is not supported currently.")
 
+        if annotations is None:
+            annotations = []
+        if auto_tagging is None:
+            auto_tagging = []
+
+        if type == DatasetType.ANNOTATED_DATA and len(annotations) == 0:
+            raise ValueError(
+                "Annoted data should provide at least one annotation folder name (groundtruth or model_name)"
+            )
         if client is None:
             client = DataverseClient.get_client()
 
         sensor_ids = [sensor.id for sensor in sensors]
         project_id = project.id
         try:
             raw_dataset_data: dict = DatasetAPISchema(
                 name=name,
                 project_id=project_id,
                 sensor_ids=sensor_ids,
                 data_source=data_source,
                 type=type,
                 annotation_format=annotation_format,
+                annotations=annotations,
                 storage_url=storage_url,
                 container_name=container_name,
                 data_folder=data_folder,
                 sas_token=sas_token,
                 sequential=sequential,
                 generate_metadata=generate_metadata,
+                auto_tagging=auto_tagging,
                 render_pcd=render_pcd,
                 description=description,
                 **kwargs,
             ).dict(exclude_none=True)
         except ValidationError as e:
             raise ValidationError(
                 f"Something wrong when composing the final dataset data: {e}"
@@ -339,14 +393,16 @@
 
         dataset_data.update(
             {
                 "project": project,
                 "sensors": sensors,
                 "sequential": sequential,
                 "generate_metadata": generate_metadata,
+                "auto_tagging": auto_tagging,
+                "annotations": annotations,
             }
         )
 
         if data_source in {DataSource.Azure, DataSource.AWS}:
             return Dataset(**dataset_data)
 
         # start uploading from local
```

### Comparing `dataverse-sdk-0.1.1/dataverse_sdk/connections.py` & `dataverse-sdk-0.1.2/dataverse_sdk/connections.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.1/dataverse_sdk/constants.py` & `dataverse-sdk-0.1.2/dataverse_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.1/dataverse_sdk/schemas/api.py` & `dataverse-sdk-0.1.2/dataverse_sdk/schemas/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
     annotation_format: AnnotationFormat
     storage_url: str
     data_folder: str
     container_name: Optional[str] = None
     sas_token: Optional[str] = None
     sequential: bool = False
     generate_metadata: bool = False
+    auto_tagging: list[str] = []
     render_pcd: bool = False
     description: Optional[str] = None
     calibration_folder: Optional[str] = None
     annotation_file: Optional[str] = None
     annotation_folder: Optional[str] = None
     lidar_folder: Optional[str] = None
     render_pcd: Optional[str] = None
-    extra_annotations: Optional[list[str]] = None
+    annotations: Optional[list[str]] = []
```

### Comparing `dataverse-sdk-0.1.1/dataverse_sdk/schemas/client.py` & `dataverse-sdk-0.1.2/dataverse_sdk/schemas/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,16 @@
 
     @classmethod
     def create(cls, project_data: dict) -> "Project":
         ontology = Ontology.create(project_data["ontology"])
         sensors = [
             Sensor.create(sensor_data) for sensor_data in project_data["sensors"]
         ]
+        if project_data["project_tag"] is None:
+            project_data["project_tag"] = {}
         project_tag = ProjectTag.create(project_data["project_tag"])
         return cls(
             id=project_data["id"],
             name=project_data["name"],
             description=project_data["description"],
             ego_car=project_data["ego_car"],
             ontology=ontology,
@@ -160,16 +162,18 @@
         sensors: list[Sensor],
         type: DatasetType,
         annotation_format: AnnotationFormat,
         storage_url: str,
         data_folder: str,
         container_name: Optional[str] = None,
         sas_token: Optional[str] = None,
+        annotations: Optional[list] = None,
         sequential: bool = False,
         generate_metadata: bool = False,
+        auto_tagging: Optional[list] = None,
         render_pcd: bool = False,
         description: Optional[str] = None,
         **kwargs,
     ):
         """Create Dataset From project itself
 
         Parameters
@@ -188,18 +192,22 @@
             storage url for cloud
         data_folder : str
             data folder of the storage
         container_name : Optional[str], optional
             container name for Azure, by default None
         sas_token : Optional[str], optional
             SAStoken for Azure, by default None
+        annotations: list, optional
+            list of annotation folder name (should be groundtruth or $model_name)
         sequential : bool, optional
             sequential or not., by default False
         generate_metadata : bool, optional
             generate meta data or not, by default False
+        auto_tagging: list, optional
+            generate auto_tagging with target models (weather/scene/timeofday), by default []
         render_pcd : bool, optional
             render pcd preview image or not, be default False
         description : Optional[str], optional
             description of the dataset, by default None
 
         Returns
         -------
@@ -209,27 +217,34 @@
         Raises
         ------
         ClientConnectionError
             raise error if client is not exist
         """
         from ..client import DataverseClient
 
+        if auto_tagging is None:
+            auto_tagging = []
+        if annotations is None:
+            annotations = []
+
         dataset_output = DataverseClient.create_dataset(
             name=name,
             data_source=data_source,
             project=self,
             sensors=sensors,
             type=type,
             annotation_format=annotation_format,
             storage_url=storage_url,
             container_name=container_name,
             data_folder=data_folder,
             sas_token=sas_token,
+            annotations=annotations,
             sequential=sequential,
             generate_metadata=generate_metadata,
+            auto_tagging=auto_tagging,
             render_pcd=render_pcd,
             description=description,
             **kwargs,
         )
         return dataset_output
```

### Comparing `dataverse-sdk-0.1.1/dataverse_sdk/schemas/common.py` & `dataverse-sdk-0.1.2/dataverse_sdk/schemas/common.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.1/dataverse_sdk.egg-info/PKG-INFO` & `dataverse-sdk-0.1.2/dataverse_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 
@@ -46,20 +46,31 @@
 
 Once you've initialized a DataverseClient, you can interact with Dataverse from the initialized object.
 
 ## Examples
 
 The following sections provide examples for the most common DataVerse tasksm including:
 
+* [List Projects](#list-projects)
 * [Create Project](#create-project)
 * [Get Project](#get-project)
 * [Create Dataset](#create-dataset)
 * [Get Dataset](#get-dataset)
 
 
+### List Projects
+The `list_projects` method will list all projects of the given sites.
+
+
+```Python
+projects = client.list_projects(current_user = True,
+                                exclude_sensor_type=SensorType.LIDAR,
+                                image_type= OntologyImageType._2D_BOUNDING_BOX)
+
+```
 ### Create Project
 
 The `create_project` method will create project on the connected site with the defined ontology and sensors.
 
 ```Python
 ontology = Ontology(
     name="test ot",
@@ -111,14 +122,15 @@
     "data_source": DataSource.Azure/Datasource.AWS,
     "storage_url": "storage/url",
     "container_name": "azure container name",
     "data_folder": "datafolder/to/vai_anno",
     "sas_token": "azure sas token",
     "name": "Dataset 1",
     "type": DatasetType.ANNOTATED_DATA,
+    "annotations": ["groundtruth"]
     "generate_metadata": False,
     "render_pcd": False,
     "annotation_format": AnnotationFormat.VISION_AI,
     "sequential": False,
     "sensors": project.sensors,
 }
 dataset = project.create_dataset(**dataset_data)
@@ -132,19 +144,20 @@
     "storage_url" : "",
     "container_name": "",
     "sas_token":"",
     "data_folder": "/path/to/your_localdir",
     "name": "Dataset Local Upload",
     "type": DatasetType.ANNOTATED_DATA,
     "generate_metadata": False,
+    "auto_tagging": ["weather"],
     "render_pcd": False,
     "annotation_format": AnnotationFormat.VISION_AI,
     "sequential": False,
     "sensors": project.sensors,
-    "extra_annotations" :['model_name']  #optional
+    "annotations" :['model_name']
 }
 dataset = project.create_dataset(**dataset_data)
 ```
 
 ## Get Dataset
 
 The `get_dataset` method retrieves the dataset info from the connected site. The `id` parameter is the unique interger ID of the dataset, not its "name" property.
```

### Comparing `dataverse-sdk-0.1.1/dataverse_sdk.egg-info/SOURCES.txt` & `dataverse-sdk-0.1.2/dataverse_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.1/setup.py` & `dataverse-sdk-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "dataverse-sdk"
-PACKAGE_VERSION = "0.1.1"
+PACKAGE_VERSION = "0.1.2"
 DESC = "Dataverse SDK For Python"
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
```

