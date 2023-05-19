# Comparing `tmp/FunPayAPI-1.0.7.tar.gz` & `tmp/FunPayAPI-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FunPayAPI-1.0.7.tar", last modified: Mon May 15 12:05:55 2023, max compression
+gzip compressed data, was "FunPayAPI-1.0.8.tar", last modified: Fri May 19 09:59:42 2023, max compression
```

## Comparing `FunPayAPI-1.0.7.tar` & `FunPayAPI-1.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 12:05:55.271564 FunPayAPI-1.0.7/
-drwxrwxrwx   0        0        0        0 2023-05-15 12:05:55.240563 FunPayAPI-1.0.7/FunPayAPI/
--rw-rw-rw-   0        0        0      162 2023-05-10 15:12:44.000000 FunPayAPI-1.0.7/FunPayAPI/__init__.py
--rw-rw-rw-   0        0        0    60938 2023-05-15 11:55:25.000000 FunPayAPI-1.0.7/FunPayAPI/account.py
-drwxrwxrwx   0        0        0        0 2023-05-15 12:05:55.265563 FunPayAPI-1.0.7/FunPayAPI/common/
--rw-rw-rw-   0        0        0        0 2023-05-12 17:46:25.000000 FunPayAPI-1.0.7/FunPayAPI/common/__init__.py
--rw-rw-rw-   0        0        0     4842 2023-05-14 16:49:23.000000 FunPayAPI-1.0.7/FunPayAPI/common/enums.py
--rw-rw-rw-   0        0        0     7842 2023-05-14 23:54:13.000000 FunPayAPI-1.0.7/FunPayAPI/common/exceptions.py
--rw-rw-rw-   0        0        0     8033 2023-04-14 18:22:19.000000 FunPayAPI-1.0.7/FunPayAPI/common/utils.py
--rw-rw-rw-   0        0        0    38383 2023-05-14 23:53:13.000000 FunPayAPI-1.0.7/FunPayAPI/types.py
-drwxrwxrwx   0        0        0        0 2023-05-15 12:05:55.270564 FunPayAPI-1.0.7/FunPayAPI/updater/
--rw-rw-rw-   0        0        0        0 2023-05-12 17:46:18.000000 FunPayAPI-1.0.7/FunPayAPI/updater/__init__.py
--rw-rw-rw-   0        0        0     8216 2023-05-11 19:12:41.000000 FunPayAPI-1.0.7/FunPayAPI/updater/events.py
--rw-rw-rw-   0        0        0    20435 2023-05-15 12:03:15.000000 FunPayAPI-1.0.7/FunPayAPI/updater/runner.py
-drwxrwxrwx   0        0        0        0 2023-05-15 12:05:55.254563 FunPayAPI-1.0.7/FunPayAPI.egg-info/
--rw-rw-rw-   0        0        0     3602 2023-05-15 12:05:55.000000 FunPayAPI-1.0.7/FunPayAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-15 12:05:55.000000 FunPayAPI-1.0.7/FunPayAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 12:05:55.000000 FunPayAPI-1.0.7/FunPayAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-15 12:05:55.000000 FunPayAPI-1.0.7/FunPayAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 12:05:55.000000 FunPayAPI-1.0.7/FunPayAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35801 2023-05-11 21:13:41.000000 FunPayAPI-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     3602 2023-05-15 12:05:55.271564 FunPayAPI-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3011 2023-05-12 11:49:15.000000 FunPayAPI-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 12:05:55.272563 FunPayAPI-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-05-15 12:05:39.000000 FunPayAPI-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:59:42.931732 FunPayAPI-1.0.8/
+drwxrwxrwx   0        0        0        0 2023-05-19 09:59:42.897732 FunPayAPI-1.0.8/FunPayAPI/
+-rw-rw-rw-   0        0        0      162 2023-05-15 12:08:20.000000 FunPayAPI-1.0.8/FunPayAPI/__init__.py
+-rw-rw-rw-   0        0        0    62476 2023-05-19 09:58:25.000000 FunPayAPI-1.0.8/FunPayAPI/account.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:59:42.924731 FunPayAPI-1.0.8/FunPayAPI/common/
+-rw-rw-rw-   0        0        0        0 2023-05-12 17:46:25.000000 FunPayAPI-1.0.8/FunPayAPI/common/__init__.py
+-rw-rw-rw-   0        0        0     4842 2023-05-14 16:49:23.000000 FunPayAPI-1.0.8/FunPayAPI/common/enums.py
+-rw-rw-rw-   0        0        0     7842 2023-05-14 23:54:13.000000 FunPayAPI-1.0.8/FunPayAPI/common/exceptions.py
+-rw-rw-rw-   0        0        0     8922 2023-05-19 09:07:17.000000 FunPayAPI-1.0.8/FunPayAPI/common/utils.py
+-rw-rw-rw-   0        0        0    38978 2023-05-19 09:36:22.000000 FunPayAPI-1.0.8/FunPayAPI/types.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:59:42.930731 FunPayAPI-1.0.8/FunPayAPI/updater/
+-rw-rw-rw-   0        0        0        0 2023-05-12 17:46:18.000000 FunPayAPI-1.0.8/FunPayAPI/updater/__init__.py
+-rw-rw-rw-   0        0        0     8216 2023-05-11 19:12:41.000000 FunPayAPI-1.0.8/FunPayAPI/updater/events.py
+-rw-rw-rw-   0        0        0    20435 2023-05-19 08:54:31.000000 FunPayAPI-1.0.8/FunPayAPI/updater/runner.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:59:42.914730 FunPayAPI-1.0.8/FunPayAPI.egg-info/
+-rw-rw-rw-   0        0        0     3602 2023-05-19 09:59:42.000000 FunPayAPI-1.0.8/FunPayAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-05-19 09:59:42.000000 FunPayAPI-1.0.8/FunPayAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 09:59:42.000000 FunPayAPI-1.0.8/FunPayAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-19 09:59:42.000000 FunPayAPI-1.0.8/FunPayAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-19 09:59:42.000000 FunPayAPI-1.0.8/FunPayAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35801 2023-05-11 21:13:41.000000 FunPayAPI-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3602 2023-05-19 09:59:42.931732 FunPayAPI-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3011 2023-05-12 11:49:15.000000 FunPayAPI-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-19 09:59:42.931732 FunPayAPI-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      928 2023-05-19 09:59:32.000000 FunPayAPI-1.0.8/setup.py
```

### Comparing `FunPayAPI-1.0.7/FunPayAPI/account.py` & `FunPayAPI-1.0.8/FunPayAPI/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Literal, Any, Optional, IO
 if TYPE_CHECKING:
     from .updater.runner import Runner
 
 from requests_toolbelt import MultipartEncoder
 from bs4 import BeautifulSoup
+from datetime import datetime, timedelta
 import requests
 import logging
 import random
 import string
 import json
 import time
 
@@ -862,15 +863,15 @@
         else:
             review = types.Review(stars, text, reply, False, str(reply_obj), order_id, buyer_username, buyer_id)
 
         order = types.Order(order_id, status, subcategory, short_description, full_description, sum_,
                             buyer_id, buyer_username, seller_id, seller_username, html_response, review)
         return order
 
-    def get_sales(self, start_from: str | None = None, include_paid: bool = True, include_closed: bool = True,
+    def get_sells(self, start_from: str | None = None, include_paid: bool = True, include_closed: bool = True,
                   include_refunded: bool = True, exclude_ids: list[str] | None = None,
                   id: Optional[int] = None, buyer: Optional[str] = None,
                   state: Optional[Literal["closed", "paid", "refunded"]] = None, game: Optional[int] = None,
                   section: Optional[str] = None, server: Optional[int] = None,
                   side: Optional[int] = None, **more_filters) -> tuple[str | None, list[types.OrderShortcut]]:
         """
         Получает и парсит список заказов со страницы https://funpay.com/orders/trade
@@ -922,14 +923,15 @@
         if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
 
         exclude_ids = exclude_ids or []
         filters = {"id": id, "buyer": buyer, "state": state, "game": game, "section": section, "server": server,
                    "side": side}
         filters = {name: filters[name] for name in filters if filters[name]}
+        filters.update(more_filters)
 
         link = "https://funpay.com/orders/trade?"
         for name in filters:
             link += f"{name}={filters[name]}&"
         link = link[:-1]
 
         if start_from:
@@ -972,17 +974,40 @@
 
             description = div.find("div", {"class": "order-desc"}).find("div").text
             price = float(div.find("div", {"class": "tc-price"}).text.split(" ")[0])
 
             buyer_div = div.find("div", {"class": "media-user-name"}).find("span")
             buyer_username = buyer_div.text
             buyer_id = int(buyer_div.get("data-href")[:-1].split("https://funpay.com/users/")[1])
+            subcategory_name = div.find("div", {"class": "text-muted"}).text
+
+            now = datetime.now()
+            order_date_text = div.find("div", {"class": "tc-date-time"}).text
+            if "сегодня" in order_date_text:  # сегодня, ЧЧ:ММ
+                h, m = order_date_text.split(", ")[1].split(":")
+                order_date = datetime(now.year, now.month, now.day, int(h), int(m))
+            elif "вчера" in order_date_text:  # вчера, ЧЧ:ММ
+                h, m = order_date_text.split(", ")[1].split(":")
+                temp = now - timedelta(days=1)
+                order_date = datetime(temp.year, temp.month, temp.day, int(h), int(m))
+            elif order_date_text.count(" ") == 2:  # ДД месяца, ЧЧ:ММ
+                split = order_date_text.split(", ")
+                day, month = split[0].split()
+                day, month = int(day), utils.MONTHS[month]
+                h, m = split[1].split(":")
+                order_date = datetime(now.year, month, day, int(h), int(m))
+            else:  # ДД месяца ГГГГ, ЧЧ:ММ
+                split = order_date_text.split(", ")
+                day, month, year = split[0].split()
+                day, month, year = int(day), utils.MONTHS[month], int(year)
+                h, m = split[1].split(":")
+                order_date = datetime(year, month, day, int(h), int(m))
 
             order_obj = types.OrderShortcut(order_id, description, price, buyer_username, buyer_id, order_status,
-                                            str(div))
+                                            order_date, subcategory_name, str(div))
             sells.append(order_obj)
 
         return next_order_id, sells
 
     def add_chats(self, chats: list[types.ChatShortcut]):
         """
         Сохраняет чаты.
```

### Comparing `FunPayAPI-1.0.7/FunPayAPI/common/enums.py` & `FunPayAPI-1.0.8/FunPayAPI/common/enums.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.7/FunPayAPI/common/exceptions.py` & `FunPayAPI-1.0.8/FunPayAPI/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.7/FunPayAPI/common/utils.py` & `FunPayAPI-1.0.8/FunPayAPI/common/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,30 @@
 """
 
 import string
 import random
 import re
 
 
+MONTHS = {
+    "января": 1,
+    "февраля": 2,
+    "марта": 3,
+    "апреля": 4,
+    "мая": 5,
+    "июня": 6,
+    "июля": 7,
+    "августа": 8,
+    "сентября": 9,
+    "октября": 10,
+    "ноября": 11,
+    "декабря": 12
+}
+
+
 def random_tag() -> str:
     """
     Генерирует случайный тег для запроса (для runner'а).
 
     :return: сгенерированный тег.
     """
     return "".join(random.choice(string.digits + string.ascii_lowercase) for _ in range(10))
@@ -130,14 +146,24 @@
         """
 
         self.ORDER_ID = re.compile(r"#[A-Z0-9]{8}")
         """
         Скомпилированное регулярное выражение, описывающее ID заказа.
         """
 
+        self.ORDER_DATE = re.compile(r"\d{1,2} [а-я]+, \d{1,2}:\d{1,2}")
+        """
+        Скомпилированное регулярное выражение, описывающее дату заказа в формате <ДД месяца, ЧЧ:ММ>.
+        """
+
+        self.FULL_ORDER_DATE = re.compile(r"\d{1,2} [а-я]+ \d{4}, \d{1,2}:\d{1,2}")
+        """
+        Скомпилированное регулярное выражение, описывающее дату заказа в формате <ДД месяца ГГГГ, ЧЧ:ММ>.
+        """
+
         self.DISCORD = "Вы можете перейти в Discord. " \
                        "Внимание: общение за пределами сервера FunPay считается нарушением правил."
         """
         Точный текст сообщения о предложении перехода в Discord.
         """
 
         self.PRODUCTS_AMOUNT = re.compile(r"\d+ шт\.")
```

### Comparing `FunPayAPI-1.0.7/FunPayAPI/types.py` & `FunPayAPI-1.0.8/FunPayAPI/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 В данном модуле описаны все типы пакета FunPayAPI
 """
 from __future__ import annotations
 from typing import Literal, overload, Optional
 from .common.utils import RegularExpressions
 from .common.enums import MessageTypes, OrderStatuses, SubCategoryTypes
+import datetime
 
 
 class ChatShortcut:
     """
     Данный класс представляет виджет чата со страницы https://funpay.com/chat/
 
     :param id_: ID чата.
@@ -252,37 +253,47 @@
 
     :param buyer_id: ID покупателя.
     :type buyer_id: :obj:`int`
 
     :param status: статус заказа.
     :type status: :class:`FunPayAPI.common.enums.OrderStatuses`
 
+    :param date: дата создания заказа.
+    :type date: :class:`datetime.datetime`
+
+    :param subcategory_name: название подкатегории, к которой относится заказ.
+    :type subcategory_name: :obj:`str`
+
     :param html: HTML код виджета заказа.
     :type html: :obj:`str`
 
     :param dont_search_amount: не искать кол-во товара.
     :type dont_search_amount: :obj:`bool`, опционально
     """
     def __init__(self, id_: str, description: str, price: float,
                  buyer_username: str, buyer_id: int, status: OrderStatuses,
-                 html: str, dont_search_amount: bool = False):
+                 date: datetime.datetime, subcategory_name: str, html: str, dont_search_amount: bool = False):
         self.id: str = id_ if not id_.startswith("#") else id_[1:]
         """ID заказа."""
         self.description: str = description
         """Описание заказа."""
         self.price: float = price
         """Цена заказа."""
         self.amount: int | None = self.parse_amount() if not dont_search_amount else None
         """Кол-во товаров."""
         self.buyer_username: str = buyer_username
         """Никнейм покупателя."""
         self.buyer_id: int = buyer_id
         """ID покупателя."""
         self.status: OrderStatuses = status
         """Статус заказа."""
+        self.date: datetime.datetime = date
+        """Дата создания заказа."""
+        self.subcategory_name: str = subcategory_name
+        """Название подкатегории, к которой относится заказ."""
         self.html: str = html
         """HTML код виджета заказа."""
 
     def parse_amount(self) -> int:
         """
         Парсит кол-во купленного товара (ищет подстроку по регулярному выражению).
```

### Comparing `FunPayAPI-1.0.7/FunPayAPI/updater/events.py` & `FunPayAPI-1.0.8/FunPayAPI/updater/events.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.7/FunPayAPI/updater/runner.py` & `FunPayAPI-1.0.8/FunPayAPI/updater/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         if not self.make_order_requests:
             return events
 
         attempts = 3
         while attempts:
             attempts -= 1
             try:
-                orders_list = self.account.get_sales()
+                orders_list = self.account.get_sells()
                 break
             except exceptions.RequestFailedError as e:
                 logger.error(e)
             except:
                 logger.error("Не удалось обновить список заказов.")
                 logger.debug("TRACEBACK", exc_info=True)
             time.sleep(1)
```

### Comparing `FunPayAPI-1.0.7/FunPayAPI.egg-info/PKG-INFO` & `FunPayAPI-1.0.8/FunPayAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FunPayAPI
-Version: 1.0.7
+Version: 1.0.8
 Summary: Прослойка между FunPayAPI и клиентом.
 Home-page: https://github.com/woopertail/FunPayAPI
 Author: Woopertail
 Author-email: woopertail@gmail.com
 License: GPL2
 Keywords: funpay bot api tools
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.7 Summary:
+Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.8 Summary:
 ÐÑÐ¾ÑÐ»Ð¾Ð¹ÐºÐ° Ð¼ÐµÐ¶Ð´Ñ FunPayAPI Ð¸ ÐºÐ»Ð¸ÐµÐ½ÑÐ¾Ð¼. Home-page: https:/
 /github.com/woopertail/FunPayAPI Author: Woopertail Author-email:
 woopertail@gmail.com License: GPL2 Keywords: funpay bot api tools Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python :: 3 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/markdown License-File: LICENSE [https://
```

### Comparing `FunPayAPI-1.0.7/LICENSE` & `FunPayAPI-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.7/PKG-INFO` & `FunPayAPI-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FunPayAPI
-Version: 1.0.7
+Version: 1.0.8
 Summary: Прослойка между FunPayAPI и клиентом.
 Home-page: https://github.com/woopertail/FunPayAPI
 Author: Woopertail
 Author-email: woopertail@gmail.com
 License: GPL2
 Keywords: funpay bot api tools
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.7 Summary:
+Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.8 Summary:
 ÐÑÐ¾ÑÐ»Ð¾Ð¹ÐºÐ° Ð¼ÐµÐ¶Ð´Ñ FunPayAPI Ð¸ ÐºÐ»Ð¸ÐµÐ½ÑÐ¾Ð¼. Home-page: https:/
 /github.com/woopertail/FunPayAPI Author: Woopertail Author-email:
 woopertail@gmail.com License: GPL2 Keywords: funpay bot api tools Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python :: 3 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/markdown License-File: LICENSE [https://
```

### Comparing `FunPayAPI-1.0.7/README.md` & `FunPayAPI-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.7/setup.py` & `FunPayAPI-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_desc = f.read()
 
 
 setup(name='FunPayAPI',
-      version="1.0.7",
+      version="1.0.8",
       description='Прослойка между FunPayAPI и клиентом.',
       long_description=long_desc,
       long_description_content_type="text/markdown",
       author='Woopertail',
       author_email='woopertail@gmail.com',
       url='https://github.com/woopertail/FunPayAPI',
       packages=find_packages("."),
```

