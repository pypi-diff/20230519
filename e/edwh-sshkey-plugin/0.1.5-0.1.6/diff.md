# Comparing `tmp/edwh_sshkey_plugin-0.1.5.tar.gz` & `tmp/edwh_sshkey_plugin-0.1.6.tar.gz`

## Comparing `edwh_sshkey_plugin-0.1.5.tar` & `edwh_sshkey_plugin-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,11 @@
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/.idea/.gitignore
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/.idea/edwh-sshkey-plugin.iml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/.idea/misc.xml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/.idea/vcs.xml
--rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/.idea/workspace.xml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/.idea/shelf/Uncommitted_changes_before_Update_at_12-05-2023_17_23__Changes_.xml
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/.idea/shelf/Uncommitted_changes_before_Update_at_12-05-2023_17_23_[Changes]/shelved.patch
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/pynguin-report/statistics.csv
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/src/edwh_sshkey_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/src/edwh_sshkey_plugin/__init__.py
--rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/src/edwh_sshkey_plugin/fabfile.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/README.md
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.6/pynguin-report/statistics.csv
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.6/src/edwh_sshkey_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.6/src/edwh_sshkey_plugin/__init__.py
+-rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.6/src/edwh_sshkey_plugin/fabfile.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.6/README.md
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 edwh_sshkey_plugin-0.1.6/PKG-INFO
```

### Comparing `edwh_sshkey_plugin-0.1.5/CHANGELOG.md` & `edwh_sshkey_plugin-0.1.6/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.6 (2023-05-19)
+### Fix
+* Ssh-key and sshkey being used separate now only sshkey. Also added git ignore to remove __pycache__ and .idea ([`a47d082`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/a47d082e723f83f4b02625f6237069f1104248bb))
+* Message requirement change, now you don't need to fill it in but it will still give you a prompt if not filled in now just custom ([`08460fe`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/08460fe1e05ef771cb97a4b7b7eab3eff023b24f))
+* Installation guide being incorrect ([`19a9e15`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/19a9e153becb99fa322a3eaec8cc46ec9b061607))
+* Project.urls now go to the correct urls ([`cdfb180`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/cdfb180e934fb2c60de9c01c0d648870af9526ac))
+* Optional dependencies not in pyproject.toml. so new .[dev] installable ([`b36c45e`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/b36c45ed459efee159342ca8514484731b8a9546))
+* Open.read() -> pathlib readlines ([`46b4a22`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/46b4a2288b3a0ffe0515b9ae37ad25ff49a7244d))
+* Documentation ([`7b96edc`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/7b96edcb5078b4af79a1291f96c1f1a601060794))
+
 ## v0.1.5 (2023-05-15)
 ### Fix
 * Fix that some people get a os.getlogin() error, os.getlogin() returns the name of the user logged in on the controlling terminal of the process. Typically processes in user session (tty, X session) have a controlling terminal. Processes spawned by a service manager like init, systemd, or upstart usually do not have a controlling terminal. You have to get the user information by other means. Our documentation for os.getlogin() recommends getpass.getuser(). which is used ([`4437128`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/44371287c9a02688b1277517641222845510be13))
 
 ## v0.1.4 (2023-05-15)
 ### Fix
 * Error messages improvements and key generation gives more info with the keys ([`e82a53a`](https://github.com/educationwarehouse/edwh-sshkey-plugin/commit/e82a53a565a7cf1416b4794d10dfbf1eabd4288d))
```

### Comparing `edwh_sshkey_plugin-0.1.5/.idea/shelf/Uncommitted_changes_before_Update_at_12-05-2023_17_23_[Changes]/shelved.patch` & `edwh_sshkey_plugin-0.1.6/src/edwh_sshkey_plugin/fabfile.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,428 @@
-Index: src/edwh_sshkey_plugin/fabfile.py
-IDEA additional info:
-Subsystem: com.intellij.openapi.diff.impl.patch.BaseRevisionTextPatchEP
-<+>from fabric import task\nfrom datetime import datetime\nfrom yaml.loader import SafeLoader\nimport pathlib\nimport yaml\nimport time\nimport os\nimport subprocess\nimport platform\n\n# the path where the yaml file with the keys is stored\nYAML_KEYS_PATH = pathlib.Path(\"~/.ssh/known_keys.yaml\").expanduser()\n\n\ndef create_new_keyholder():\n    \"\"\"\n    When a user wants to add a keys for the first time, this function will be called.\n    It's to create a new yaml file where the keys will be stored.\n    \"\"\"\n    with open(YAML_KEYS_PATH, \"x\") as new_key_holder:\n        new_key_holder.close()\n\n\ndef create_new_yaml_file_if_not_exists():\n    \"\"\"\n    Checks if the yaml file exists, if not it will create a new one.\n    \"\"\"\n    if not YAML_KEYS_PATH.exists():\n        create_new_keyholder()\n\n\ndef open_new_keyholder(read: bool):\n    \"\"\"\n    To open the yaml file, this function will be called.\n    \"\"\"\n    if YAML_KEYS_PATH.exists():\n        return open(YAML_KEYS_PATH, \"r\" if read else \"w\")\n    else:\n        create_new_keyholder()\n\n\ndef get_keys_from_keyholder():\n    \"\"\"\n    This function retrieves keys from a keyholder.\n\n    The function first opens a new keyholder and loads its contents as a dictionary using the yaml library.\n    If the keyholder is empty, the function prints an error message and exits with code 255.\n    Otherwise, it returns a dictionary of keys from the keyholder.\n\n    :return: A dictionary of keys from the keyholder.\n    \"\"\"\n    # It opens the keyholder and loads its contents as a dictionary using the yaml library.\n    key_holder = open_new_keyholder(True)\n    key_db: dict = yaml.load(key_holder, Loader=SafeLoader)\n    # This checks if the keyholder is empty. If empty -> exit with code 255\n    if key_db is None:\n        print(\n            \"functionality for generating local keys automaticly and adding them to the keyholder currently isn't supported\"\n        )\n        print(\"please run create to generate a new key\")\n        exit(255)\n    # This returns a dictionary of keys from the keyholder.\n    return dict(key_db.setdefault(\"keys\"))\n\n\ndef get_key_count(keys, command_line_key):\n    \"\"\"\n    This function takes in two arguments: a list of keys and a command line key. It returns the number of times the keys appear in the command line key.\n\n    :param keys: A list of keys to search for in the command line key.\n    :type keys: list\n    :param command_line_key: The command line key to search for the keys in.\n    :type command_line_key: str\n    :return: The number of times the keys appear in the command line key.\n    :rtype: int\n    \"\"\"\n    # The length of the list of keys that appear in the command line key is returned.\n    return len([key for key in keys if key in command_line_key])\n\n\ndef add_keys_to_remote(c, command_line_keys, all_key_information):\n    \"\"\"\n    Adds SSH keys to a remote server's authorized keys file.\n\n    :param c: An object representing a connection to the remote server.\n    :type c: Connection\n    :param command_line_keys: A list of keys to be added to the remote server.\n    :type command_line_keys: list\n    :param all_key_information: A dictionary containing information about all available keys.\n    :type all_key_information: dict\n    \"\"\"\n    # If the user enters a key that isn't in the YAML file, it will break out of the loop.\n    for command_line_key in command_line_keys:\n        if command_line_key not in all_key_information:\n            break\n\n        all_key_information_remote_items = dict(\n            all_key_information[command_line_key].items()\n        )\n\n        keys = [\n            name\n            for name in [\"key\", \"datetime\", \"who@hostname\", \"message\"]\n            if name in all_key_information_remote_items\n        ]\n\n        # 4 as in the 4 items in the dictionary above (key, datetime, who@hostname, message)\n        if len(keys) == 4:\n            # It puts the keys in the authorized_keys file on the remote server.\n            # So the public key is now on the remote server.\n            # This means that the user can now log in to the remote server using the private key.\n            c.run(\n                f'echo \"{all_key_information_remote_items[\"key\"]}\" >> ~/.ssh/authorized_keys'\n            )\n            # This is a way to check if the key is already in the authorized_keys file.\n            # By making another file with all the keys and call the function 'sort -u' on it.\n            # This function sorts the keys and removes duplicates.\n            c.run(\"touch ~/.ssh/keys\")\n            c.run(\"sort -u ~/.ssh/authorized_keys > ~/.ssh/keys\")\n            time.sleep(1)\n            c.run(\"cp ~/.ssh/keys ~/.ssh/authorized_keys\")\n            c.run(\"rm ~/.ssh/keys\")\n            print(\n                f\"It worked out! The \\033[1m{command_line_key}\\033[0m key is added to the remote server.\"\n            )\n\n\ndef remote_key_doesnt_exist(c, command_line_keys, all_key_information):\n    \"\"\"\n    This function checks if the keys provided in the command line are present in the YAML file.\n    If a key is not present in the YAML file, the user is prompted to create it.\n\n    :param c: Connection object\n    :param command_line_keys: List of keys provided in the command line\n    :param all_key_information: Dictionary containing all key information from the YAML file\n    \"\"\"\n    # removing all keys that are already in the yaml file, so we can create the ones that are not in the yaml file\n    # and then add them to the yaml file\n    not_in_yaml_keys = [\n        which_key\n        for which_key in command_line_keys\n        if which_key not in all_key_information.keys()\n    ]\n    print(\n        f'Wrong \\033[1m{\" \".join(not_in_yaml_keys)}\\033[0m key, '\n        f\"first check if you filled in the right key. Or if it is in the YAML file.\"\n    )\n    # Here is the '-' replaced with a space, so it can be used in the generate function.\n    # The generate function requires two out of three arguments to be filled in. So that's why the key is split.\n    for which_key in not_in_yaml_keys:\n        if \"-\" not in which_key:\n            print(f\"\\033[1m{which_key}\\033[0m isn't a valid host-name please give it up with the format: owner-hostname-goal\")\n            continue\n\n        new_key = which_key.replace(\"-\", \" \")\n\n        # Create the key that isn't in the YAML file.\n        if input(f\"Do you want to create {which_key}? [Y/n]: \").replace(\" \", \"\") in (\n            \"y\",\n            \"Y\",\n            \"\",\n        ):\n            generate_message = str(\n                input(\"What message do you want to go with the ssh-key? REQUIRED: \")\n            )\n            if not generate_message:\n                print(\"Please give up a message for the next time!\")\n                exit(1)\n            key_split = new_key.split()\n\n            if len(key_split) > 3:\n                print(f\"to many arguments given in the key: {which_key} format needs to be: owner-hostname-goal\")\n\n            # This is to create a new key, the split is to make sure that the key is in the right format.\n            generate(\n                c,\n                generate_message,\n                owner=key_split[0],\n                hostname=key_split[1],\n                goal=new_key.split()[2] if len(key_split) == 3 else \"\",\n            )\n            # eventually it will add the keys that are just created\n            add_to_remote(c, command_line_keys)\n\n\n@task(\n    help={\n        \"keys-to-remote\": \"list of keys you want to add to the remote server\",\n    },\n    iterable=[\"keys_to_remote\"],\n)\ndef add_to_remote(c, keys_to_remote: list):\n    \"\"\"\n    Adds the specified SSH key(s) to the remote machine. You can add multiple keys at once.\n\n    The private/public key is located local in the ~/.managed_ssh_keys-{key_name} directory.\n    You can see who has the private/public key, by looking at the YAML file.\n    There is a key called 'who@hostname', that's the person who created the new ssh key.\n\n\n    If there are keys that are not in the YAML file, the user is prompted to create them.\n    NOTE: you must provide a message, otherwise the program will terminate.\n    \"\"\"\n    # If keys_to_remote is a string, convert it to a list with a single element\n    if type(keys_to_remote) == str:\n        keys_to_remote = [keys_to_remote]\n\n    # check which keys are already in the YAML file\n    all_key_information = dict(get_keys_from_keyholder())\n\n    # check if given keys exist else ask to generate them\n    key_count = get_key_count(all_key_information.keys(), keys_to_remote)\n\n    if key_count == len(keys_to_remote):\n        add_keys_to_remote(c, keys_to_remote, all_key_information)\n    else:\n        remote_key_doesnt_exist(c, keys_to_remote, all_key_information)\n\n\n@task(\n    help={\n        \"keys_to_remote\": \"list of keys you want to remove from the server\",\n    },\n    iterable=[\"keys_to_remote\"],\n)\ndef delete_remote(c, keys_to_remote):\n    \"\"\"\n    Removes the specified SSH key(s) from the remote machine. You can remove multiple keys at once.\n    \"\"\"\n    # If keys_to_remote is a string, convert it to a list with a single element\n    if type(keys_to_remote) == str:\n        keys_to_remote = [keys_to_remote]\n\n    # Get all key information from the keyholder\n    all_key_information = get_keys_from_keyholder()\n\n    # Loop through each key specified in keys_to_remote\n    for command_line_key in keys_to_remote:\n        # If the key is not found in all_key_information, break out of the loop\n        if command_line_key not in all_key_information:\n            break\n\n        # Get the SSH key from all_key_information and remove newlines\n        ssh_key = dict(all_key_information[command_line_key].items())[\"key\"].replace(\n            \"\\n\", \"\"\n        )\n        # Remove the key from the remote server's authorized_keys file\n        c.run(f'grep -v \"{ssh_key}\" ~/.ssh/authorized_keys > ~/.ssh/keys')\n        c.run(\"mv ~/.ssh/keys ~/.ssh/authorized_keys\")\n        # Print a success message\n        print(f\"Success! The {command_line_key} key has been removed.\")\n\n\n@task(\n    help={\n        \"message\": \"a message to know what the key is used for, REQUIRED\",\n        \"owner\": \"owner of the server you are generating a key for\",\n        \"hostname\": \"hostname of the server you are generating the key for\",\n        \"goal\": \"What is the goal to use this key for, for example: 'production' or 'testing''\",\n    }\n)\ndef generate(c, message, owner=\"\", hostname=\"\", goal=\"\"):\n    \"\"\"\n    This function generates a new SSH key and saves it to a yaml file. (~/.ssh/known_keys.yaml)\n\n    You need a message and 2 out of 3 arguments to generate a new key. (owner, hostname, goal) Otherwise it will fail.\n\n    The private/public key is located local in the ~/.managed_ssh_keys-{key_name} directory.\n    You can see who has the private/public key, by looking at the YAML file.\n    There is a key called 'who@hostname', that's the person who created the new ssh key.\n    \"\"\"\n    # Create a new YAML file if it does not already exist\n    create_new_yaml_file_if_not_exists()\n\n    # Create a key name by joining the non-empty values of owner, hostname, and goal with a hyphen\n    key_name = \"-\".join(filter(bool, [owner, hostname, goal]))\n    # If less than two of three from owner, hostname, and goal are provided, print an error message and return\n    if sum([owner != \"\", hostname != \"\", goal != \"\"]) < 2:\n        print(\n            \"Please provide at least two of the following arguments: Owner, Hostname, goal\"\n        )\n        return\n\n    # If a file with the specified key name already exists, print an error message and return\n    if pathlib.Path(f\"~/.managed_ssh_keys-{key_name}\").expanduser().exists():\n        print(f\"{key_name} already exists. Key generation aborted.\")\n        return\n\n    # Run the ssh-keygen command to generate a new SSH key\n    # As type of key we use rsa, with a bit size of 4096\n    # The key is saved in ~/.ssh/.managed_ssh_keys-{key_name}\n    # The key has no passphrase\n    # The key has given a comment with the message\n    subprocess.run(\n        f'ssh-keygen -t rsa -b 4096 -f ~/.ssh/.managed_ssh_keys-{key_name} -N \"\" -C \"{message}\"',\n        shell=True,\n    )\n\n    # Open the YAML_KEYS_PATH file in append mode\n    with open(YAML_KEYS_PATH, \"a\") as f:\n        # Dump the key information to the YAML file\n        yaml.dump(\n            {\n                \"keys\": {\n                    key_name: {\n                        \"key\": open(\n                            pathlib.Path(\n                                f\"~/.ssh/.managed_ssh_keys-{key_name}.pub\"\n                            ).expanduser()\n                        ).read(),\n                        \"datetime\": datetime.today().strftime(\n                            \"Datum: %Y-%m-%d Tijdstip: %H:%M:%S\"\n                        ),\n                        \"who@hostname\": f\"{os.getlogin()}@{platform.node()}\",\n                        \"message\": message,\n                    }\n                }\n            },\n            f,\n            indent=4,\n        )\n    # Print a success message\n    print(f\"Public key saved in ~/.managed_ssh_keys-{key_name}.pub\")\n    print(f\"Private key saved in ~/.managed_ssh_keys-{key_name}\")\n\n\n@task()\ndef list(c):\n    \"\"\"\n    Lists all the local or local and remote ssh_keys.\n    This function lists the authorized keys on a remote machine and compares them with the keys in a local YAML file.\n    It separates the keys into three categories: local keys, remote known keys, and unrecognized keys.\n    \"\"\"\n    # Load the keys from the YAML file\n    all_key_information = get_keys_from_keyholder()\n\n    # Get the list of authorized keys from the remote machine\n    if len(c.run(\"ls ~/.ssh/authorized_keys\", warn=True, hide=True).stdout) > 0:\n        remote_keys = c.run(\"cat ~/.ssh/authorized_keys\", hide=True).stdout\n    else:\n        remote_keys = \"\"\n\n    # Iterate through the keys and separate them into two lists\n    local_keys = []\n    remote_known_keys = []\n    for key_data in all_key_information.values():\n        if key_data[\"key\"] in remote_keys:\n            remote_known_keys.append(key_data[\"key\"].replace(\"\\n\", \"\"))\n        else:\n            local_keys.append(key_data[\"key\"])\n\n    remote_keys = remote_keys.split(\"\\n\")\n\n    # Check for any unrecognized keys in the authorized_keys file\n    if len(c.run(\"ls ~/.ssh/authorized_keys\", warn=True, hide=True).stdout) > 0:\n        unrecognized_keys = [\n            remote_key\n            for remote_key in remote_keys\n            if remote_key not in remote_known_keys and remote_key != \"\"\n        ]\n    else:\n        unrecognized_keys = [\n            remote_key for remote_key in remote_keys if remote_key != \"\"\n        ]\n\n    if unrecognized_keys:\n        print(\"\\033[1mUnrecognized keys found in remote auth_keys:\\033[0m\")\n        # If there are unrecognized keys, print them with a number, so you can see how many there are.\n        for index in range(len(unrecognized_keys)):\n            print(f\"key {index+1}\")\n            print(unrecognized_keys[index])\n            print()\n        print()\n\n    # Display the keys in a table\n    if local_keys or remote_known_keys:\n        if local_keys:\n            print(\"\\033[1mLocal Keys\\033[0m\")\n            for key in local_keys:\n                print(f\"\\033[33m{key}\\033[0m\")\n\n        if remote_known_keys:\n            print(\"\\033[1mRemote Keys\\033[0m\")\n            for key in remote_known_keys:\n                print(f\"\\033[33m{key}\\033[0m\")\n    else:\n        print(\"No keys found in key_holder.yaml\")\n
-Subsystem: com.intellij.openapi.diff.impl.patch.CharsetEP
-<+>UTF-8
-===================================================================
-diff --git a/src/edwh_sshkey_plugin/fabfile.py b/src/edwh_sshkey_plugin/fabfile.py
---- a/src/edwh_sshkey_plugin/fabfile.py	(revision 94445e2968148e18eaddd14506e8eb1c0b7bd6e9)
-+++ b/src/edwh_sshkey_plugin/fabfile.py	(date 1683905006298)
-@@ -385,3 +385,6 @@
-                 print(f"\033[33m{key}\033[0m")
-     else:
-         print("No keys found in key_holder.yaml")
-+
-+@task
-+def test(c):
+import fabric.connection
+import invoke
+from fabric import task
+from datetime import datetime
+from yaml.loader import SafeLoader
+import pathlib
+import yaml
+import os
+import subprocess
+import platform
+import getpass
+
+# the path where the yaml file with the keys is stored
+YAML_KEYS_PATH = pathlib.Path("~/.ssh/known_keys.yaml").expanduser()
+
+
+def local_connection(c):
+    return "invoke" in str(type(c))
+
+
+def create_new_yaml_file_if_not_exists():
+    """
+    Checks if the yaml file exists, if not it will create a new one.
+    """
+    if not YAML_KEYS_PATH.exists():
+        YAML_KEYS_PATH.touch()
+
+
+def open_new_keyholder(read: bool):
+    """
+    To open the yaml file, this function will be called.
+    """
+    create_new_yaml_file_if_not_exists()
+    return YAML_KEYS_PATH.open("r" if read else "w")
+
+
+def get_keys_from_keyholder(gen=False) -> dict:
+    """
+    This function retrieves keys from a keyholder.
+
+    The function first opens a new keyholder and loads its contents as a dictionary using the yaml library.
+    If the keyholder is empty, the function prints an error message and exits with code 255.
+    Otherwise, it returns a dictionary of keys from the keyholder.
+
+    :return: A dictionary of keys from the keyholder.
+    """
+    # It opens the keyholder and loads its contents as a dictionary using the yaml library.
+    key_holder = open_new_keyholder(True)
+    key_db: dict = yaml.load(key_holder, Loader=SafeLoader)
+    # This checks if the keyholder is empty. If empty -> exit with code 255
+    if key_db is None:
+        if gen:
+            return {}
+
+        print(
+            "functionality for generating local keys automaticly and adding them to the keyholder currently isn't supported"
+        )
+        print("please run `ew sshkey.generate` to generate a new key")
+        exit(255)
+
+    # This returns a dictionary of keys from the keyholder.
+    return dict(key_db.setdefault("keys"))
+
+
+def get_key_count(keys, command_line_key):
+    """
+    This function takes in two arguments: a list of keys and a command line key. It returns the number of times the keys appear in the command line key.
+
+    :param keys: A list of keys to search for in the command line key.
+    :type keys: list
+    :param command_line_key: The command line key to search for the keys in.
+    :type command_line_key: str
+    :return: The number of times the keys appear in the command line key.
+    :rtype: int
+    """
+    # The length of the list of keys that appear in the command line key is returned.
+    return len([key for key in keys if key in command_line_key])
+
+
+def add_keys_to_remote(c, command_line_keys, all_key_information):
+    """
+    Adds SSH keys to a remote server's authorized keys file.
+
+    :param c: An object representing a connection to the remote server.
+    :type c: Connection
+    :param command_line_keys: A list of keys to be added to the remote server.
+    :type command_line_keys: list
+    :param all_key_information: A dictionary containing information about all available keys.
+    :type all_key_information: dict
+    """
+    # If the user enters a key that isn't in the YAML file, it will break out of the loop.
+    for command_line_key in command_line_keys:
+        if command_line_key not in all_key_information:
+            break
+
+        all_key_information_remote_items = all_key_information[command_line_key]
+
+        if all(
+            attr in all_key_information_remote_items
+            for attr in ("key", "datetime", "who@hostname", "message")
+        ):
+            # It puts the keys in the authorized_keys file on the remote server.
+            # So the public key is now on the remote server.
+            # This means that the user can now log in to the remote server using the private key.
+            c.run(
+                f'echo "{all_key_information_remote_items["key"]}" >> ~/.ssh/authorized_keys'
+            )
+            # This is a way to check if the key is already in the authorized_keys file.
+            # By making another file with all the keys and call the function 'sort -u' on it.
+            # This function sorts the keys and removes duplicates.
+            c.run("sort -u ~/.ssh/authorized_keys > ~/.ssh/keys")
+            c.run("mv ~/.ssh/keys ~/.ssh/authorized_keys")
+            print(
+                f"It worked out! The \033[1m{command_line_key}\033[0m key is added to the remote server."
+            )
+
+
+def remote_key_doesnt_exist(c, command_line_keys, all_key_information):
+    """
+    This function checks if the keys provided in the command line are present in the YAML file.
+    If a key is not present in the YAML file, the user is prompted to create it.
+
+    :param c: Connection object
+    :param command_line_keys: List of keys provided in the command line
+    :param all_key_information: Dictionary containing all key information from the YAML file
+    """
+    # removing all keys that are already in the yaml file, so we can create the ones that are not in the yaml file
+    # and then add them to the yaml file
+    not_in_yaml_keys = [
+        which_key
+        for which_key in command_line_keys
+        if which_key not in all_key_information.keys()
+    ]
+    print(
+        f'Wrong \033[1m{" ".join(not_in_yaml_keys)}\033[0m key, '
+        f"first check if you filled in the right key. Or if it is in the YAML file."
+    )
+    # Here is the '-' replaced with a space, so it can be used in the generate function.
+    # The generate function requires two out of three arguments to be filled in. So that's why the key is split.
+    for which_key in not_in_yaml_keys:
+        if "-" not in which_key:
+            print(
+                f"\033[1m{which_key}\033[0m isn't a valid host-name please give it up with the format: owner-hostname-goal"
+            )
+            continue
+
+        new_key = which_key.replace("-", " ")
+
+        # Create the key that isn't in the YAML file.
+        if input(f"Do you want to create {which_key}? [Y/n]: ").replace(" ", "") in (
+            "y",
+            "Y",
+            "",
+        ):
+            generate_message = str(
+                input("What message do you want to go with the sshkey? REQUIRED: ")
+            )
+            if not generate_message:
+                print("Please give up a message for the next time!")
+                exit(1)
+            key_split = new_key.split()
+
+            if len(key_split) > 3:
+                print(
+                    f"to many arguments given in the key: {which_key} format needs to be: owner-hostname-goal"
+                )
+                exit(1)
+
+            # This is to create a new key, the split is to make sure that the key is in the right format.
+            generate(
+                c,
+                generate_message,
+                owner=key_split[0],
+                hostname=key_split[1],
+                goal=new_key.split()[2] if len(key_split) == 3 else "",
+            )
+            # eventually it will add the keys that are just created
+            add(c, command_line_keys)
+
+
+@task(
+    help={
+        "keys-to-remote": "list of keys you want to add to the remote server",
+    },
+    iterable=["keys_to_remote"],
+)
+def add(c, keys_to_remote: list):
+    """
+    Adds the specified SSH key(s) to the remote machine. You can add multiple keys at once.
+
+    The private/public key is located local in the ~/.managed_ssh_keys-{key_name} directory.
+    You can see who has the private/public key, by looking at the YAML file.
+    There is a key called 'who@hostname', that's the person who created the new ssh key.
+
+
+    If there are keys that are not in the YAML file, the user is prompted to create them.
+    NOTE: you must provide a message, otherwise the program will terminate.
+    """
+    if local_connection(c):
+        if input("are you sure you want to add local keys(Y/n): ").replace(
+            " ", ""
+        ) not in ["Y", "y", ""]:
+            print("please use `edwh -H ubuntu@user.nl sshkey.add because ")
+            exit(255)
+        else:
+            print("Adding keys to local known_hosts")
+
+    # If keys_to_remote is a string, convert it to a list with a single element
+    if type(keys_to_remote) == str:
+        keys_to_remote = [keys_to_remote]
+
+    # check which keys are already in the YAML file
+    all_key_information = get_keys_from_keyholder()
+
+    # check if given keys exist else ask to generate them
+    key_count = get_key_count(all_key_information.keys(), keys_to_remote)
+
+    if key_count == len(keys_to_remote):
+        add_keys_to_remote(c, keys_to_remote, all_key_information)
+    else:
+        remote_key_doesnt_exist(c, keys_to_remote, all_key_information)
+
+
+@task(
+    help={
+        "keys_to_remote": "list of keys you want to remove from the server",
+    },
+    iterable=["keys_to_remote"],
+)
+def delete(c, keys_to_remote):
+    """
+    Removes the specified SSH key(s) from the remote machine. You can remove multiple keys at once.
+    """
+    if local_connection(c):
+        if input("are you sure you want to add local keys(Y/n").replace(
+            " ", ""
+        ) not in ["Y", "y", ""]:
+            print("please use `edwh -H ubuntu@user.nl sshkey.delete to remove remote keys ")
+            exit(255)
+        else:
+            print("Removing local keys from known_hosts")
+
+    # If keys_to_remote is a string, convert it to a list with a single element
+    if isinstance(keys_to_remote, str):
+        keys_to_remote = [keys_to_remote]
+
+    # Get all key information from the keyholder
+    all_key_information = get_keys_from_keyholder()
+
+    # Loop through each key specified in keys_to_remote
+    for command_line_key in keys_to_remote:
+        # If the key is not found in all_key_information, break out of the loop
+        if command_line_key not in all_key_information:
+            break
+
+        # Get the SSH key from all_key_information and remove newlines
+        ssh_key = all_key_information[command_line_key]["key"].strip()
+        # Remove the key from the remote server's authorized_keys file
+        c.run(f'grep -v "{ssh_key}" ~/.ssh/authorized_keys > ~/.ssh/keys')
+        c.run("mv ~/.ssh/keys ~/.ssh/authorized_keys")
+        # Print a success message
+        print(f"Success! The {command_line_key} key has been removed.")
+    else:
+        print("please give up keys using edwh.sshkey.delete -k [keys]")
+
+
+@task(
+    help={
+        "message": "a message to know what the key is used for, REQUIRED",
+        "owner": "owner of the server you are generating a key for",
+        "hostname": "hostname of the server you are generating the key for",
+        "goal": "What is the goal to use this key for, for example: 'production' or 'testing'",
+    }
+)
+def generate(c, message="", owner="", hostname="", goal=""):
+    """
+    This function generates a new SSH key and saves it to a yaml file. (~/.ssh/known_keys.yaml)
+
+    You need a message and 2 out of 3 arguments to generate a new key. (owner, hostname, goal) Otherwise it will fail.
+
+    The private and public key is located local in the ~/.managed_ssh_keys-{key_name} directory.
+    You can see who has the private/public key, by looking at the YAML file.
+    There is a key called 'who@hostname', that's the person who created the new ssh key.
+    """
+
+    if not message:
+        print("please use `edwh sshkey.generate -m {message} {required args}` to proceed")
+
+    # Get the yaml keys or create a new YAML file if it does not already exist
+    keys_dict = {"keys": {}}
+    current_keys = get_keys_from_keyholder(gen=True)
+
+    # Create a key name by joining the non-empty values of owner, hostname, and goal with a hyphen
+    key_name = "-".join(_ for _ in (owner, hostname, goal) if _)
+    # If less than two of three from owner, hostname, and goal are provided, print an error message and return
+    if "-" not in key_name:
+        print(
+            "Please provide at least two of the following arguments: Owner, Hostname, goal"
+        )
+        return
+
+    # If a file with the specified key name already exists, print an error message and return
+    if pathlib.Path(f"~/.managed_ssh_keys-{key_name}").expanduser().exists():
+        print(f"{key_name} already exists. Key generation aborted.")
+        return
+
+    # Run the ssh-keygen command to generate a new SSH key
+    # As type of key we use rsa, with a bit size of 4096
+    # The key is saved in ~/.ssh/.managed_ssh_keys-{key_name}
+    # The key has no passphrase
+    # The key has given a comment with the message
+    curr_time = datetime.now().strftime("Datum: %Y-%m-%d Tijdstip: %H:%M:%S")
+    host = f"{getpass.getuser()}@{platform.node()}"
+
+    subprocess.run(
+        f'ssh-keygen -t rsa -b 4096 -f ~/.ssh/.managed_ssh_keys-{key_name} -N "" -C "key name: {key_name} '
+        f'message: {message} who@hostname: {host} {curr_time}"',
+        shell=True,
+    )
+    keys_dict["keys"].update(current_keys)
+    keys_dict["keys"][key_name] = {
+        "key": pathlib.Path(f"~/.ssh/.managed_ssh_keys-{key_name}.pub").expanduser().read_text(),
+        "datetime": curr_time,
+        "who@hostname": host,
+        "message": message,
+    }
+
+    # Open the YAML_KEYS_PATH file in append mode
+    with open(YAML_KEYS_PATH, "w") as f:
+        # Dump the key information to the YAML file
+        yaml.dump(
+            keys_dict,
+            f,
+            indent=4,
+        )
+    # Print a success message
+    print(f"Public key saved in ~/.managed_ssh_keys-{key_name}.pub")
+    print(f"Private key saved in ~/.managed_ssh_keys-{key_name}")
+
+
+def get_keys(c, private):
+    if not private:
+        return get_keys_from_keyholder()
+
+    key_names = get_keys_from_keyholder()
+    keys = {}
+    for key_name in key_names:
+        # we should only be able to find 1 key
+        private_key_file = pathlib.Path(f"~/.ssh/.managed_ssh_keys-{key_name}").expanduser()
+
+        if private_key_file is None:
+            print(f"[ERROR] private key for {key_name} not found!")
+            print("exiting....")
+            exit(1)
+
+            # reinact yaml file so we don't need to parse this differently
+        keys[key_name] = {"key": private_key_file.read_text()}
+    return keys
+
+
+@task(name="list")
+def list_(c, private=False):
+    """
+    Lists all the local or local and remote ssh_keys.
+    This function lists the authorized keys on a remote machine and compares them with the keys in a local YAML file.
+    It separates the keys into three categories: local keys, remote known keys, and unrecognized keys.
+    """
+    # Load the keys from the YAML file
+    all_key_information = get_keys(c, private)
+
+    # Get the list of authorized keys from the remote machine
+    if len(c.run("ls ~/.ssh/authorized_keys", warn=True, hide=True).stdout) > 0:
+        remote_keys = c.run("cat ~/.ssh/authorized_keys", hide=True).stdout
+    else:
+        remote_keys = ""
+
+    # Iterate through the keys and separate them into two lists
+    key_names = {}
+    local_keys = []
+    remote_known_keys = []
+    for key in all_key_information.keys():
+        key_data = all_key_information[key]
+        if key_data["key"] in remote_keys:
+            remote_known_keys.append(key_data["key"].replace("\n", ""))
+        else:
+            local_keys.append(key_data["key"])
+
+        key_names[key_data["key"]] = key
+    remote_keys = remote_keys.split("\n")
+
+    # Check for any unrecognized keys in the authorized_keys file
+    if len(c.run("ls ~/.ssh/authorized_keys", warn=True, hide=True).stdout) > 0:
+        unrecognized_keys = [
+            remote_key
+            for remote_key in remote_keys
+            if remote_key not in remote_known_keys and remote_key != ""
+        ]
+    else:
+        unrecognized_keys = [
+            remote_key for remote_key in remote_keys if remote_key != ""
+        ]
+
+    if unrecognized_keys:
+        print("\033[1mUnrecognized keys found in remote auth_keys:\033[0m")
+        # If there are unrecognized keys, print them with a number, so you can see how many there are.
+        for index in range(len(unrecognized_keys)):
+            print(f"key {index+1}")
+            print(unrecognized_keys[index])
+            print()
+        print()
+
+    # Display the keys in a table
+    if local_keys or remote_known_keys:
+        if local_keys and local_connection(c):
+            print("\033[1mLocal Keys\033[0m")
+            for key in local_keys:
+                print(f"Key {key_names[key]}:")
+                print(f"\033[33m{key}\033[0m")
+
+        if remote_known_keys:
+            print("\033[1mRemote Keys\033[0m")
+            for key in remote_known_keys:
+                print(f"Key {key_names[key]}:")
+                print(f"\033[33m{key}\033[0m")
+        elif not local_connection(c):
+            print("\033[1mNo remote keys have been found!\033[0m")
+    else:
+        print("No keys found in key_holder.yaml")
```

### Comparing `edwh_sshkey_plugin-0.1.5/tests/__init__.py` & `edwh_sshkey_plugin-0.1.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `edwh_sshkey_plugin-0.1.5/LICENSE.txt` & `edwh_sshkey_plugin-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_sshkey_plugin-0.1.5/README.md` & `edwh_sshkey_plugin-0.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # edwh-sshkey-plugin
 
-[![PyPI - Version](https://img.shields.io/pypi/v/edwh-demo-plugin.svg)](https://pypi.org/project/edwh-demo-plugin)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-demo-plugin.svg)](https://pypi.org/project/edwh-demo-plugin)
+[![PyPI - Version](https://img.shields.io/pypi/v/edwh-sshkey-plugin.svg)](https://pypi.org/project/edwh-sshkey-plugin)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-sshkey-plugin.svg)](https://pypi.org/project/edwh-sshkey-plugin)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Guide](#guide)
@@ -13,27 +13,33 @@
 - [Adding keys](#adding-keys-to-remote)
 - [Removing keys](#removing-ssh-keys-from-a-remote-machine)
 - [Listing Local/Remote Keys](#list-ssh-keys-from-a-remote-or-local-machine)
 - [License](#license)
 
 ## Installation
 
+To install all edwh related plugins
 ```console
-pip install edwh-sshkey-plugin
+pipx install edwh[plugins,all,omgeving]
+```
+
+To only install edwh sshkey plugin
+```console
+pipx install edwh[sshkey]
 ```
 
 ## Guide
 ### Generating new keys:
 example for ubuntu@user.nl
 ```console
-edwh sshkey.generate --message={message} --owner=ubuntu --hostname=user --doel=nl
+edwh sshkey.generate --message={message} --owner=ubuntu --hostname=user --goal=nl
 ```
 
 possible arguments for `ew sshkey.generate`:
-- **message**: REQUIRED, message to give with the ssh-keygen
+- **message**: REQUIRED, message to give with the generated key
 - **owner**: owner of the server you are generating a key for
 - **hostname**: hostname of the server you are generating the key for
 - **goal**: What is the goal to use this key for, for example: 'production' or 'testing'
 
 #### note:
 you atleast need to give this function 2-3 parameters and a message else it will not work.
 
@@ -68,8 +74,8 @@
 edwh sshkey.list -H ubuntu@user.nl
 ```
 
 #### Note:
 this list all found known and unknown keys on the local or remote server.
 
 ## License
-`edwh-ssh-key-plugin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`edwh-sshkey-plugin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `edwh_sshkey_plugin-0.1.5/pyproject.toml` & `edwh_sshkey_plugin-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -21,18 +21,25 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ['invoke']
 
+[project.optional-dependencies]
+dev = [
+    "hatch",
+    # "python-semantic-release",
+    "black",
+]
+
 [project.urls]
-Documentation = "https://github.com/remcoboerma/edwh_sshkey_plugin#readme"
-Issues = "https://github.com/remcoboerma/edwh_sshkey_plugin/issues"
-Source = "https://github.com/remcoboerma/edwh_sshkey_plugin"
+Documentation = "https://github.com/educationwarehouse/edwh-sshkey-plugin#readme"
+Issues = "https://github.com/educationwarehouse/edwh-sshkey-plugin/issues"
+Source = "https://github.com/educationwarehouse/edwh-sshkey-plugin"
 
 # https://packaging.python.org/en/latest/guides/creating-and-discovering-plugins/#using-package-metadata
 [project.entry-points."edwh.tasks"]
 sshkey = "edwh_sshkey_plugin.fabfile"
 
 [tool.hatch.version]
 path = "src/edwh_sshkey_plugin/__about__.py"
```

### Comparing `edwh_sshkey_plugin-0.1.5/PKG-INFO` & `edwh_sshkey_plugin-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: edwh-sshkey-plugin
-Version: 0.1.5
+Version: 0.1.6
 Summary: plugin for adding and removing keys to servers
-Project-URL: Documentation, https://github.com/remcoboerma/edwh_sshkey_plugin#readme
-Project-URL: Issues, https://github.com/remcoboerma/edwh_sshkey_plugin/issues
-Project-URL: Source, https://github.com/remcoboerma/edwh_sshkey_plugin
+Project-URL: Documentation, https://github.com/educationwarehouse/edwh-sshkey-plugin#readme
+Project-URL: Issues, https://github.com/educationwarehouse/edwh-sshkey-plugin/issues
+Project-URL: Source, https://github.com/educationwarehouse/edwh-sshkey-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: invoke
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: hatch; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # edwh-sshkey-plugin
 
-[![PyPI - Version](https://img.shields.io/pypi/v/edwh-demo-plugin.svg)](https://pypi.org/project/edwh-demo-plugin)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-demo-plugin.svg)](https://pypi.org/project/edwh-demo-plugin)
+[![PyPI - Version](https://img.shields.io/pypi/v/edwh-sshkey-plugin.svg)](https://pypi.org/project/edwh-sshkey-plugin)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-sshkey-plugin.svg)](https://pypi.org/project/edwh-sshkey-plugin)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Guide](#guide)
@@ -33,27 +36,33 @@
 - [Adding keys](#adding-keys-to-remote)
 - [Removing keys](#removing-ssh-keys-from-a-remote-machine)
 - [Listing Local/Remote Keys](#list-ssh-keys-from-a-remote-or-local-machine)
 - [License](#license)
 
 ## Installation
 
+To install all edwh related plugins
 ```console
-pip install edwh-sshkey-plugin
+pipx install edwh[plugins,all,omgeving]
+```
+
+To only install edwh sshkey plugin
+```console
+pipx install edwh[sshkey]
 ```
 
 ## Guide
 ### Generating new keys:
 example for ubuntu@user.nl
 ```console
-edwh sshkey.generate --message={message} --owner=ubuntu --hostname=user --doel=nl
+edwh sshkey.generate --message={message} --owner=ubuntu --hostname=user --goal=nl
 ```
 
 possible arguments for `ew sshkey.generate`:
-- **message**: REQUIRED, message to give with the ssh-keygen
+- **message**: REQUIRED, message to give with the generated key
 - **owner**: owner of the server you are generating a key for
 - **hostname**: hostname of the server you are generating the key for
 - **goal**: What is the goal to use this key for, for example: 'production' or 'testing'
 
 #### note:
 you atleast need to give this function 2-3 parameters and a message else it will not work.
 
@@ -88,8 +97,8 @@
 edwh sshkey.list -H ubuntu@user.nl
 ```
 
 #### Note:
 this list all found known and unknown keys on the local or remote server.
 
 ## License
-`edwh-ssh-key-plugin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`edwh-sshkey-plugin` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

