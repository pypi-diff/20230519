# Comparing `tmp/gridappsd_python-2023.5.1a1.tar.gz` & `tmp/gridappsd_python-2023.5.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd_python-2023.5.1a1.tar", max compression
+gzip compressed data, was "gridappsd_python-2023.5.1a4.tar", max compression
```

## Comparing `gridappsd_python-2023.5.1a1.tar` & `gridappsd_python-2023.5.1a4.tar`

### file list

```diff
@@ -1,25 +1,17 @@
--rw-r--r--   0        0        0    10500 2023-05-11 02:03:47.316910 gridappsd_python-2023.5.1a1/README.md
--rw-r--r--   0        0        0     3756 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/__init__.py
--rw-r--r--   0        0        0     4620 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/__main__.py
--rw-r--r--   0        0        0     7189 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/app_registration.py
--rwxr-xr-x   0        0        0      555 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/conf/entrypoint.sh
--rwxr-xr-x   0        0        0      434 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/conf/run-gridappsd.sh
--rw-r--r--   0        0        0     4689 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/difference_builder.py
--rw-r--r--   0        0        0    27595 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/docker_handler.py
--rw-r--r--   0        0        0      227 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/field_interface/__init__.py
--rw-r--r--   0        0        0      280 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/field_interface/agents/__init__.py
--rw-r--r--   0        0        0    13624 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/field_interface/agents/agents.py
--rw-r--r--   0        0        0     1987 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/field_interface/context.py
--rw-r--r--   0        0        0     1840 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/field_interface/gridappsd_field_bus.py
--rw-r--r--   0        0        0     7538 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/field_interface/interfaces.py
--rw-r--r--   0        0        0    17130 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/goss.py
--rw-r--r--   0        0        0    12684 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/gridappsd.py
--rw-r--r--   0        0        0     3318 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/houses.py
--rw-r--r--   0        0        0     2723 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/loghandler.py
--rw-r--r--   0        0        0     2449 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/register_app.py
--rw-r--r--   0        0        0    12220 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/simulation.py
--rw-r--r--   0        0        0     3234 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/timeseries.py
--rw-r--r--   0        0        0    12052 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/topics.py
--rw-r--r--   0        0        0     3177 2023-05-11 02:03:47.320910 gridappsd_python-2023.5.1a1/gridappsd/utils.py
--rw-r--r--   0        0        0     1122 2023-05-11 02:04:36.901316 gridappsd_python-2023.5.1a1/pyproject.toml
--rw-r--r--   0        0        0    11455 1970-01-01 00:00:00.000000 gridappsd_python-2023.5.1a1/PKG-INFO
+-rw-r--r--   0        0        0    10500 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/README.md
+-rw-r--r--   0        0        0     3756 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/__init__.py
+-rw-r--r--   0        0        0     4620 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/__main__.py
+-rw-r--r--   0        0        0     7189 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/app_registration.py
+-rw-r--r--   0        0        0     4689 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/difference_builder.py
+-rw-r--r--   0        0        0    30366 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/docker_handler.py
+-rw-r--r--   0        0        0    17130 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/goss.py
+-rw-r--r--   0        0        0    12684 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/gridappsd.py
+-rw-r--r--   0        0        0     3318 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/houses.py
+-rw-r--r--   0        0        0     2723 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/loghandler.py
+-rw-r--r--   0        0        0     2449 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/register_app.py
+-rw-r--r--   0        0        0    12220 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/simulation.py
+-rw-r--r--   0        0        0     3234 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/timeseries.py
+-rw-r--r--   0        0        0    12052 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/topics.py
+-rw-r--r--   0        0        0     3177 2023-05-19 15:51:23.580363 gridappsd_python-2023.5.1a4/gridappsd/utils.py
+-rw-r--r--   0        0        0     1155 2023-05-19 15:52:30.433233 gridappsd_python-2023.5.1a4/pyproject.toml
+-rw-r--r--   0        0        0    11433 1970-01-01 00:00:00.000000 gridappsd_python-2023.5.1a4/PKG-INFO
```

### Comparing `gridappsd_python-2023.5.1a1/README.md` & `gridappsd_python-2023.5.1a4/README.md`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/__init__.py` & `gridappsd_python-2023.5.1a4/gridappsd/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/__main__.py` & `gridappsd_python-2023.5.1a4/gridappsd/__main__.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/app_registration.py` & `gridappsd_python-2023.5.1a4/gridappsd/app_registration.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/difference_builder.py` & `gridappsd_python-2023.5.1a4/gridappsd/difference_builder.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/docker_handler.py` & `gridappsd_python-2023.5.1a4/gridappsd/docker_handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,650 +1,723 @@
-#!/usr/bin/env python3
+# #!/usr/bin/env python3
 
-import contextlib
-import logging
-import os
-import random
-import re
-import shutil
-import tarfile
-import threading
-import urllib.request
-from copy import deepcopy
-from datetime import datetime, timedelta
-from pathlib import Path
-from pprint import pformat
-from subprocess import PIPE
-from typing import Optional, Union
-
-import stomp
-import time
-from docker.models.containers import Container
-
-from gridappsd import GridAPPSD
-from gridappsd.goss import GRIDAPPSD_ENV_ENUM
-
-logging.getLogger("urllib3.connectionpool").setLevel(logging.INFO)
-logging.getLogger("docker.auth").setLevel(logging.INFO)
-logging.getLogger("docker.utils").setLevel(logging.INFO)
-
-_log = logging.getLogger("gridappsd.docker_handler")
-
-
-try:
-    import docker
-    HAS_DOCKER = True
-except ImportError:
-    _log.warning("Docker api not loaded. pip install docker to install as package.")
-    HAS_DOCKER = False
-
-if HAS_DOCKER:
-
-    # The following variable is used for creating a volume for the gridappsd container
-    # to utilize.  It allows the ability to use multiple containers to run tests
-    # along side each other.
-    GRIDAPPSD_CONFIG_VOLUME_NAME = f"gridappsd_config_{random.randint(1,100)}"
-
-    # This named container will be used to hold configuration/folders so that other containers
-    # that start can use them.  To use add "volume_from": [CONFIGURATION_CONTAINER_NAME] and
-    # the mount point within the container will also be within the service container.
-    CONFIGURATION_CONTAINER_NAME = "testconfig"
-
-    def expand_all(user_path):
-        return os.path.expandvars(os.path.expanduser(user_path))
-
-    __TMP_ROOT__ = "/tmp/assets"
-    if Path(__TMP_ROOT__).exists():
-        shutil.rmtree(__TMP_ROOT__, ignore_errors=True)
-    os.makedirs(__TMP_ROOT__)
-
-    # This path needs to be the path to the repo where configuration files are located.
-    GRIDAPPSD_CONF_DIR = Path(__file__).resolve().parent.parent.joinpath("gridappsd/conf")
-
-    assert Path(GRIDAPPSD_CONF_DIR).joinpath("entrypoint.sh").exists()
-    assert Path(GRIDAPPSD_CONF_DIR).joinpath("run-gridappsd.sh").exists()
-
-    GRIDAPPSD_DATA_REPO = str(Path(__TMP_ROOT__).joinpath("mysql").resolve())
-
-    os.makedirs(GRIDAPPSD_DATA_REPO, exist_ok=True)
-    if not Path(GRIDAPPSD_DATA_REPO).is_dir():
-        raise AttributeError(f"Invalid GRIDAPPSD_DATA_REPO couldn't make or doesn't exist {GRIDAPPSD_DATA_REPO}")
-
-    MYSQL_SCHEMA_INIT_DIR = f'{GRIDAPPSD_DATA_REPO}/docker-entrypoint-initdb.d'
-
-
-    def mysql_setup():
-        """
-        Downloads gridappsd_mysql_dump.sql into the MYSQL_SCHEMA_INIT_DIR init directory.
-        This will then be mounted into the mysql container.
-        """
-        # Downlaod mysql file
-        _log.debug("Downloading mysql data file from Bootstrap repository")
-        mysql_file = f'{MYSQL_SCHEMA_INIT_DIR}/gridappsd_mysql_dump.sql'
-        if os.path.isdir(mysql_file):
-            raise RuntimeError(f"mysql datafile is directory, delete {mysql_file} using sudo rm -rf {mysql_file}")
-        if not os.path.isdir(MYSQL_SCHEMA_INIT_DIR):
-            os.makedirs(MYSQL_SCHEMA_INIT_DIR, 0o0775, exist_ok=True)
-        urllib.request.urlretrieve(
-            'https://raw.githubusercontent.com/GRIDAPPSD/Bootstrap/master/gridappsd_mysql_dump.sql',
-            filename=mysql_file)
-
-        # Modify the mysql file to allow connections from gridappsd container
-        with open(mysql_file, "r") as sources:
-            lines = sources.readlines()
-        with open(mysql_file, "w") as sources:
-            for line in lines:
-                sources.write(re.sub(r'localhost', '%', line))
-        assert Path(mysql_file).exists()
-
-    # Use the environmental variable if specified otherwise use the develop tag.
-    DEFAULT_GRIDAPPSD_TAG = os.environ.get('GRIDAPPSD_TAG_ENV', 'develop')
-
-    # Network to connect all of the containers up to by default.
-    NETWORK = "test_my_network"
-
-    __TPL_DEPENDENCY_CONFIG__ = {
-        "influxdb": {
-            "start": True,
-            "image": "gridappsd/influxdb:{{DEFAULT_GRIDAPPSD_TAG}}",
-            "pull": True,
-            "ports": {"8086/tcp": 8086},
-            "environment": {"INFLUXDB_DB": "proven"}
-        },
-        "redis": {
-            "start": True,
-            "image": "redis:3.2.11-alpine",
-            "pull": True,
-            "ports": {"6379/tcp": 6379},
-            "environment": [],
-            "entrypoint": "redis-server --appendonly yes",
-        },
-        "blazegraph": {
-            "start": True,
-            "image": "gridappsd/blazegraph:{{DEFAULT_GRIDAPPSD_TAG}}",
-            "pull": True,
-            "ports": {"8080/tcp": 8889},
-            "environment": []
-        },
-        "mysql": {
-            "start": True,
-            "image": "mysql/mysql-server:5.7",
-            "pull": True,
-            "ports": {"3306/tcp": 3306},
-            "environment": {
-                "MYSQL_RANDOM_ROOT_PASSWORD": "yes",
-                "MYSQL_PORT": "3306"
-            },
-            # "volumes": {
-            #     "/home/gridappsd/test-assets": {"bind": "/whatthehell", "mode": "rw"}
-            #     #"test-assets": {"bind": "/whatthehell", "mode": "rw"}
-            #     #data_dir + "/dumps/": {"bind": "/docker-entrypoint-initdb.d/", "mode": "ro"}
-            # },
-            # Our own so we can create
-            "volumes_required": [
-                dict(name="mysql_config",
-                     local_path=MYSQL_SCHEMA_INIT_DIR,
-                     container_path="/docker-entrypoint-initdb.d")
-            ],
-            "volumes_from": [
-                "mysql_config"
-            ],
-            "onsetupfn": mysql_setup
-        },
-        "proven": {
-            "start": True,
-            "image": "gridappsd/proven:{{DEFAULT_GRIDAPPSD_TAG}}",
-            "pull": True,
-            "ports": {"8080/tcp": 18080},
-            "environment": {
-                "PROVEN_SERVICES_PORT": "18080",
-                "PROVEN_SWAGGER_HOST_PORT": "localhost:18080",
-                "PROVEN_USE_IDB": "true",
-                "PROVEN_IDB_URL": "http://influxdb:8086",
-                "PROVEN_IDB_DB": "proven",
-                "PROVEN_IDB_RP": "autogen",
-                "PROVEN_IDB_USERNAME": "root",
-                "PROVEN_IDB_PASSWORD": "root",
-                "PROVEN_T3DIR": "/proven"},
-            "links": {"influxdb": "influxdb"}
-        }
-    }
-
-    __TPL_GRIDAPPSD_CONFIG__ = {
-        "gridappsd": {
-            "start": True,
-            "image": "gridappsd/gridappsd:{{DEFAULT_GRIDAPPSD_TAG}}",
-            "pull": True,
-            "ports": {"61613/tcp": 61613, "61614/tcp": 61614, "61616/tcp": 61616},
-            "environment": {
-                "PATH": "/gridappsd/bin:/gridappsd/lib:/gridappsd/services/fncsgossbridge/service:/usr/local/bin:/usr/local/sbin:/usr/sbin:/usr/bin:/sbin:/bin",
-                "DEBUG": 1,
-                "START": 1
-            },
-            "links": {"mysql": "mysql",
-                      "influxdb": "influxdb",
-                      "blazegraph": "blazegraph",
-                      "proven": "proven",
-                      "redis": "redis"},
-            "volumes_required": [
-                dict(name=GRIDAPPSD_CONFIG_VOLUME_NAME,
-                     local_path=GRIDAPPSD_CONF_DIR,
-                     container_path="/startup/conf")
-            ],
-            "volumes_from": [
-                GRIDAPPSD_CONFIG_VOLUME_NAME
-            ],
-            "entrypoint": "/startup/conf/entrypoint.sh",
-            "command": "/startup/conf/entrypoint.sh"
-        }
-    }
-
-    def __update_template_data__(data, update_dict):
-        data_cpy = deepcopy(data)
-        for k, v in data_cpy.items():
-            for u, p in update_dict.items():
-                v['image'] = v['image'].replace(u, p)
-
-        return data_cpy
-
-
-    __replace_dict__ = {"{{DEFAULT_GRIDAPPSD_TAG}}": DEFAULT_GRIDAPPSD_TAG}
-    DEFAULT_DOCKER_DEPENDENCY_CONFIG = __update_template_data__(__TPL_DEPENDENCY_CONFIG__, __replace_dict__)
-    DEFAULT_GRIDAPPSD_DOCKER_CONFIG = __update_template_data__(__TPL_GRIDAPPSD_CONFIG__, __replace_dict__)
-
-    def update_gridappsd_tag(new_gridappsd_tag):
-        """
-        Update the default tag used within the dependency and gridappsd containers to be
-        what is specified in the new gridappsd_tag variable
-        """
-        global DEFAULT_GRIDAPPSD_TAG
-
-        DEFAULT_GRIDAPPSD_TAG = new_gridappsd_tag
-        _log.info(f"Updated gridappsd docker tag {DEFAULT_GRIDAPPSD_TAG} ")
-        __replace_dict__.update({"{{DEFAULT_GRIDAPPSD_TAG}}": DEFAULT_GRIDAPPSD_TAG})
-        DEFAULT_DOCKER_DEPENDENCY_CONFIG.update(__update_template_data__(__TPL_DEPENDENCY_CONFIG__, __replace_dict__))
-        DEFAULT_GRIDAPPSD_DOCKER_CONFIG.update(__update_template_data__(__TPL_GRIDAPPSD_CONFIG__, __replace_dict__))
-
-
-    class Containers:
-        """
-        This class allows the creation/management of containers created by the gridappsd
-        docker process.
-        """
-        __client__ = docker.from_env()
-
-        def __init__(self, container_def):
-            self._container_def = container_def
-
-        @property
-        def container_def(self):
-            return self._container_def
-
-        @staticmethod
-        def remove_container(name):
-            try:
-                container = Containers.__client__.containers.get(name)
-                container.kill()
-            except docker.errors.NotFound:
-                _log.debug(f"container {name} not found so couldn't remove.")
-
-        @staticmethod
-        def container_list(ignore_list: Optional[Union[str, list]] = "gridappsd_dev"):
-            """
-            Provides a wrapper around the listing of docker containers.  This function was
-            brought about when running from within a docker container.
-
-            Currently the docker container that is run using docker-compose up from the
-            gridappsd-dev-environment is specified as gridappsd_dev, however this can change
-            and could potentially be extended to multiple named containers.
-
-            @param: ignore_list:
-                optional container names to not stop :: A string or list of strings
-            """
-
-            if ignore_list is None:
-                ignore_list = []
-            elif isinstance(ignore_list, str):
-                ignore_list = [ignore_list]
-            containers = []
-            for cont in Containers.__client__.containers.list():
-                if cont.name not in ignore_list:
-                    containers.append(cont)
-            return containers
-
-        @staticmethod
-        def reset_all_containers(ignore_list: Optional[Union[str, list]] = "gridappsd_dev"):
-            """
-            Provides a wrapper around the resetting of all docker containers.  This function was
-            brought about when running from within a docker container.
-
-            Currently the docker container that is run using docker-compose up from the
-            gridappsd-dev-environment is specified as gridappsd_dev, however this can change
-            and could potentially be extended to multiple named containers.
-
-            @param: ignore_list:
-                optional container names to not stop :: A string or list of strings
-            """
-            if ignore_list is None:
-                ignore_list = []
-            elif isinstance(ignore_list, str):
-                ignore_list = [ignore_list]
-
-            for cont in Containers.__client__.containers.list():
-                if cont.name not in ignore_list:
-                    cont.kill()
-
-        @staticmethod
-        def check_required_running(self, config):
-            my_config = deepcopy(config)
-
-            for c in Containers.__client__.containers.list():
-                my_config.pop(c.name, None)
-
-            assert not my_config, f"The required containers were not satisfied missing {list(my_config.keys())}"
-
-        @staticmethod
-        def create_volume_container(name, volume_name,
-                                    mount_in_container_at, restart_if_exists: bool = False,
-                                    mode="rw"):
-
-            _log.info(f"Creating container {name} and mounting volume {volume_name} "
-                      f"at {mount_in_container_at} in container {name}")
-            client = docker.from_env()
-
-            should_create = False
-            try:
-                cont = Containers.__client__.containers.get(name)
-            except docker.errors.NotFound:
-                # start container
-                should_create = True
-            else:
-                if restart_if_exists:
-                    should_create = True
-                    cont.stop()
-                else:
-                    return cont
-
-            if should_create:
-                kwargs = {}
-                kwargs['image'] = "alpine"
-                # Only name the containers if remove is on
-                kwargs['remove'] = True
-                kwargs['name'] = name
-                kwargs['detach'] = True
-                kwargs['volumes'] = {
-                    volume_name: {"bind": mount_in_container_at, "mode": mode}
-                }
-                # keep the container running
-                kwargs['command'] = "tail -f /dev/null"
-                cont = client.containers.run(**kwargs)
-                _log.info(f"New container for volume created {cont.name}")
-                # print(f"New container is: {container.name}")
-                return cont
-
-        @staticmethod
-        def create_get_network(name: str) -> docker.models.networks.Network:
-            try:
-                network = Containers.__client__.networks.get(name)
-            except docker.errors.NotFound:
-                network = Containers.__client__.networks.create(name, driver="bridge")
-
-            return network
-
-        @staticmethod
-        def copy_to(src: str, dst: str):
-            """
-            Copy a local directory onto a destination
-
-            .. note::
-
-                Make sure the dst (destination) is in the form container:directory
-
-            @param: src: The local directory to copy from the host
-            @param: dst: The container:destination to copy the src to.
-            """
-            _log.debug(f"copying folder from: {src} to {dst}")
-            src = str(src)
-            # python3.6 can't combine PosixPath and str
-            assert os.path.exists(src), f"{src} does not exist!"
-            client = docker.from_env()
-            name, dst = dst.split(':')
-            container = client.containers.get(name)
-            assert container is not None
-            cwd = os.getcwd()
-            os.chdir(os.path.dirname(src))
-            srcname = os.path.basename(src)
-            tarfilename = src + '.tar'
-            tar = tarfile.open(tarfilename, mode='w')
-            try:
-                tar.add(srcname)
-            finally:
-                tar.close()
-
-            data = open(tarfilename, 'rb').read()
-            resp = container.put_archive(os.path.dirname(dst), data)
-            os.chdir(cwd)
-            _log.debug(f"Response from put_archive {resp}")
-
-        def start(self):
-            _log.info("Starting containers")
-            # Containers.create_volume_container(CONFIGURATION_CONTAINER_NAME, "testconfig", "/testconfig")
-            #pprint(DEFAULT_GRIDAPPSD_DOCKER_CONFIG)
-            client = docker.from_env()
-            # print(f"Docker client version: {client.version()}")
-            for service, value in self._container_def.items():
-                _log.info(f"Pulling {service} image")
-                _log.info(f"Pulling {service} : {self._container_def[service]['image']}")
-                client.images.pull(self._container_def[service]['image'])
-                try:
-                    container = client.containers.get(service)
-                    self._container_def[service]['containerid'] = container.id
-                except docker.errors.NotFound:
-                    _log.debug(f"Couldn't find {service} so continuing on.")
-
-                # Provide a way to dynamically create things that the container will need
-                # on the host system.  This is important if we want to create a volume before
-                # starting the container up.
-                if value.get('onsetupfn'):
-                    value.get('onsetupfn')()
-
-                if self._container_def[service].get("volumes_required"):
-                    for vr in self._container_def[service].get("volumes_required"):
-                        _log.info(f"Creating volume for {service}: name={vr['name']}, "
-                                  f"volume_name={vr['name']}, container_path={vr['container_path']}")
-                        Containers.create_volume_container(
-                            name=vr["name"],
-                            volume_name=vr["name"],
-                            mount_in_container_at=vr["container_path"],
-                            restart_if_exists=True
-                            )
-                        time.sleep(20)
-                        if vr.get("local_path"):
-                            _log.debug(f"contents of local path({vr.get('local_path')}):\n\t{os.listdir(vr.get('local_path'))}")
-                            _log.info(f"Copy to mounted volume for {service}: "
-                                      f"local_path={vr['local_path']}, container_path={vr['container_path']}")
-                            Containers.copy_to(vr["local_path"], f'{vr["name"]}:{vr["container_path"]}')
-            network = Containers.create_get_network(NETWORK)
-            for service, value in self._container_def.items():
-                if self._container_def[service]['start']:
-                    _log.debug(f"Starting {service} : {self._container_def[service]['image']}")
-                    kwargs = {}
-                    kwargs['image'] = self._container_def[service]['image']
-                    # Only name the containers if remove is on
-                    kwargs['remove'] = True
-                    kwargs['name'] = service
-                    kwargs['detach'] = True
-                    kwargs['entrypoint'] = value.get('entrypoint')
-                    if self._container_def[service].get('entrypoint'):
-                        kwargs['entrypoint'] = value['entrypoint']
-                    if self._container_def[service].get('environment'):
-                        kwargs['environment'] = value['environment']
-                    if self._container_def[service].get('ports'):
-                        kwargs['ports'] = value['ports']
-                    if self._container_def[service].get('volumes'):
-                        kwargs['volumes'] = value['volumes']
-                    if self._container_def[service].get('entrypoint'):
-                        kwargs['entrypoint'] = value['entrypoint']
-                    # if self._container_def[service].get('links'):
-                    #     kwargs['links'] = value['links']
-                    if self._container_def[service].get('volumes_from'):
-                        kwargs['volumes_from'] = value['volumes_from']
-                    #for k, v in kwargs.items():
-                    #    print(f"k->{k}, v->{v}")
-                    _log.debug("Starting container with the following args:")
-                    _log.debug(f"{pformat(kwargs)}")
-                    launched_container = None
-                    try:
-                        container = client.containers.get(service)
-                        _log.debug("Found existing container")
-                    except docker.errors.NotFound:
-                        container = client.containers.run(**kwargs)
-                        _log.debug("Started new container")
-                        network.connect(container.id)
-                    self._container_def[service]['containerid'] = container.id
-            _log.debug(f"Current containers are: {[x.name for x in client.containers.list()]}")
-
-        def wait_for_log_pattern(self, container, pattern, timeout=60):
-            assert self._container_def.get(container), f"Container {container} is not in definition."
-            client = docker.from_env()
-            container = client.containers.get(self._container_def.get(container)['containerid'])
-            until = datetime.now() + timedelta(seconds=timeout)
-            for p in container.logs(stream=True, until=until):
-                _log.info(f"HANDLER: {p.decode('utf-8')}")
-                if pattern in p.decode('utf-8'):
-                    print(f"Found pattern {pattern}")
-                    return
-            raise TimeoutError(f"Pattern {pattern} was not found in logs of container {container} within {timeout}s")
-
-        def wait_for_http_ok(self, url, timeout=30):
-            import requests
-            results = None
-            test_count = 0
-
-            while results is None or not results.ok:
-                test_count += 1
-                if test_count > timeout:
-                    raise TimeoutError(f"Could not reach {url} within allotted timeout {timeout}s")
-                results = requests.get(url)
-                time.sleep(1)
-
-            print(f"Found url {url} within timeout {timeout}")
-
-        def stop(self):
-            client = docker.from_env()
-            for service, value in self._container_def.items():
-                if value.get('containerid'):
-                    try:
-                        cnt = client.containers.get(value.get('containerid'))
-                        cnt.kill()
-                        time.sleep(2)
-
-                        if "volumes_required" in value:
-                            # Loop over the volumes that are required for each image and
-                            # remove the volume.
-                            for volume_spec in value["volumes_required"]:
-                                Containers.remove_container(volume_spec['name'])
-                                time.sleep(2)
-
-                        # client.containers.get(value.get('containerid')).kill() # value.get('name')).kill()
-                    except docker.errors.NotFound as ex:
-                        _log.error(f"Volume {value.get('containerid')} was not found.")
-                        _log.exception(ex)
-
-
-    threads = []
-
-    def stream_container_log_to_file(container_name: str, logfile: str):
-        client = docker.from_env()
-        container = client.containers.list(filters=dict(name=container_name))[0]
-
-        print(container)
-
-        def log_output():
-            nonlocal container, logfile
-            print(f"Starting to write to file {logfile}.")
-            with open(logfile, 'wb') as fp:
-                print(f"openfile")
-                for p in container.logs(stream=True, stderr=PIPE, stdout=PIPE):
-                    fp.write(p)
-                    fp.flush()
-
-        threading.Thread(target=log_output, daemon=True).start()
-
-
-    @contextlib.contextmanager
-    def run_containers(config, stop_after=True) -> Containers:
-        containers = Containers(config)
-
-        containers.start()
-        try:
-            yield containers
-        finally:
-            if stop_after:
-                containers.stop()
-
-
-    @contextlib.contextmanager
-    def run_dependency_containers(stop_after=False) -> Containers:
-
-        containers = Containers(DEFAULT_DOCKER_DEPENDENCY_CONFIG)
-
-        containers.start()
-        try:
-            yield containers
-        finally:
-            if stop_after:
-                containers.stop()
-
-
-    @contextlib.contextmanager
-    def run_gridappsd_container(stop_after=True, rebuild_if_present=False) -> Container:
-        """ A contextmanager that uses """
-
-        parent_container = get_docker_in_docker()
-
-        client = docker.from_env()
-        # if there is a parent_container then we need to make sure that it is connected
-        # to the same network as our systems.  If not then we need to modify the network
-        # to include the parent container
-        if parent_container:
-            env = DEFAULT_GRIDAPPSD_DOCKER_CONFIG['gridappsd'].get('environment')
-            if env is None:
-                env = {}
-            env[GRIDAPPSD_ENV_ENUM.GRIDAPPSD_ADDRESS.name] = 'gridappsd'
-            env[GRIDAPPSD_ENV_ENUM.GRIDAPPSD_USER.name] = 'test_app_user'
-            env[GRIDAPPSD_ENV_ENUM.GRIDAPPSD_PASSWORD.name] = '4Test'
-            DEFAULT_GRIDAPPSD_DOCKER_CONFIG['gridappsd']['environment'] = env
-
-            _log.debug(f"Running inside a container environment: {parent_container.name}")
-            network = client.networks.get(NETWORK)
-            has_it = False
-            for x in network.containers:
-                if x.name == parent_container.name:
-                    has_it = True
-                    _log.debug(f"parent_container {parent_container.name} is connected to the network.")
-                    break
-            if not has_it:
-                _log.debug(f"Connecting new container to the network: {parent_container.name}")
-                network.connect(parent_container)
-        else:
-            _log.debug("Not running in a container")
-
-        containers = Containers(DEFAULT_GRIDAPPSD_DOCKER_CONFIG)
-
-        gridappsd_container = None
-        try:
-            gridappsd_container = client.containers.get("gridappsd")
-            _log.info(f"{gridappsd_container.name} container found")
-            if rebuild_if_present:
-                gridappsd_container.kill()
-        except docker.errors.NotFound:
-            _log.debug("gridappsd container not found!")
-
-        try:
-            if gridappsd_container is None:
-                containers.start()
-
-                # the gridappsd container itself will take a bit to start up.
-                time.sleep(30)
-
-                tries = 30
-                while True:
-                    tries -= 1
-                    if tries <=0:
-                        raise RuntimeError("Couldn't connect to gridappsd server in a timely manner!")
-                    try:
-                        g = GridAPPSD()
-                        if g.connected:
-                            _log.info("Connected to gridappsd!")
-                            g.disconnect()
-                            break
-
-                    except stomp.exception.ConnectFailedException or stomp.exception.NotConnectedException:
-                        _log.error("Retesting connection")
-
-            yield gridappsd_container
-        finally:
-            if stop_after:
-                containers.stop()
-
-
-    def get_docker_in_docker() -> Container:
-        """
-        Grab the parent container named the same as the current machine's hostname.  We are assuming that this
-        is going to be a container.
-        """
-        # There needs to be a test to make sure that the current container (assuming run in dev environment)
-        # is able to be run from the docker dev environment.  That environment is going to be assumed to be
-        # the same name as the host name of the container.  See the docker-compose starting the dev environment
-        hostname = str(open("/etc/hostname", "rt").read().strip())
-        client = docker.from_env()
-        try:
-            parent_container = client.containers.get(hostname)
-            _log.info(f"Inside parent container: {hostname}")
-            # Setup to use gridappsd as the connection address.  This value is used in the
-            # utils script to establish connection with the gridappsd server
-            os.environ["GRIDAPPSD_ADDRESS"] = "gridappsd"
-        except docker.errors.NotFound:
-            _log.debug(f"Docker container is not named this hostname {hostname}")
-            parent_container = None
-        return parent_container
+# import contextlib
+# import logging
+# import os
+# import random
+# import re
+# import shutil
+# import tarfile
+# import threading
+# import time
+# import urllib.request
+# from copy import deepcopy
+# from datetime import datetime, timedelta
+# from pathlib import Path
+# from pprint import pformat
+# from subprocess import PIPE
+# from typing import Optional, Union
+
+# import stomp
+
+# from gridappsd import GridAPPSD
+# from gridappsd.goss import GRIDAPPSD_ENV_ENUM
+
+# logging.getLogger("urllib3.connectionpool").setLevel(logging.INFO)
+# logging.getLogger("docker.auth").setLevel(logging.INFO)
+# logging.getLogger("docker.utils").setLevel(logging.INFO)
+
+# _log = logging.getLogger("gridappsd.docker_handler")
+
+# try:
+#     from python_on_whales import docker
+#     HAS_DOCKER = True
+# except ImportError:
+#     _log.warning(
+#         "Docker api not loaded. pip install docker to install as package.")
+#     HAS_DOCKER = False
+
+# if HAS_DOCKER:
+
+#     # The following variable is used for creating a volume for the gridappsd container
+#     # to utilize.  It allows the ability to use multiple containers to run tests
+#     # along side each other.
+#     GRIDAPPSD_CONFIG_VOLUME_NAME = f"gridappsd_config_{random.randint(1,100)}"
+
+#     # This named container will be used to hold configuration/folders so that other containers
+#     # that start can use them.  To use add "volume_from": [CONFIGURATION_CONTAINER_NAME] and
+#     # the mount point within the container will also be within the service container.
+#     CONFIGURATION_CONTAINER_NAME = "testconfig"
+
+#     def expand_all(user_path):
+#         return os.path.expandvars(os.path.expanduser(user_path))
+
+#     __TMP_ROOT__ = "/tmp/assets"
+#     if Path(__TMP_ROOT__).exists():
+#         shutil.rmtree(__TMP_ROOT__, ignore_errors=True)
+#     os.makedirs(__TMP_ROOT__)
+
+#     # This path needs to be the path to the repo where configuration files are located.
+#     GRIDAPPSD_CONF_DIR = Path(__file__).parent.parent.joinpath("conf")
+
+#     assert Path(GRIDAPPSD_CONF_DIR).joinpath("entrypoint.sh").exists()
+#     assert Path(GRIDAPPSD_CONF_DIR).joinpath("run-gridappsd.sh").exists()
+
+#     GRIDAPPSD_DATA_REPO = str(Path(__TMP_ROOT__).joinpath("mysql").resolve())
+
+#     os.makedirs(GRIDAPPSD_DATA_REPO, exist_ok=True)
+#     if not Path(GRIDAPPSD_DATA_REPO).is_dir():
+#         raise AttributeError(
+#             f"Invalid GRIDAPPSD_DATA_REPO couldn't make or doesn't exist {GRIDAPPSD_DATA_REPO}"
+#         )
+
+#     MYSQL_SCHEMA_INIT_DIR = f'{GRIDAPPSD_DATA_REPO}/docker-entrypoint-initdb.d'
+
+#     def mysql_setup():
+#         """
+#         Downloads gridappsd_mysql_dump.sql into the MYSQL_SCHEMA_INIT_DIR init directory.
+#         This will then be mounted into the mysql container.
+#         """
+#         # Downlaod mysql file
+#         _log.debug("Downloading mysql data file from Bootstrap repository")
+#         mysql_file = f'{MYSQL_SCHEMA_INIT_DIR}/gridappsd_mysql_dump.sql'
+#         if os.path.isdir(mysql_file):
+#             raise RuntimeError(
+#                 f"mysql datafile is directory, delete {mysql_file} using sudo rm -rf {mysql_file}"
+#             )
+#         if not os.path.isdir(MYSQL_SCHEMA_INIT_DIR):
+#             os.makedirs(MYSQL_SCHEMA_INIT_DIR, 0o0775, exist_ok=True)
+#         urllib.request.urlretrieve(
+#             'https://raw.githubusercontent.com/GRIDAPPSD/Bootstrap/master/gridappsd_mysql_dump.sql',
+#             filename=mysql_file)
+
+#         # Modify the mysql file to allow connections from gridappsd container
+#         with open(mysql_file, "r") as sources:
+#             lines = sources.readlines()
+#         with open(mysql_file, "w") as sources:
+#             for line in lines:
+#                 sources.write(re.sub(r'localhost', '%', line))
+#         assert Path(mysql_file).exists()
+
+#     # Use the environmental variable if specified otherwise use the develop tag.
+#     DEFAULT_GRIDAPPSD_TAG = os.environ.get('GRIDAPPSD_TAG_ENV', 'develop')
+
+#     # Network to connect all of the containers up to by default.
+#     NETWORK = "test_my_network"
+
+#     __TPL_DEPENDENCY_CONFIG__ = {
+#         "influxdb": {
+#             "start": True,
+#             "image": "gridappsd/influxdb:{{DEFAULT_GRIDAPPSD_TAG}}",
+#             "pull": True,
+#             "ports": {
+#                 "8086/tcp": 8086
+#             },
+#             "environment": {
+#                 "INFLUXDB_DB": "proven"
+#             }
+#         },
+#         "redis": {
+#             "start": True,
+#             "image": "redis:3.2.11-alpine",
+#             "pull": True,
+#             "ports": {
+#                 "6379/tcp": 6379
+#             },
+#             "environment": [],
+#             "entrypoint": "redis-server --appendonly yes",
+#         },
+#         "blazegraph": {
+#             "start": True,
+#             "image": "gridappsd/blazegraph:{{DEFAULT_GRIDAPPSD_TAG}}",
+#             "pull": True,
+#             "ports": {
+#                 "8080/tcp": 8889
+#             },
+#             "environment": []
+#         },
+#         "mysql": {
+#             "start":
+#             True,
+#             "image":
+#             "mysql/mysql-server:5.7",
+#             "pull":
+#             True,
+#             "ports": {
+#                 "3306/tcp": 3306
+#             },
+#             "environment": {
+#                 "MYSQL_RANDOM_ROOT_PASSWORD": "yes",
+#                 "MYSQL_PORT": "3306"
+#             },
+#             # "volumes": {
+#             #     "/home/gridappsd/test-assets": {"bind": "/whatthehell", "mode": "rw"}
+#             #     #"test-assets": {"bind": "/whatthehell", "mode": "rw"}
+#             #     #data_dir + "/dumps/": {"bind": "/docker-entrypoint-initdb.d/", "mode": "ro"}
+#             # },
+#             # Our own so we can create
+#             "volumes_required": [
+#                 dict(name="mysql_config",
+#                      local_path=MYSQL_SCHEMA_INIT_DIR,
+#                      container_path="/docker-entrypoint-initdb.d")
+#             ],
+#             "volumes_from": ["mysql_config"],
+#             "onsetupfn":
+#             mysql_setup
+#         },
+#         "proven": {
+#             "start": True,
+#             "image": "gridappsd/proven:{{DEFAULT_GRIDAPPSD_TAG}}",
+#             "pull": True,
+#             "ports": {
+#                 "8080/tcp": 18080
+#             },
+#             "environment": {
+#                 "PROVEN_SERVICES_PORT": "18080",
+#                 "PROVEN_SWAGGER_HOST_PORT": "localhost:18080",
+#                 "PROVEN_USE_IDB": "true",
+#                 "PROVEN_IDB_URL": "http://influxdb:8086",
+#                 "PROVEN_IDB_DB": "proven",
+#                 "PROVEN_IDB_RP": "autogen",
+#                 "PROVEN_IDB_USERNAME": "root",
+#                 "PROVEN_IDB_PASSWORD": "root",
+#                 "PROVEN_T3DIR": "/proven"
+#             },
+#             "links": {
+#                 "influxdb": "influxdb"
+#             }
+#         }
+#     }
+
+#     __TPL_GRIDAPPSD_CONFIG__ = {
+#         "gridappsd": {
+#             "start":
+#             True,
+#             "image":
+#             "gridappsd/gridappsd:{{DEFAULT_GRIDAPPSD_TAG}}",
+#             "pull":
+#             True,
+#             "ports": {
+#                 "61613/tcp": 61613,
+#                 "61614/tcp": 61614,
+#                 "61616/tcp": 61616
+#             },
+#             "environment": {
+#                 "PATH":
+#                 "/gridappsd/bin:/gridappsd/lib:/gridappsd/services/fncsgossbridge/service:/usr/local/bin:/usr/local/sbin:/usr/sbin:/usr/bin:/sbin:/bin",
+#                 "DEBUG": 1,
+#                 "START": 1
+#             },
+#             "links": {
+#                 "mysql": "mysql",
+#                 "influxdb": "influxdb",
+#                 "blazegraph": "blazegraph",
+#                 "proven": "proven",
+#                 "redis": "redis"
+#             },
+#             "volumes_required": [
+#                 dict(name=GRIDAPPSD_CONFIG_VOLUME_NAME,
+#                      local_path=GRIDAPPSD_CONF_DIR,
+#                      container_path="/startup/conf")
+#             ],
+#             "volumes_from": [GRIDAPPSD_CONFIG_VOLUME_NAME],
+#             "entrypoint":
+#             "/startup/conf/entrypoint.sh",
+#             "command":
+#             "/startup/conf/entrypoint.sh"
+#         }
+#     }
+
+#     def __update_template_data__(data, update_dict):
+#         data_cpy = deepcopy(data)
+#         for k, v in data_cpy.items():
+#             for u, p in update_dict.items():
+#                 v['image'] = v['image'].replace(u, p)
+
+#         return data_cpy
+
+#     __replace_dict__ = {"{{DEFAULT_GRIDAPPSD_TAG}}": DEFAULT_GRIDAPPSD_TAG}
+#     DEFAULT_DOCKER_DEPENDENCY_CONFIG = __update_template_data__(
+#         __TPL_DEPENDENCY_CONFIG__, __replace_dict__)
+#     DEFAULT_GRIDAPPSD_DOCKER_CONFIG = __update_template_data__(
+#         __TPL_GRIDAPPSD_CONFIG__, __replace_dict__)
+
+#     def update_gridappsd_tag(new_gridappsd_tag):
+#         """
+#         Update the default tag used within the dependency and gridappsd containers to be
+#         what is specified in the new gridappsd_tag variable
+#         """
+#         global DEFAULT_GRIDAPPSD_TAG
+
+#         DEFAULT_GRIDAPPSD_TAG = new_gridappsd_tag
+#         _log.info(f"Updated gridappsd docker tag {DEFAULT_GRIDAPPSD_TAG} ")
+#         __replace_dict__.update(
+#             {"{{DEFAULT_GRIDAPPSD_TAG}}": DEFAULT_GRIDAPPSD_TAG})
+#         DEFAULT_DOCKER_DEPENDENCY_CONFIG.update(
+#             __update_template_data__(__TPL_DEPENDENCY_CONFIG__,
+#                                      __replace_dict__))
+#         DEFAULT_GRIDAPPSD_DOCKER_CONFIG.update(
+#             __update_template_data__(__TPL_GRIDAPPSD_CONFIG__,
+#                                      __replace_dict__))
+
+#     class Containers:
+#         """
+#         This class allows the creation/management of containers created by the gridappsd
+#         docker process.
+#         """
+#         __client__ = docker.from_env()
+
+#         def __init__(self, container_def):
+#             self._container_def = container_def
+
+#         @property
+#         def container_def(self):
+#             return self._container_def
+
+#         @staticmethod
+#         def remove_container(name):
+#             try:
+#                 container = Containers.__client__.containers.get(name)
+#                 container.kill()
+#             except docker.errors.NotFound:
+#                 _log.debug(f"container {name} not found so couldn't remove.")
+
+#         @staticmethod
+#         def container_list(
+#                 ignore_list: Optional[Union[str, list]] = "gridappsd_dev"):
+#             """
+#             Provides a wrapper around the listing of docker containers.  This function was
+#             brought about when running from within a docker container.
+
+#             Currently the docker container that is run using docker-compose up from the
+#             gridappsd-dev-environment is specified as gridappsd_dev, however this can change
+#             and could potentially be extended to multiple named containers.
+
+#             @param: ignore_list:
+#                 optional container names to not stop :: A string or list of strings
+#             """
+
+#             if ignore_list is None:
+#                 ignore_list = []
+#             elif isinstance(ignore_list, str):
+#                 ignore_list = [ignore_list]
+#             containers = []
+#             for cont in Containers.__client__.containers.list():
+#                 if cont.name not in ignore_list:
+#                     containers.append(cont)
+#             return containers
+
+#         @staticmethod
+#         def reset_all_containers(
+#                 ignore_list: Optional[Union[str, list]] = "gridappsd_dev"):
+#             """
+#             Provides a wrapper around the resetting of all docker containers.  This function was
+#             brought about when running from within a docker container.
+
+#             Currently the docker container that is run using docker-compose up from the
+#             gridappsd-dev-environment is specified as gridappsd_dev, however this can change
+#             and could potentially be extended to multiple named containers.
+
+#             @param: ignore_list:
+#                 optional container names to not stop :: A string or list of strings
+#             """
+#             if ignore_list is None:
+#                 ignore_list = []
+#             elif isinstance(ignore_list, str):
+#                 ignore_list = [ignore_list]
+
+#             for cont in Containers.__client__.containers.list():
+#                 if cont.name not in ignore_list:
+#                     cont.kill()
+
+#         @staticmethod
+#         def check_required_running(self, config):
+#             my_config = deepcopy(config)
+
+#             for c in Containers.__client__.containers.list():
+#                 my_config.pop(c.name, None)
+
+#             assert not my_config, f"The required containers were not satisfied missing {list(my_config.keys())}"
+
+#         @staticmethod
+#         def create_volume_container(name,
+#                                     volume_name,
+#                                     mount_in_container_at,
+#                                     restart_if_exists: bool = False,
+#                                     mode="rw"):
+
+#             _log.info(
+#                 f"Creating container {name} and mounting volume {volume_name} "
+#                 f"at {mount_in_container_at} in container {name}")
+#             client = docker.from_env()
+
+#             should_create = False
+#             try:
+#                 cont = Containers.__client__.containers.get(name)
+#             except docker.errors.NotFound:
+#                 # start container
+#                 should_create = True
+#             else:
+#                 if restart_if_exists:
+#                     should_create = True
+#                     cont.stop()
+#                 else:
+#                     return cont
+
+#             if should_create:
+#                 kwargs = {}
+#                 kwargs['image'] = "alpine"
+#                 # Only name the containers if remove is on
+#                 kwargs['remove'] = True
+#                 kwargs['name'] = name
+#                 kwargs['detach'] = True
+#                 kwargs['volumes'] = {
+#                     volume_name: {
+#                         "bind": mount_in_container_at,
+#                         "mode": mode
+#                     }
+#                 }
+#                 # keep the container running
+#                 kwargs['command'] = "tail -f /dev/null"
+#                 cont = client.containers.run(**kwargs)
+#                 _log.info(f"New container for volume created {cont.name}")
+#                 # print(f"New container is: {container.name}")
+#                 return cont
+
+#         @staticmethod
+#         def create_get_network(name: str) -> docker.models.networks.Network:
+#             try:
+#                 network = Containers.__client__.networks.get(name)
+#             except docker.errors.NotFound:
+#                 network = Containers.__client__.networks.create(
+#                     name, driver="bridge")
+
+#             return network
+
+#         @staticmethod
+#         def copy_to(src: str, dst: str):
+#             """
+#             Copy a local directory onto a destination
+
+#             .. note::
+
+#                 Make sure the dst (destination) is in the form container:directory
+
+#             @param: src: The local directory to copy from the host
+#             @param: dst: The container:destination to copy the src to.
+#             """
+#             _log.debug(f"copying folder from: {src} to {dst}")
+#             src = str(src)
+#             # python3.6 can't combine PosixPath and str
+#             assert os.path.exists(src), f"{src} does not exist!"
+#             client = docker.from_env()
+#             name, dst = dst.split(':')
+#             container = client.containers.get(name)
+#             assert container is not None
+#             cwd = os.getcwd()
+#             os.chdir(os.path.dirname(src))
+#             srcname = os.path.basename(src)
+#             tarfilename = src + '.tar'
+#             tar = tarfile.open(tarfilename, mode='w')
+#             try:
+#                 tar.add(srcname)
+#             finally:
+#                 tar.close()
+
+#             data = open(tarfilename, 'rb').read()
+#             resp = container.put_archive(os.path.dirname(dst), data)
+#             os.chdir(cwd)
+#             _log.debug(f"Response from put_archive {resp}")
+
+#         def start(self):
+#             _log.info("Starting containers")
+#             # Containers.create_volume_container(CONFIGURATION_CONTAINER_NAME, "testconfig", "/testconfig")
+#             #pprint(DEFAULT_GRIDAPPSD_DOCKER_CONFIG)
+#             client = docker.from_env()
+#             # print(f"Docker client version: {client.version()}")
+#             for service, value in self._container_def.items():
+#                 _log.info(f"Pulling {service} image")
+#                 _log.info(
+#                     f"Pulling {service} : {self._container_def[service]['image']}"
+#                 )
+#                 client.images.pull(self._container_def[service]['image'])
+#                 try:
+#                     container = client.containers.get(service)
+#                     self._container_def[service]['containerid'] = container.id
+#                 except docker.errors.NotFound:
+#                     _log.debug(f"Couldn't find {service} so continuing on.")
+
+#                 # Provide a way to dynamically create things that the container will need
+#                 # on the host system.  This is important if we want to create a volume before
+#                 # starting the container up.
+#                 if value.get('onsetupfn'):
+#                     value.get('onsetupfn')()
+
+#                 if self._container_def[service].get("volumes_required"):
+#                     for vr in self._container_def[service].get(
+#                             "volumes_required"):
+#                         _log.info(
+#                             f"Creating volume for {service}: name={vr['name']}, "
+#                             f"volume_name={vr['name']}, container_path={vr['container_path']}"
+#                         )
+#                         Containers.create_volume_container(
+#                             name=vr["name"],
+#                             volume_name=vr["name"],
+#                             mount_in_container_at=vr["container_path"],
+#                             restart_if_exists=True)
+#                         time.sleep(20)
+#                         if vr.get("local_path"):
+#                             _log.debug(
+#                                 f"contents of local path({vr.get('local_path')}):\n\t{os.listdir(vr.get('local_path'))}"
+#                             )
+#                             _log.info(
+#                                 f"Copy to mounted volume for {service}: "
+#                                 f"local_path={vr['local_path']}, container_path={vr['container_path']}"
+#                             )
+#                             Containers.copy_to(
+#                                 vr["local_path"],
+#                                 f'{vr["name"]}:{vr["container_path"]}')
+#             network = Containers.create_get_network(NETWORK)
+#             for service, value in self._container_def.items():
+#                 if self._container_def[service]['start']:
+#                     _log.debug(
+#                         f"Starting {service} : {self._container_def[service]['image']}"
+#                     )
+#                     kwargs = {}
+#                     kwargs['image'] = self._container_def[service]['image']
+#                     # Only name the containers if remove is on
+#                     kwargs['remove'] = True
+#                     kwargs['name'] = service
+#                     kwargs['detach'] = True
+#                     kwargs['entrypoint'] = value.get('entrypoint')
+#                     if self._container_def[service].get('entrypoint'):
+#                         kwargs['entrypoint'] = value['entrypoint']
+#                     if self._container_def[service].get('environment'):
+#                         kwargs['environment'] = value['environment']
+#                     if self._container_def[service].get('ports'):
+#                         kwargs['ports'] = value['ports']
+#                     if self._container_def[service].get('volumes'):
+#                         kwargs['volumes'] = value['volumes']
+#                     if self._container_def[service].get('entrypoint'):
+#                         kwargs['entrypoint'] = value['entrypoint']
+#                     # if self._container_def[service].get('links'):
+#                     #     kwargs['links'] = value['links']
+#                     if self._container_def[service].get('volumes_from'):
+#                         kwargs['volumes_from'] = value['volumes_from']
+#                     #for k, v in kwargs.items():
+#                     #    print(f"k->{k}, v->{v}")
+#                     _log.debug("Starting container with the following args:")
+#                     _log.debug(f"{pformat(kwargs)}")
+#                     launched_container = None
+#                     try:
+#                         container = client.containers.get(service)
+#                         _log.debug("Found existing container")
+#                     except docker.errors.NotFound:
+#                         container = client.containers.run(**kwargs)
+#                         _log.debug("Started new container")
+#                         network.connect(container.id)
+#                     self._container_def[service]['containerid'] = container.id
+#             _log.debug(
+#                 f"Current containers are: {[x.name for x in client.containers.list()]}"
+#             )
+
+#         def wait_for_log_pattern(self, container, pattern, timeout=60):
+#             assert self._container_def.get(
+#                 container), f"Container {container} is not in definition."
+#             client = docker.from_env()
+#             container = client.containers.get(
+#                 self._container_def.get(container)['containerid'])
+#             until = datetime.now() + timedelta(seconds=timeout)
+#             for p in container.logs(stream=True, until=until):
+#                 _log.info(f"HANDLER: {p.decode('utf-8')}")
+#                 if pattern in p.decode('utf-8'):
+#                     print(f"Found pattern {pattern}")
+#                     return
+#             raise TimeoutError(
+#                 f"Pattern {pattern} was not found in logs of container {container} within {timeout}s"
+#             )
+
+#         def wait_for_http_ok(self, url, timeout=30):
+#             import requests
+#             results = None
+#             test_count = 0
+
+#             while results is None or not results.ok:
+#                 test_count += 1
+#                 if test_count > timeout:
+#                     raise TimeoutError(
+#                         f"Could not reach {url} within allotted timeout {timeout}s"
+#                     )
+#                 results = requests.get(url)
+#                 time.sleep(1)
+
+#             print(f"Found url {url} within timeout {timeout}")
+
+#         def stop(self):
+#             client = docker.from_env()
+#             for service, value in self._container_def.items():
+#                 if value.get('containerid'):
+#                     try:
+#                         cnt = client.containers.get(value.get('containerid'))
+#                         cnt.kill()
+#                         time.sleep(2)
+
+#                         if "volumes_required" in value:
+#                             # Loop over the volumes that are required for each image and
+#                             # remove the volume.
+#                             for volume_spec in value["volumes_required"]:
+#                                 Containers.remove_container(
+#                                     volume_spec['name'])
+#                                 time.sleep(2)
+
+#                         # client.containers.get(value.get('containerid')).kill() # value.get('name')).kill()
+#                     except docker.errors.NotFound as ex:
+#                         _log.error(
+#                             f"Volume {value.get('containerid')} was not found."
+#                         )
+#                         _log.exception(ex)
+
+#     threads = []
+
+#     def stream_container_log_to_file(container_name: str, logfile: str):
+#         client = docker.from_env()
+#         container = client.containers.list(filters=dict(
+#             name=container_name))[0]
+
+#         print(container)
+
+#         def log_output():
+#             nonlocal container, logfile
+#             print(f"Starting to write to file {logfile}.")
+#             with open(logfile, 'wb') as fp:
+#                 print(f"openfile")
+#                 for p in container.logs(stream=True, stderr=PIPE, stdout=PIPE):
+#                     fp.write(p)
+#                     fp.flush()
+
+#         threading.Thread(target=log_output, daemon=True).start()
+
+#     @contextlib.contextmanager
+#     def run_containers(config, stop_after=True) -> Containers:
+#         containers = Containers(config)
+
+#         containers.start()
+#         try:
+#             yield containers
+#         finally:
+#             if stop_after:
+#                 containers.stop()
+
+#     @contextlib.contextmanager
+#     def run_dependency_containers(stop_after=False) -> Containers:
+
+#         containers = Containers(DEFAULT_DOCKER_DEPENDENCY_CONFIG)
+
+#         containers.start()
+#         try:
+#             yield containers
+#         finally:
+#             if stop_after:
+#                 containers.stop()
+
+#     @contextlib.contextmanager
+#     def run_gridappsd_container(stop_after=True,
+#                                 rebuild_if_present=False) -> Container:
+#         """ A contextmanager that uses """
+
+#         parent_container = get_docker_in_docker()
+
+#         client = docker.from_env()
+#         # if there is a parent_container then we need to make sure that it is connected
+#         # to the same network as our systems.  If not then we need to modify the network
+#         # to include the parent container
+#         if parent_container:
+#             env = DEFAULT_GRIDAPPSD_DOCKER_CONFIG['gridappsd'].get(
+#                 'environment')
+#             if env is None:
+#                 env = {}
+#             env[GRIDAPPSD_ENV_ENUM.GRIDAPPSD_ADDRESS.name] = 'gridappsd'
+#             env[GRIDAPPSD_ENV_ENUM.GRIDAPPSD_USER.name] = 'test_app_user'
+#             env[GRIDAPPSD_ENV_ENUM.GRIDAPPSD_PASSWORD.name] = '4Test'
+#             DEFAULT_GRIDAPPSD_DOCKER_CONFIG['gridappsd']['environment'] = env
+
+#             _log.debug(
+#                 f"Running inside a container environment: {parent_container.name}"
+#             )
+#             network = client.networks.get(NETWORK)
+#             has_it = False
+#             for x in network.containers:
+#                 if x.name == parent_container.name:
+#                     has_it = True
+#                     _log.debug(
+#                         f"parent_container {parent_container.name} is connected to the network."
+#                     )
+#                     break
+#             if not has_it:
+#                 _log.debug(
+#                     f"Connecting new container to the network: {parent_container.name}"
+#                 )
+#                 network.connect(parent_container)
+#         else:
+#             _log.debug("Not running in a container")
+
+#         containers = Containers(DEFAULT_GRIDAPPSD_DOCKER_CONFIG)
+
+#         gridappsd_container = None
+#         try:
+#             gridappsd_container = client.containers.get("gridappsd")
+#             _log.info(f"{gridappsd_container.name} container found")
+#             if rebuild_if_present:
+#                 gridappsd_container.kill()
+#         except docker.errors.NotFound:
+#             _log.debug("gridappsd container not found!")
+
+#         try:
+#             if gridappsd_container is None:
+#                 containers.start()
+
+#                 # the gridappsd container itself will take a bit to start up.
+#                 time.sleep(30)
+
+#                 tries = 30
+#                 while True:
+#                     tries -= 1
+#                     if tries <= 0:
+#                         raise RuntimeError(
+#                             "Couldn't connect to gridappsd server in a timely manner!"
+#                         )
+#                     try:
+#                         g = GridAPPSD()
+#                         if g.connected:
+#                             _log.info("Connected to gridappsd!")
+#                             g.disconnect()
+#                             break
+
+#                     except stomp.exception.ConnectFailedException or stomp.exception.NotConnectedException:
+#                         _log.error("Retesting connection")
+
+#             yield gridappsd_container
+#         finally:
+#             if stop_after:
+#                 containers.stop()
+
+#     def get_docker_in_docker() -> Container:
+#         """
+#         Grab the parent container named the same as the current machine's hostname.  We are assuming that this
+#         is going to be a container.
+#         """
+#         # There needs to be a test to make sure that the current container (assuming run in dev environment)
+#         # is able to be run from the docker dev environment.  That environment is going to be assumed to be
+#         # the same name as the host name of the container.  See the docker-compose starting the dev environment
+#         hostname = str(open("/etc/hostname", "rt").read().strip())
+#         client = docker.from_env()
+#         try:
+#             parent_container = client.containers.get(hostname)
+#             _log.info(f"Inside parent container: {hostname}")
+#             # Setup to use gridappsd as the connection address.  This value is used in the
+#             # utils script to establish connection with the gridappsd server
+#             os.environ["GRIDAPPSD_ADDRESS"] = "gridappsd"
+#         except docker.errors.NotFound:
+#             _log.debug(
+#                 f"Docker container is not named this hostname {hostname}")
+#             parent_container = None
+#         return parent_container
```

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/goss.py` & `gridappsd_python-2023.5.1a4/gridappsd/goss.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/gridappsd.py` & `gridappsd_python-2023.5.1a4/gridappsd/gridappsd.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/houses.py` & `gridappsd_python-2023.5.1a4/gridappsd/houses.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/loghandler.py` & `gridappsd_python-2023.5.1a4/gridappsd/loghandler.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/register_app.py` & `gridappsd_python-2023.5.1a4/gridappsd/register_app.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/simulation.py` & `gridappsd_python-2023.5.1a4/gridappsd/simulation.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/timeseries.py` & `gridappsd_python-2023.5.1a4/gridappsd/timeseries.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/topics.py` & `gridappsd_python-2023.5.1a4/gridappsd/topics.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/gridappsd/utils.py` & `gridappsd_python-2023.5.1a4/gridappsd/utils.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.5.1a1/pyproject.toml` & `gridappsd_python-2023.5.1a4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-python"
-version = "2023.5.1a1"
+version = "2023.5.1a4"
 description = "A GridAPPS-D Python Adapter"
 authors = [
     "C. Allwardt <3979063+craig8@users.noreply.github.com>",
     "P. Sharma <poorva.sharma@pnnl.gov",
     "A. Fisher <andrew.fisher@pnnl.gov"
 ]
 license = "BSD-3-Clause"
@@ -30,19 +30,21 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7.9,<4.0"
 PyYAML = "^6.0"
 pytz = "^2022.7"
 dateutils = "^0.6.7"
 stomp-py = "6.0.0"
-cim-graph = "^0.1.20230413185916a0"
+requests = "2.28.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.2"
 pytest-html = "^3.1.1"
 mock = "^4.0.3"
-docker = "^4.4.4"
 yapf = "^0.32.0"
+mypy = "^1.3.0"
+python-on-whales = "^0.60.1"
+gitpython = "^3.1.31"
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gridappsd_python-2023.5.1a1/PKG-INFO` & `gridappsd_python-2023.5.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: gridappsd-python
-Version: 2023.5.1a1
+Version: 2023.5.1a4
 Summary: A GridAPPS-D Python Adapter
 Home-page: https://gridappsd.readthedocs.io
 License: BSD-3-Clause
 Keywords: gridappsd,grid,activmq,powergrid,simulation,library
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.7.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: cim-graph (>=0.1.20230413185916a0,<0.2.0)
 Requires-Dist: dateutils (>=0.6.7,<0.7.0)
 Requires-Dist: pytz (>=2022.7,<2023.0)
+Requires-Dist: requests (==2.28.2)
 Requires-Dist: stomp-py (==6.0.0)
 Project-URL: Repository, https://github.com/GRIDAPPSD/gridappsd-python
 Description-Content-Type: text/markdown
 
 [![Run All Pytests](https://github.com/GRIDAPPSD/gridappsd-python/actions/workflows/run-pytest.yml/badge.svg)](https://github.com/GRIDAPPSD/gridappsd-python/actions/workflows/run-pytest.yml)
 
 # gridappsd-python
```

