# Comparing `tmp/rpa_cooperativa-1.0.53.tar.gz` & `tmp/rpa_cooperativa-1.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.53.tar", last modified: Fri May  5 19:21:45 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.54.tar", last modified: Fri May 19 18:59:18 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.53.tar` & `rpa_cooperativa-1.0.54.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:21:45.174346 rpa_cooperativa-1.0.53/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.53/LICENSE
--rw-rw-rw-   0        0        0     6670 2023-05-05 19:21:45.167732 rpa_cooperativa-1.0.53/PKG-INFO
--rw-rw-rw-   0        0        0     5525 2023-05-03 11:36:32.000000 rpa_cooperativa-1.0.53/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 19:21:44.922557 rpa_cooperativa-1.0.53/rpa_coop/
--rw-rw-rw-   0        0        0      568 2023-05-02 17:34:09.000000 rpa_cooperativa-1.0.53/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:21:45.084693 rpa_cooperativa-1.0.53/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.53/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.53/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.53/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.53/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.53/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.53/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.53/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.53/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.53/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.53/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.53/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    80721 2023-05-05 19:08:06.000000 rpa_cooperativa-1.0.53/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:21:45.153839 rpa_cooperativa-1.0.53/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6670 2023-05-05 19:21:43.000000 rpa_cooperativa-1.0.53/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-05-05 19:21:44.000000 rpa_cooperativa-1.0.53/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:21:43.000000 rpa_cooperativa-1.0.53/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-05 19:21:43.000000 rpa_cooperativa-1.0.53/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      559 2023-05-05 19:21:43.000000 rpa_cooperativa-1.0.53/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 19:21:43.000000 rpa_cooperativa-1.0.53/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 19:21:45.177345 rpa_cooperativa-1.0.53/setup.cfg
--rw-rw-rw-   0        0        0     2325 2023-05-05 19:03:14.000000 rpa_cooperativa-1.0.53/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:59:18.875618 rpa_cooperativa-1.0.54/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.54/LICENSE
+-rw-rw-rw-   0        0        0     6875 2023-05-19 18:59:18.869056 rpa_cooperativa-1.0.54/PKG-INFO
+-rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.54/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 18:59:18.437703 rpa_cooperativa-1.0.54/rpa_coop/
+-rw-rw-rw-   0        0        0      585 2023-05-19 18:39:16.000000 rpa_cooperativa-1.0.54/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:59:18.748006 rpa_cooperativa-1.0.54/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.54/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.54/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.54/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.54/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.54/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.54/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.54/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.54/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.54/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.54/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.54/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    82582 2023-05-19 18:55:16.000000 rpa_cooperativa-1.0.54/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-05-19 18:59:18.853073 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6875 2023-05-19 18:59:17.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-05-19 18:59:18.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 18:59:17.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-19 18:59:17.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      559 2023-05-19 18:59:17.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-19 18:59:17.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 18:59:18.880302 rpa_cooperativa-1.0.54/setup.cfg
+-rw-rw-rw-   0        0        0     2325 2023-05-19 18:38:52.000000 rpa_cooperativa-1.0.54/setup.py
```

### Comparing `rpa_cooperativa-1.0.53/LICENSE` & `rpa_cooperativa-1.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.53/PKG-INFO` & `rpa_cooperativa-1.0.54/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.53
+Version: 1.0.54
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
@@ -74,14 +74,25 @@
 
 time.sleep(1)
 driver.get(url)
 time.sleep(1)
 driver.maximize_window()
 ```
 
+## manipulacao api adobe
+```python
+from rpa_coop import adobe
+
+res = adobe.alterar_status_usuario('usuario_xyz@dominio.com.br', 'INACTIVE')
+print(res.text)
+print(res.status_code)
+        
+```
+
+
 ## manipulacao de emails:
 ```python
 from rpa_coop import mail
 
 mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', 'msg aqui')
 
 lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']
```

### Comparing `rpa_cooperativa-1.0.53/README.md` & `rpa_cooperativa-1.0.54/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,25 @@
 
 time.sleep(1)
 driver.get(url)
 time.sleep(1)
 driver.maximize_window()
 ```
 
+## manipulacao api adobe
+```python
+from rpa_coop import adobe
+
+res = adobe.alterar_status_usuario('usuario_xyz@dominio.com.br', 'INACTIVE')
+print(res.text)
+print(res.status_code)
+        
+```
+
+
 ## manipulacao de emails:
 ```python
 from rpa_coop import mail
 
 mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', 'msg aqui')
 
 lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']
```

### Comparing `rpa_cooperativa-1.0.53/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.54/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.53/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.54/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.53/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.54/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.53/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.54/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.53/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.54/rpa_coop/rpa_coop.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,44 @@
         credenciais = credencial_atributos[0]
         valor = credenciais.get(select_atributo)
         result = f'{select_atributo} : {valor}'
         if print_atributo: print(result)
         if retorna_atributo: return valor
         return credenciais
 
+
+class Adobe:
+    def __init__(self):
+        self.token_api_adobe = str(gerador_pwd('api_adobe', 'senha'))
+        self.url_api_adobe = str(gerador_pwd('api_adobe', 'ip_host'))
+        
+        
+    def alterar_status_usuario(self, email_usuario:str, status_usuario:str):
+        '''status_usuario: ACTIVE, INACTIVE'''
+        token_get_user = self.token_api_adobe
+        url = f'{self.url_api_adobe}users'
+        headers = { "Authorization": f"{token_get_user}"}
+        response = requests.get(url, headers=headers)
+        df = pd.DataFrame(response.json()['userInfoList'])
+        for x in df.itertuples():
+            if str(x.email) == str(email_usuario):
+                id_usuario = str(x.id)
+                break
+            else:
+                id_usuario = 'Não encontrado'
+
+        if id_usuario == 'Não encontrado': raise Exception('Usuário não encontrado')
+        url = f'{self.url_api_adobe}users/{id_usuario}/state'
+        headers = { "Authorization": f"{token_get_user}"}
+        body = {"state": f"{status_usuario}", "comment": "desativado por rpa"}
+        response = requests.put(url, headers=headers, json=body)
+        return response
+        
+        
+        
   
 class Dados:
     
 
     def __init__(self):
         self.ip_planning = str(os.getenv('ip_planning'))
         self.user_planning = str(os.getenv('user_planning'))
@@ -1083,14 +1113,31 @@
         else:
             if isinstance(destinatarios, list): todos_destinos.extend(destinatarios)
             if isinstance(destinatarios, str): todos_destinos.append(destinatarios)
             smtpserver.send_message (msg, from_addr=self.user_mail, to_addrs=todos_destinos)
             
         smtpserver.close()
         
+        
+        
+    # def ler_email(self):
+    #     from imap_tools import MailBox
+    #     serv_imap = self.smtpsrv.replace('smtp', 'imap')
+        
+    #     # get list of email bodies from INBOX folder
+    #     with MailBox(serv_imap).login(self.user_mail, self.password_mail, 'INBOX') as mailbox:
+    #         for msg in mailbox.fetch():
+    #             msg_de = str(msg.from_)
+    #             if 'edenilson' in msg_de:
+    #                 # print(msg.subject)
+    #                 # print(msg.text)
+    #                 return msg.text
+            
+        
+        
                        
 class Acc:
     import pyautogui as p
     import subprocess
     import pyperclip
     
     
@@ -1793,14 +1840,15 @@
             
         return dia_util_proximo
         
         
         
         
 
-    
+# mail = Emails()
+# mail.ler_email()
```

### Comparing `rpa_cooperativa-1.0.53/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.53
+Version: 1.0.54
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
@@ -74,14 +74,25 @@
 
 time.sleep(1)
 driver.get(url)
 time.sleep(1)
 driver.maximize_window()
 ```
 
+## manipulacao api adobe
+```python
+from rpa_coop import adobe
+
+res = adobe.alterar_status_usuario('usuario_xyz@dominio.com.br', 'INACTIVE')
+print(res.text)
+print(res.status_code)
+        
+```
+
+
 ## manipulacao de emails:
 ```python
 from rpa_coop import mail
 
 mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', 'msg aqui')
 
 lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']
```

### Comparing `rpa_cooperativa-1.0.53/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.53/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.53/setup.py` & `rpa_cooperativa-1.0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.53",
+    version="1.0.54",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

