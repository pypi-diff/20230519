# Comparing `tmp/inhandtest-0.0.46.tar.gz` & `tmp/inhandtest-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.46.tar", last modified: Tue May 16 09:07:53 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.47.tar", last modified: Fri May 19 01:02:56 2023, max compression
```

## Comparing `inhandtest-0.0.46.tar` & `inhandtest-0.0.47.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 09:07:53.000000 inhandtest-0.0.46/
--rw-rw-rw-   0        0        0      535 2023-05-16 09:07:53.000000 inhandtest-0.0.46/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.46/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 09:07:53.000000 inhandtest-0.0.46/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.46/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:07:53.000000 inhandtest-0.0.46/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.46/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    39712 2023-05-16 03:23:36.000000 inhandtest-0.0.46/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27870 2023-05-10 08:56:15.000000 inhandtest-0.0.46/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.46/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    49636 2023-05-16 05:53:35.000000 inhandtest-0.0.46/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    10957 2023-05-09 09:49:30.000000 inhandtest-0.0.46/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.46/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.46/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.46/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.46/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.46/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    51883 2023-05-16 09:03:39.000000 inhandtest-0.0.46/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.46/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.46/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6076 2023-05-15 10:19:14.000000 inhandtest-0.0.46/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.46/inhandtest/ip.py
--rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.46/inhandtest/mail.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.46/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32728 2023-05-06 01:14:17.000000 inhandtest-0.0.46/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    25281 2023-05-12 08:18:46.000000 inhandtest-0.0.46/inhandtest/tools.py
--rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.46/requirements.txt
--rw-rw-rw-   0        0        0     1450 2023-05-16 09:07:33.000000 inhandtest-0.0.46/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 01:02:56.000000 inhandtest-0.0.47/
+-rw-rw-rw-   0        0        0      535 2023-05-19 01:02:56.000000 inhandtest-0.0.47/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.47/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 01:02:56.000000 inhandtest-0.0.47/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.47/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 01:02:56.000000 inhandtest-0.0.47/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.47/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    39712 2023-05-16 03:23:36.000000 inhandtest-0.0.47/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.47/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.47/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    52406 2023-05-18 09:41:02.000000 inhandtest-0.0.47/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    15461 2023-05-17 09:10:24.000000 inhandtest-0.0.47/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.47/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.47/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.47/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.47/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.47/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    51883 2023-05-16 09:03:39.000000 inhandtest-0.0.47/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7583 2023-05-06 07:36:44.000000 inhandtest-0.0.47/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.47/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6847 2023-05-18 06:06:23.000000 inhandtest-0.0.47/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.47/inhandtest/ip.py
+-rw-rw-rw-   0        0        0    11620 2023-05-08 10:30:07.000000 inhandtest-0.0.47/inhandtest/mail.py
+drwxrwxrwx   0        0        0        0 2023-05-19 01:02:56.000000 inhandtest-0.0.47/inhandtest/pages/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.47/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 01:02:56.000000 inhandtest-0.0.47/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:38:25.000000 inhandtest-0.0.47/inhandtest/pages/ingateway/__init__.py
+-rw-rw-rw-   0        0        0     5307 2023-05-18 09:51:01.000000 inhandtest-0.0.47/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0      593 2023-05-18 07:02:23.000000 inhandtest-0.0.47/inhandtest/pages/ingateway/locators.py
+-rw-rw-rw-   0        0        0      303 2023-05-15 09:37:04.000000 inhandtest-0.0.47/inhandtest/pages/locale.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.47/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    32773 2023-05-16 10:13:54.000000 inhandtest-0.0.47/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    25281 2023-05-12 08:18:46.000000 inhandtest-0.0.47/inhandtest/tools.py
+-rw-rw-rw-   0        0        0      137 2023-05-15 07:42:26.000000 inhandtest-0.0.47/requirements.txt
+-rw-rw-rw-   0        0        0     1544 2023-05-19 01:02:26.000000 inhandtest-0.0.47/setup.py
```

### Comparing `inhandtest-0.0.46/README.md` & `inhandtest-0.0.47/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.47/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.47/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         return {
             'system': {
                 'default': 'basic_setup',
                 'menu': [self.system_menu],
                 'basic_setup': {
                     'mouse_move': (300, 0),
                     'menu': self.page.locator('#setup_system'),
-                    # 'visible_locator': [self.frame.locator('#_language')],
+                    'visible_locator': [self.frame.locator('#_language')],
                     'wait_locator': [self.frame.locator('#_language')]},
                 'time': {
                     'mouse_move': (300, 0),
                     'menu': self.page.locator('#setup_time'),
                     'visible_locator': [self.frame.locator('#_tm_sel')],
                     'wait_locator': [self.frame.locator('#_tm_sel')]},
                 'serial_port': {   # 只有615 有该菜单
```

### Comparing `inhandtest-0.0.46/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.47/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/base_page/base_page.py` & `inhandtest-0.0.47/inhandtest/base_page/base_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from inhandtest.base_page._ig_contents_locators import IGContentsLocators
 from typing import List
 from inhandtest.exception import ModelError
 from inhandtest.tools import loop_inspector
 from playwright.sync_api import Page, Locator, expect, TimeoutError, sync_playwright
 from inhandtest.base_page._vg710_contents_locators import VGContentsLocators
 from inhandtest.base_page._ir3XX_contents_locators import Ir3XXContentsLocators
-from inhandtest.base_page.table_tr import Table
+from inhandtest.base_page.table_tr import Table, IgTable
 import allure
 import logging
 import re
 
 
 class BasePage:
 
@@ -40,16 +40,16 @@
                       locale: dict 国际化
         """
         self.page = page
         self.host = host
         self.model = model.upper()
         self.protocol = protocol
         self.port = port
-        self.__username = username
-        self.__password = password
+        self.username = username
+        self.password = password
         self.language = language
         self.__browser_type = kwargs.get('browser')
         self.__http_credentials_model = ('VG710',)  # 需要使用http认证的设备, 没有登录页面 只有登录弹窗
         if self.page is None:
             self.__new_page()
         if self.model == 'VG710':
             self.content_locator = VGContentsLocators(self.page, language).tags_menu
@@ -96,15 +96,15 @@
             browser = self.__playwright.firefox
         elif self.__browser_type == 'webkit':
             browser = self.__playwright.webkit
         else:
             browser = self.__playwright.chromium
         self.__browser = browser.launch(headless=False)
         if self.model in self.__http_credentials_model:
-            http_credentials = {'username': self.__username, 'password': self.__password}
+            http_credentials = {'username': self.username, 'password': self.password}
         else:
             http_credentials = None
         self.__context = self.__browser.new_context(ignore_https_errors=True, http_credentials=http_credentials)
         logging.info('Start your journey browser is chrome')
         self.page = self.__context.new_page()
         self.page.on("dialog", dialog_)
 
@@ -113,16 +113,16 @@
         """
 
         :param username:  如果不传使用默认的用户名
         :param password:  如果不传使用默认的密码
         :param status: 登录状态 'success'|'fail' 期望登录的状态是成功还是失败，失败了就会停留在登录页面，不做任何操作
         :return:
         """
-        username = self.__username if not username else username
-        password = self.__password if not password else password
+        username = self.username if not username else username
+        password = self.password if not password else password
 
         def goto_router():
             device = "{}://{}:{}".format(self.protocol, self.host, self.port)
             try:
                 self.page.goto(device, timeout=120 * 1000)
             except Exception:
                 raise
@@ -163,29 +163,29 @@
                     logging.info(f"Device %s refresh page {i + 1} times" % self.host)
                     self.page.reload()
                 except TimeoutError:
                     pass
         else:
             raise Exception(f'Device {self.host} page error')
 
-    @allure.step('页面抓取接口{url}返回结果')
+    @allure.step('页面抓取接口返回结果')
     def wait_for_response(self, url: str, timeout=30) -> dict:
         """
 
         :param url:  pattern 匹配的正则表达式,
         :param timeout: 默认30秒
         :return: 返回结果
         """
         with self.page.expect_response(lambda response: re.search(url, response.url) and response.status == 200,
                                        timeout=timeout * 1000) as response_info:
             logging.info("Device %s fetch url %s " % (self.host, response_info.value.url))
         logging.info("Device %s the api response is  %s " % (self.host, response_info.value.json()))
         return response_info.value.json()
 
-    @allure.step('进入菜单{menu}')
+    @allure.step('进入菜单')
     def access_menu(self, menu: str, wait_time=None) -> None:
         """进入菜单，多个菜单使用点号隔开，不限多少层级   menu_locator 存放在 base_locators 里面，
             定义menu = {'system': {'locator': '#menu_id', 'wait_locator': '#wait_locator_id'},
                                'status':{'locator': '#status_id', 'wait_locator': '#wait_locator_id'}}
             定义菜单时所有菜单的点号都需要省略，如2.4g 写成24g；空格写成下划线，如wi-fi 2.4g 写成wi-fi_24g
             中划线写成下划线，如wi-fi-2.4g 写成wi_fi_24g
 
@@ -271,15 +271,15 @@
                 menu = default_change(menu, self.content_locator).split('.')
                 access(menu)
             except Exception:
                 raise f'not support this menu {menu}'
             if wait_time:
                 self.page.wait_for_timeout(wait_time)
 
-    @allure.step('{log_desc} 输入{value}')
+    @allure.step('输入信息')
     def fill(self, locator: Locator, value: str or int, log_desc=None, force=False) -> None:
         """ 封装公共的输入操作
 
         :param locator:  元素定位
 
         :param value: 输入的值
         :param log_desc: 功能描述，用英文 如 Static Routing Destination
@@ -289,15 +289,15 @@
         if value is not None:
             locator.clear()
             locator.fill(str(value), force=force)
             locator.blur()  # 鼠标移出输入框
             if log_desc:
                 logging.info(f'Device {self.host} fill {log_desc} {value}')
 
-    @allure.step('点击 {log_desc}')
+    @allure.step('点击按钮')
     def click(self, locator: Locator, log_desc=None, dialog_message: str = None, tip_messages: str or list = None,
               wait_for_time: int = None, tip_messages_timeout=30) -> None:
         """ 封装公共的点击操作
 
         :param locator:  元素定位
         :param log_desc: 功能描述，用英文 如 Static Routing Destination
         :param dialog_message: str  点击按钮后有dialog弹出，并且期望对信息做验证， 支持模糊匹配
@@ -316,15 +316,15 @@
                 locator.click()
             if log_desc:
                 logging.info(f'Device {self.host} click {log_desc}')
             self.tip_messages(tip_messages, tip_messages_timeout)
             if wait_for_time:
                 self.page.wait_for_timeout(wait_for_time)
 
-    @allure.step('{log_desc} {action}')
+    @allure.step('勾选框')
     def check(self, locator: Locator, action='check', log_desc=None, tip_messages: str or list = None) -> None:
         """ 封装公共的单选操作
         :param locator:  元素定位
         :param log_desc: 功能描述，用英文 如 Static Routing Destination
         :param action: 'check'|'uncheck'| None | '是' | 'Yes'
         :param tip_messages: str or list 点击后等待该tip出现 再等待tip消失，如果有多个，使用列表传入
                             tip_messages 是支持模糊匹配
@@ -396,34 +396,33 @@
                     option_p = self.page.locator(f'//div[@id="{locator.get_attribute("aria-controls")}"]').locator(
                         '..').locator('//div[@class="rc-virtual-list-holder-inner"]')
                     option = option_p.locator(f'//div[@title="{value}"]')
                     all_option = option_p.locator('.ant-select-item.ant-select-item-option')
                 else:  # IG902 设备的下拉选择
                     now_option = locator.locator(
                         '//div/div/div[@class="ant-select-selection-selected-value"]').inner_text()
-                    option_p = self.page.locator(
-                        f'//div[@id="{locator.locator(".ant-select-selection").get_attribute("aria-controls")}"]').locator(
-                        '//ul[@role="listbox"]')
-                    option = option_p.get_by_text(re.compile(value, re.IGNORECASE))
-                    all_option = option_p.locator('//li')
+                    option_id = locator.locator(".ant-select-selection").get_attribute("aria-controls")
+                    all_option = self.page.locator(f'//div[@id="{option_id}"]').locator('//ul[@role="listbox"]/li')
+                    option = self.page.locator(f'//div[@id="{option_id}"]').locator('//ul[@role="listbox"]/li',
+                                                                                    has_text=value)
                 if now_option != value:
                     locator.scroll_into_view_if_needed()
                     if not locator.is_editable():
                         locator.click(force=True)
                     else:
                         locator.click()
                     scroll_into_view_action(all_option, option)
             else:  # IR300 等设备的下拉选择
                 locator.select_option(str(value))  # value 可以为label 或者value
                 if locator.locator(f'//option[@value="{value}"]').count() == 1:
                     value = locator.locator(f'//option[@value="{value}"]').inner_text()
             if log_desc:
                 logging.info(f"Device {self.host} select {log_desc} of {value}")
 
-    @allure.step('{log_desc} {action}')
+    @allure.step('切换按钮')
     def switch_button(self, locator: Locator, action: str = 'enable', log_desc=None) -> None:
         """控制通用开关按钮开关， 如拨号的开关
 
         :param locator:  开关按钮元素
         :param action: enable, disable, None 可以开启或关闭，但是并没有提交，只是点击了下
         :param log_desc:  开关功能描述
         :return: None
@@ -439,14 +438,34 @@
                 if locator.get_attribute('aria-checked') == 'false' or not locator.get_attribute('aria-checked'):
                     pass
                 else:
                     locator.click(force=True)
                     if log_desc:
                         logging.info(f"Device {self.host} {log_desc} disabled")
 
+    @allure.step('点选框操作')
+    def radio_select(self, locator: Locator, value: str, log_desc=None) -> None:
+        """ 当前只有IG和ER的设备有单选框
+
+        :param locator: 在所有label元素的上级div定位
+        :param value: 选项的值，注意国际化
+        :param log_desc: 选项的描述
+        :return:
+        """
+        if value:
+            locator.wait_for(state='visible')
+            locator_label = locator.locator(f'//label[text()="{value}"]')
+            if locator_label.count() == 1:
+                if 'ant-radio-wrapper-checked' not in locator_label.get_attribute('class'):
+                    locator.click(force=True)
+                    if log_desc:
+                        logging.info(f"Device {self.host} {log_desc} radio select {value}")
+            else:
+                raise Exception(f'found {value} option {locator_label.count()} elements')
+
     @allure.step('伸缩按钮')
     def expand(self, left_text: str, action: str = 'expand') -> None:
         """ 伸缩按钮
 
         :param left_text: 伸缩按钮 左边的文本，需要注意国际化
         :param action: expand|close|None
         :return:
@@ -528,18 +547,18 @@
         """对话框提示进行校验， 使用时需要在base_locator 里面定义dialog_massage 且返回字典数据
 
         :param f:  是一个操作函数，执行后会有dialog弹窗出现
         :param message: 校验的信息, 支持模糊匹配
         :return:
         """
         if message:
+            message = self.locale.get(message) if self.locale.get(message) else message
             with self.page.expect_event('dialog') as dialog_info:
                 f()
-            assert self.locale.get(message) in dialog_info.value.message, \
-                f'{self.host} assert {message} dialog error'
+            assert message in dialog_info.value.message, f'{self.host} assert {message} dialog error'
 
     @allure.step("校验tip messages")
     def tip_messages(self, messages: str or list = None, timeout=30) -> None:
         """ 某些提交操作会出现文本的提示，提示在过几秒钟后会消失，对于该类消息的验证使用该方法，
             使用时需要在base_locator tip_messages 且返回字典数据
 
         :param messages: str or list 点击后等待该tip出现 再等待tip消失，如果有多个，使用列表传入
@@ -547,42 +566,42 @@
                             该项校验 页面元素必须停留时间1秒及更多时间，否则不容易检测到导致报错
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
             tip_messages = [messages] if isinstance(messages, str) else messages
             for message in tip_messages:
-                message = self.locale.get(message)  # 国际化转换
+                message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
                 expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_visible(timeout=timeout * 1000)
                 expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_hidden(timeout=timeout * 1000)
 
     @allure.step("校验text messages")
     def text_messages(self, messages: str or list = None, timeout=10) -> None:
         """ 对文本内容做验证，如在输入框输入错误内容时出现的文本，该类文本会一直存在
         :param messages: str or list 文本内容，如果有多个，使用列表传入
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
             text_messages = [messages] if isinstance(messages, str) else messages
             for message in text_messages:
-                message = self.locale.get(message)  # 国际化转换
+                message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
                 expect(self.page.get_by_text(re.compile(message, re.IGNORECASE))).to_be_visible(timeout=timeout * 1000)
 
     @allure.step("校验元素Title")
     def title_messages(self, messages: str or list = None, timeout=10) -> None:
         """ 对元素的属性title做内容验证，
         :param messages: str or list 文本内容，如果有多个，使用列表传入
         :param timeout: 校验超时时间
         :return:
         """
         if messages:
             text_messages = [messages] if isinstance(messages, str) else messages
             for message in text_messages:
-                message = self.locale.get(message)  # 国际化转换
+                message = self.locale.get(message) if self.locale.get(message) else message  # 国际化转换
                 expect(self.page.get_by_title(re.compile(message, re.IGNORECASE))).to_be_visible(timeout=timeout * 1000)
 
     @allure.step('设置页面翻页')
     def page_refresh(self, refresh_time: str, select_locator: Locator) -> None:
         """
         :param refresh_time: str
                         '0'|'3'|'4'|'5'|'10'|'15'|'30'|'60'|'120'|'180'|'240'|'300'|'600'|'900'|'1200'|'1800'
@@ -597,68 +616,94 @@
             else:
                 if select_locator.is_disabled():
                     self.click(select_locator.locator('..').locator('#refresh-button'), 'refresh button')
                     self.page.wait_for_timeout(500)
                 self.select_option(select_locator, refresh_time, 'refresh time select')
                 self.click(select_locator.locator('..').locator('#refresh-button'), 'refresh button ok')
 
-    @staticmethod
     @allure.step("Table tr action")
-    def table_tr(locators: dict, value: list, log_desc=None) -> List[int or None] or None:
+    def table_tr(self, locators: dict, value: list, log_desc=None) -> List[int or None] or None:
         """
 
         :param locators: {"locator": $locator2, "param": {$key2: $value2}, "columns": list, 'unique_columns': list}
         :param value: [($action,{**kwarg})] ex: [('delete_all', )],  [('edit', $old, $new)]多个操作时使用列表 [('add',{}), ('add',{})]
         :param log_desc: 日志描述
         :return:
         """
-        tr = Table(locators.get('columns'), locators.get('locator'),
-                   locators.get('unique_columns'), locators.get('param'), log_desc)
-        exist_tr = []
-        if value:
-            for value_ in value:
-                if value_[0] == 'add':
-                    tr.add(**value[1])
-                elif value_[0] == 'delete_all':
-                    tr.delete_all()
-                elif value_[0] == 'delete':
-                    tr.delete(**value[1])
-                elif value_[0] == 'exist':
-                    exist_tr.append(tr.exist(**value[1]))
-                elif value_[0] == 'edit':
-                    tr.edit(value[1], value[2])
-            return exist_tr
+        if self.model in ('IG902', 'IG502'):
+            tr = IgTable(locators.get('columns'), locators.get('locator'), locators.get('param'), log_desc)
+            exist_tr = []
+            if value:
+                for value_ in value:
+                    if value_[0] == 'add':
+                        tr.add(self.agg_in, **value_[1])
+                    elif value_[0] == 'delete_all':
+                        tr.delete_all()
+                    elif value_[0] == 'delete':
+                        tr.delete(value_[1])
+                    elif value_[0] == 'exist':
+                        exist_tr.append(tr.exist(value_[1], self.locale))
+                    elif value_[0] == 'edit':
+                        tr.edit(self.agg_in, value_[1], **value_[2])
+                return exist_tr
+        else:
+            tr = Table(locators.get('columns'), locators.get('locator'),
+                       locators.get('unique_columns'), locators.get('param'), log_desc)
+            exist_tr = []
+            if value:
+                for value_ in value:
+                    if value_[0] == 'add':
+                        tr.add(**value[1])
+                    elif value_[0] == 'delete_all':
+                        tr.delete_all()
+                    elif value_[0] == 'delete':
+                        tr.delete(**value[1])
+                    elif value_[0] == 'exist':
+                        exist_tr.append(tr.exist(**value[1]))
+                    elif value_[0] == 'edit':
+                        tr.edit(value[1], value[2])
+                return exist_tr
 
     def agg_in(self, locators: list, action_dict: dict) -> None:
         """封装公共的整合输入操作
                 :param locators:  列表 嵌套 长度为2的元组，元组的第一项为操作项名称， 第二项为对应的一个字典
                     [($param1, {"locator": $locator1, "type": $type1, "relation": [($param2, $value2)], "param": {$key1: $value1}}),
                     ($param2, {"locator": $locator2, "type": $type2, "relation": [($param3, $value3),……], "param": {$key2: $value2}}),
                     ($param3, {"locator": $locator2, "type": 'table_tr', "relation": [($param3, $value3),……], "param": {$key2: $value2},
                                 "columns": list, 'unique_columns': list}),]
                     $param: 操作项的名称，如 'language'|'sim'|'status'
                     $locator: 操作项的元素定位， locator or [locator,locator,...]
-                    $type: 操作项的类型 fill|select|button|check|upload_file|download_file|text_visible|error_tips|locators_title|
-                                     multi_select|multi_check|multi_fill|table_tr,
+                    $type: 操作项的类型 text|select|button|check|upload_file|download_file|tip_messages|text_messages|title_messages|
+                                     multi_select|multi_check|multi_fill|table_tr|switch_button|radio|expand|
                             select value值可以是label|Value
                             multi_select指一个参数有多个select, 对应操作项的多个locator及value用[]传入
                     "relation":[($param, $value)]: 操作项的关联项，若有多个则首个为最先操作的关联项，其中$param为关联项的名称，$value为关联项的预期值
                     "param":{$key, $value}: 参数转换，如大小写转换{"ab":"AB"} {"wan":"Wan"}等.
                 :param action_dict: 要做操作的参数名称与对应的值{$param1: $value1, $param2: $value2}
                 :return:
                 """
         relations = []
 
         def operation(param, param_locator, value):
+            if param_locator.get('wait_for'):
+                self.page.wait_for_timeout(param_locator.get('wait_for'))
             if param_locator.get('type') == 'text':
                 self.fill(param_locator.get('locator'), value, param)
             elif param_locator.get('type') == 'select':
                 if param_locator.get('param') and value in param_locator.get('param').keys():
                     value = param_locator.get('param').get(value)
                 self.select_option(param_locator.get('locator'), value, param)
+            elif param_locator.get('type') == 'radio':
+                if param_locator.get('param') and value in param_locator.get('param').keys():
+                    value = param_locator.get('param').get(value)
+                self.radio_select(param_locator.get('locator'), value, param)
+            elif param_locator.get('type') == 'switch_button':
+                self.switch_button(param_locator.get('locator'), value, param)
+            elif param_locator.get('type') == 'expand':
+                self.expand(param_locator.get('locator'), value)  # 此处获取到的locator 是一个str
             elif param_locator.get('type') == 'button':
                 if value:
                     dialog_message, tip_messages, wait_for_time, tip_messages_timeout = None, None, None, 30
                     if isinstance(value, dict):
                         dialog_message = value.get('dialog_message')
                         tip_messages = value.get('tip_messages')
                         wait_for_time = value.get('wait_for_time')
@@ -671,15 +716,15 @@
                     value_, tip_messages = value, None
                     if isinstance(value, dict):
                         value_ = value.get('value')
                         tip_messages = value.get('tip_messages')
                     self.check(param_locator.get('locator'), value_, param, tip_messages)
             elif param_locator.get('type') == 'table_tr':
                 if isinstance(value, list):  # value按照table_tr()的传参方式传参,
-                    self.table_tr(param_locator, value, param)
+                    self.table_tr(param_locator.get('locator'), value, param)
                 else:
                     logging.error(f'value {value} should be a list, not {type(value)}')
             elif param_locator.get('type').startswith('multi_'):
                 if len(param_locator.get('locator')) == len(value):
                     for locator_, value_ in dict(zip(param_locator.get('locator'), value)):
                         if 'select' in param_locator.get('type'):
                             if param_locator.get('param') and value_ in param_locator.get('param').keys():
```

### Comparing `inhandtest-0.0.46/inhandtest/exception.py` & `inhandtest-0.0.47/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/file.py` & `inhandtest-0.0.47/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/inmodbus.py` & `inhandtest-0.0.47/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/inmongodb.py` & `inhandtest-0.0.47/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/inmqtt.py` & `inhandtest-0.0.47/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/inrequest.py` & `inhandtest-0.0.47/inhandtest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/inserial.py` & `inhandtest-0.0.47/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/insocket.py` & `inhandtest-0.0.47/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/inssh.py` & `inhandtest-0.0.47/inhandtest/inssh.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 # @Time    : 2023/3/8 13:26:52
 # @Author  : Pane Li
 # @File    : inssh.py
 """
 inssh
 
 """
+import functools
 import logging
 import os.path
 
 import paramiko
 from paramiko.ssh_exception import *
 
 
 class InSsh:
-    def __init__(self, host: str, username: str, password: str, port=22):
+    def __init__(self, host: str, username: str, password: str, port=22, sftp=True):
         """
 
         :param host: ssh 连接主机地址
         :param username: ssh 连接主机用户名
         :param password: ssh 连接主机密码
         :param port: 端口， 默认22
+        :param sftp: 是否开启sftp 服务
         """
         self.__host = host
         self.__username = username
         self.__password = password
         self.__port = port
         self.ssh = paramiko.SSHClient()
         self.ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
@@ -33,62 +35,79 @@
             logging.info(f"ssh connect {self.__host} by {self.__username}:{self.__password}")
             self.ssh.connect(self.__host, self.__port, self.__username, self.__password, timeout=5)
         except AuthenticationException:
             raise AuthenticationException(f"ssh connect {self.__host} Username or Password error")
         except Exception:
             raise ConnectionError(f"ssh connect {self.__host} connect error")
         self.transport.connect(username=username, password=password)
-        self.sftp = paramiko.SFTPClient.from_transport(self.transport)
+        if sftp:
+            self.sftp = paramiko.SFTPClient.from_transport(self.transport)
+        else:
+            self.sftp = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
+    def enable_sftp(func):
+        @functools.wraps(func)
+        def wrapper(self, *args, **kwargs):
+            if self.sftp is None:
+                raise Exception("please set sftp=True when init InSsh")
+            result = func(self, *args, **kwargs)
+            return result
+
+        return wrapper
+
     def exec_command(self, command: str) -> str:
         """执行命令并返回结果
 
         :param command: 执行命令, 多条时使用分号隔开
         :return: 返回所有命令执行后的结果
         """
         result = None
         if command:
             stdin, stdout, stderr = self.ssh.exec_command(command)
             logging.info(f'exec command 【{command}】')
             result = stdout.read().decode("utf-8")
             logging.info(f'command result 【{result}】')
         return result
 
+    @enable_sftp
     def download_file(self, remote_file, local_file) -> None:
         """
         从服务器上下载文件
         :param remote_file: 远端文件路径
         :param local_file: 本地文件路径
         :return:
         """
+
         try:
             self.sftp.get(remote_file, local_file)
             logging.info(f'{remote_file} download success')
         except Exception as e:
             logging.error(f'{remote_file} download failed, {e}')
 
+    @enable_sftp
     def upload_file(self, remote_file, local_file) -> None:
         """
         文件上传
         :param remote_file: 远端文件路径
         :param local_file: 本地文件路径
         :return:
         """
         try:
             self.sftp.put(local_file, remote_file)
             logging.info(f'{local_file} upload success')
         except Exception as e:
             logging.error(f'{remote_file} upload failed, {e}')
 
+    @enable_sftp
     def clear_dir_or_remove_file(self, dir_name_or_file_path: str) -> None:
         """ 清除远端目录下所有文件，或单个文件
 
         :param dir_name_or_file_path: 目录或者文件路径
         :return:
         """
 
@@ -101,66 +120,72 @@
 
         if os.path.isdir(dir_name_or_file_path):
             files = self.sftp.listdir(dir_name_or_file_path)
             [remove_file(os.path.join(dir_name_or_file_path, i)) for i in files]
         else:
             remove_file(dir_name_or_file_path)
 
+    @enable_sftp
     def get_file_content(self, file_path: str) -> str:
         """获取文件内容
 
         :param file_path:  文件路径  ex： 'D:\ecoer\sdf.sh'
         :return:
         """
         self.sftp.chdir(os.path.dirname(file_path))
         logging.info(f'read {file_path} content success')
         return self.sftp.file(os.path.basename(file_path), 'r').read().decode(encoding='utf-8')
 
+    @enable_sftp
     def write_file_content(self, file_path: str, content: str, mode='w') -> None:
         """像文件写入数据
 
         :param file_path: 文件全路径 ex: 'D:\ecoer\sdf.sh'
         :param content: 写入的文件内容，多行内容使用\n 连接
         :param mode: 'w' 替换文件内容写入， 'a' 追加内容
         :return:
         """
         self.sftp.chdir(os.path.dirname(file_path))
         with self.sftp.open(os.path.basename(file_path), mode) as f:
             f.write(content)
         logging.info(f'write {file_path} content success')
 
+    @enable_sftp
     def chmod(self, file_path: str, mode) -> None:
         """更改文件权限
 
         :param file_path:
         :param mode:
         :return:
         """
         self.sftp.chmod(file_path, mode)
         logging.info(f'chmod {file_path} success')
 
+    @enable_sftp
     def mkdir(self, path, mode=511) -> None:
         """创建文件夹
 
         :param path: 路径
         :param mode:  511 即 o777 权限，最大的
         :return:
         """
         self.sftp.mkdir(path, mode)
         logging.info(f'mkdir {path} success')
 
+    @enable_sftp
     def rmdir(self, path) -> None:
         """删除文件夹
 
         :param path: 路径
         :return:
         """
         self.sftp.rmdir(path)
         logging.info(f'remove {path} success')
 
+    @enable_sftp
     def rename(self, old_path, new_path) -> None:
         """文件重命名
 
         :param old_path:
         :param new_path:
         :return:
         """
@@ -169,15 +194,17 @@
 
     def close(self) -> None:
         """断开连接
 
         :return:
         """
         self.ssh.close()
-        self.sftp.close()
+        if self.sftp:
+            self.sftp.close()
         self.transport.close()
 
 
 if __name__ == '__main__':
     import sys
 
     logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO, stream=sys.stdout)
+    InSsh('10.5.17.45', 'inhand', '64391099@inhand', sftp=False).download_file('/home/inhand/1.txt', 'D:\ecoer\1.txt')
```

### Comparing `inhandtest-0.0.46/inhandtest/ip.py` & `inhandtest-0.0.47/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/mail.py` & `inhandtest-0.0.47/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/pytest_email.html` & `inhandtest-0.0.47/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/inhandtest/telnet.py` & `inhandtest-0.0.47/inhandtest/telnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         try:
             # 连接telnet服务器
             logging.info("Start telnet 【%s:%s】" % (self.host, self.port))
             self.tn = telnetlib.Telnet(self.host, self.port, timeout=10)
         except:
             raise ConnectionError(f'Device【{self.host}:{self.port} connect failed】')
         logging.info("Telnet 【%s:%s】 connected" % (self.host, self.port))
+        self.tn.write("\n".encode("cp936"))
         logging.info(self.tn.read_until('login:'.encode("cp936")).decode("cp936").strip())
         # 登录路由器
         self.tn.write("{}\n".format(self.user).encode("cp936"))
         logging.info(self.tn.read_until('Password:'.encode("cp936")).decode("cp936").strip())
         self.tn.write("{}\n".format(self.password).encode("cp936"))
         login_result = self.tn.read_until(login_spe.get(self.model).encode("cp936"), timeout=20).decode("cp936").strip()
         logging.info(login_result)
```

### Comparing `inhandtest-0.0.46/inhandtest/tools.py` & `inhandtest-0.0.47/inhandtest/tools.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.46/setup.py` & `inhandtest-0.0.47/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 setup
 
 """
 from distutils.core import setup
 
 setup(
     name='inhandtest',
-    version='0.0.46',
+    version='0.0.47',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
-    packages=['inhandtest', 'inhandtest.base_page'],
-    package_data={'inhandtest': ['pytest_email.html']},
+    packages=['inhandtest', 'inhandtest.base_page', 'inhandtest.pages', 'inhandtest.pages.ingateway', ],
+    package_data={'inhandtest': ['pytest_email.html'], 'inhandtest.pages.ingateway': ['*.yaml']},
     url='https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》',
     long_description='方便inhand测试同事在自动化测试时，对通用协议或者常用工具及方法做封装，需要使用时即在线安装；\n映翰通出品，追尾必究！',
     classifiers=[
         "Programming Language :: Python :: 3.7",
     ],
     install_requires=['pytz', 'requests', 'playwright', 'pyserial', 'modbus-tk', 'paho-mqtt', 'urllib3', 'paramiko',
                       'emails', 'Jinja2', 'pymongo', 'psutil', 'lxml', 'dynaconf'
```

