# Comparing `tmp/denemesonuc-0.1.7.tar.gz` & `tmp/denemesonuc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denemesonuc-0.1.7.tar", max compression
+gzip compressed data, was "denemesonuc-0.2.0.tar", max compression
```

## Comparing `denemesonuc-0.1.7.tar` & `denemesonuc-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/LICENSE
--rw-r--r--   0        0        0       67 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/README.md
--rw-r--r--   0        0        0      186 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/denemesonuc/__init__.py
--rw-r--r--   0        0        0     3078 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/denemesonuc/denek.py
--rw-r--r--   0        0        0     6684 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/denemesonuc/fetch_new.py
--rw-r--r--   0        0        0     4982 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/denemesonuc/fetch_old.py
--rw-r--r--   0        0        0     2736 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/denemesonuc/models.py
--rw-r--r--   0        0        0      622 2023-05-02 16:09:15.148907 denemesonuc-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 denemesonuc-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/LICENSE
+-rw-r--r--   0        0        0       67 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/README.md
+-rw-r--r--   0        0        0     2366 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/denemesonuc/__init__.py
+-rw-r--r--   0        0        0     6370 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/denemesonuc/fetchers/karnemiz.py
+-rw-r--r--   0        0        0     7544 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/denemesonuc/fetchers/okulizyon.py
+-rw-r--r--   0        0        0     6835 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/denemesonuc/models.py
+-rw-r--r--   0        0        0      315 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/denemesonuc/utils.py
+-rw-r--r--   0        0        0      713 2023-05-19 10:54:38.141023 denemesonuc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 denemesonuc-0.2.0/PKG-INFO
```

### Comparing `denemesonuc-0.1.7/LICENSE` & `denemesonuc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `denemesonuc-0.1.7/denemesonuc/fetch_new.py` & `denemesonuc-0.2.0/denemesonuc/fetchers/karnemiz.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,179 +1,198 @@
-from selenium.common.exceptions import NoSuchElementException, TimeoutException
+"""Fetcher module for the `bes.karnemiz.com` (old) type frontend."""
+
 from selenium.webdriver.remote.webdriver import WebDriver
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
 
-import denemesonuc.models
+from denemesonuc.models import Denek
 
 
 def fetch(
     driver: WebDriver,
-    ad: str,
-    no: int,
-    duzey: int,
-    sehir: str,
-    ilce: str,
-    kurum: str,
-    deneme: denemesonuc.models.DenemeLogin,
-    starting_div: int = 8,
-    naming_aliases: dict[str, str] = {},
-) -> denemesonuc.models.DenemeResult:
-    """### denek ve deneme bilgileriyle yeni tip deneme sonuçlarını çeker
-
-    returns DenemeResult if successful
-    raises DenekNotFound if denek did not take the test
-    raises RunTimeError if element with text not found on login page"""
-
-    ret = denemesonuc.models.DenemeResult()
-
-    if deneme.logout_url:
-        driver.get(deneme.logout_url)
-
-    driver.get(deneme.url)
-
-    def click_on_list_element(text_equal_to: str, *args, **kwargs):
-        ul = driver.find_element(*args, **kwargs)
-        li = ul.find_elements("tag name", "li")
-        for i in li:
-            if i.text == text_equal_to:
-                i.click()
-                return
-        raise RuntimeError(f"element with text {text_equal_to} not found")
-
-    driver.find_element("id", "select2-gt_ogrencino_sinifcombo-container").click()
-    click_on_list_element(str(duzey) + ".Sınıf", "id", "select2-gt_ogrencino_sinifcombo-results")
-
-    driver.find_element("id", "select2-gt_ogrencino_ilcombo-container").click()
-    click_on_list_element(sehir, "id", "select2-gt_ogrencino_ilcombo-results")
-
-    driver.find_element("id", "select2-gt_ogrencino_ilcecombo-container").click()
-    click_on_list_element(ilce, "id", "select2-gt_ogrencino_ilcecombo-results")
-
-    driver.find_element("id", "select2-gt_ogrencino_kurumcombo-container").click()
-    click_on_list_element(kurum, "id", "select2-gt_ogrencino_kurumcombo-results")
-
-    ogrnoinp = driver.find_element("id", "gt_ogrencino_ogrnoedit")
-    ogrnoinp.send_keys(str(no))
-
-    # if it exists, type value
-    for i in ("gt_ogrencino_adsoyadedit", "gt_ogrencino_adedit"):
-        try:
-            adinp = driver.find_element("id", i)
-            adinp.send_keys(ad)
-        except NoSuchElementException:
-            pass
+    denek: Denek,
+    deneme_url: str,
+    deneme_name: str,
+    deneme_lesson_names: dict[str, dict] = {},
+    **fetch_options,
+) -> None:
+    """Fetch the report of the given denek.
+
+    This function implements the logic of fetching the report of the \
+        given denek from the remote web server that uses the `bes.karnemiz.com` (old) \
+        type frontend.
+    
+    Args:
+        driver: \
+            The selenium driver object that will be used to fetch the \
+            deneme results.
+        denek: The denek that will be fetched.
+        deneme_url: The url of the remote web server that \
+            contains the deneme results.
+        deneme_name: The name of the deneme.
+        deneme_lesson_names: The names of the lessons that are in the \
+            deneme. The keys are the short names of the lessons and the \
+            values are dicts that contain the names of the lessons and the \
+            number of questions in the lessons. Total lessons are fetched \
+            in a different way, so they don't need to be included in this \
+            dict.
+        **fetch_options: The options that are used to fetch the \
+            deneme results.
+    
+    Raises:
+        ...
+    """
+    from selenium.common.exceptions import NoSuchElementException, TimeoutException
+    from selenium.webdriver.remote.webelement import WebElement
+    from selenium.webdriver.support import expected_conditions as EC
+    from selenium.webdriver.support.select import Select
+    from selenium.webdriver.support.wait import WebDriverWait
+
+    from denemesonuc.models import (
+        DenekDidntTakeDeneme,
+        DenekProbablyDidntTakeDeneme,
+        LessonBasedResult,
+        LessonResultContainer,
+        Ranking,
+        Report,
+    )
+    from denemesonuc.utils import uppercase_tr
+
+    if logout := fetch_options.get("deneme_logout_url"):
+        driver.get(logout)
+
+    driver.get(deneme_url)
 
-    driver.find_element("id", "gt_ogrencino_girisbtn").submit()
+    # at login page
+
+    # grade
+    Select(driver.find_element("id", "seviye")).select_by_visible_text(denek.grade)
+
+    # province
+    Select(driver.find_element("id", "ilkodu")).select_by_visible_text(
+        uppercase_tr(denek.province)
+    )
 
+    # school
+    driver.find_element("id", "kurumarama").send_keys(denek.school)
+    WebDriverWait(driver, 3).until(EC.presence_of_element_located(("id", "ui-id-2")))
+    driver.find_element("id", "ui-id-2").click()
+
+    # number
+    driver.find_element("id", "ogrencino").send_keys(denek.number)
+
+    # name
+    driver.find_element("id", "isim").send_keys(denek.name)
+
+    # submit
+    driver.find_element("name", "bulbtn1").submit()
+
+    # at report page
     try:
-        WebDriverWait(driver, 6).until(
-            EC.presence_of_element_located(("xpath", "/html/body/section/div/div[1]/div/div/h6[2]"))
+        WebDriverWait(driver, 5).until(
+            EC.presence_of_element_located(
+                (
+                    "xpath",
+                    "/html/body/div[1]/section/div/div/div[1]",
+                )  # base xpath for deneme selection
+            )
         )
     except TimeoutException as e:
-        raise TimeoutException("denek probably did not take the test") from e
+        raise DenekProbablyDidntTakeDeneme(
+            f"Denek probably did not take any denemes from {deneme_url}"
+        ) from e
+
+    # select correct deneme
+    deneme_selector = Select(driver.find_element("id", "digersinavlarcombo"))
+
+    try:
+        deneme_selector.select_by_visible_text(deneme_name)
+    except NoSuchElementException as e:
+        raise DenekDidntTakeDeneme(
+            f"Denek did not take the deneme {deneme_name} from {deneme_url}"
+        ) from e
+
+    WebDriverWait(driver, 5).until(
+        EC.text_to_be_present_in_element(
+            ("xpath", "/html/body/div[1]/section/div/div/div[4]/div/div"), deneme_name
+        )
+    )
+
+    root = driver.find_element("xpath", "/html/body/div[1]/section/div/div")
 
-    root = driver.find_element("xpath", "/html/body/section")
-    li = root.find_elements("tag name", "a")
-    for i in li:
-        if i.text == deneme.deneme_adi:
-            i.click()
-            break
-    else:
-        raise denemesonuc.models.DenekNotFound("denek did not take the test")
-
-    # at data page
-
-    document = "/html/body/section"
-
-    derece_head = f"{document}/div[1]/div[5]/div/div/div/"
-    d_sinif = int(
-        driver.find_element("xpath", f"{derece_head}/div[2]").text
-    )  # /html/body/section/div[1]/div[5]/div/div/div/div[2]
-    d_kurum = int(
-        driver.find_element("xpath", f"{derece_head}/div[3]").text
-    )  # /html/body/section/div[1]/div[5]/div/div/div/div[3]
-    d_il = int(driver.find_element("xpath", f"{derece_head}/div[5]").text)
-    d_genel = int(driver.find_element("xpath", f"{derece_head}/div[6]").text.split("\n")[0])
-    ret.drc = denemesonuc.models.DenemeDerece(d_sinif, d_kurum, d_il, d_genel)
-
-    ret.sinif = (
-        driver.find_element("xpath", f"{document}/div/div[1]/div/div/h5")
-        .text.replace("-", "")  # 9larda "-9A" gibi, diğer sınıflarda "11A" gibi gözüküyor o yüzden
-        .split()[0]
-    )  # "12C / 987" gibi.
-
-    ret.puan = float(
-        driver.find_element(
-            "xpath", f"/html/body/section/div[1]/div[3]/div/div/div/div[2]"
-        ).text.replace(",", ".")
-    )
-
-    ul = driver.find_element("xpath", f"{document}/div[1]")
-    li = ul.find_elements("tag name", "div")
-
-    i = starting_div - 1
-    available_heads = {}
-    while True:
-        i += 1
-        try:
-            driver.find_element("xpath", f"{document}/div[1]/div[{i}]")
-        except NoSuchElementException:
-            break
-
-        try:
-            b = driver.find_element("xpath", f"{document}/div[1]/div[{i}]/div/div")
-            c = driver.find_element("xpath", f"{document}/div[1]/div[{i+1}]/div[2]/div/div")
-        except NoSuchElementException:
-            continue
-
-        if c.find_elements("tag name", "h3"):
-            h = "3"
-        elif c.find_elements("tag name", "h2"):
-            h = "2"
-        elif c.find_elements("tag name", "h5"):
-            h = "5[2]"
-        else:
-            continue
-
-        available_heads[b.text] = denemesonuc.models.DersSonuc(
-            int(
-                driver.find_element(
-                    "xpath", f"{document}/div[1]/div[{i+1}]/div[2]/div/div/h{h}"
-                ).text
-            ),
-            int(
-                driver.find_element(
-                    "xpath", f"{document}/div[1]/div[{i+1}]/div[3]/div/div/h{h}"
-                ).text
-            ),
-            int(
-                driver.find_element(
-                    "xpath", f"{document}/div[1]/div[{i+1}]/div[4]/div/div/h{h}"
-                ).text
-            ),
-            float(
-                driver.find_element(
-                    "xpath", f"{document}/div[1]/div[{i+1}]/div[5]/div/div/h{h}"
-                ).text.replace(",", ".")
-            ),
-            int(
-                driver.find_element(
-                    "xpath", f"{document}/div[1]/div[{i+1}]/div[1]/div/div/h{h}"
-                ).text
-            ),
+    rank_root1 = root.find_element("xpath", "./div[5]/div/div[3]/div")
+    rank_root2 = root.find_element("xpath", "./div[5]/div/div[5]/div")
+
+    ranks = []
+    for i in range(2, 7):
+        ranks.append(int(rank_root1.find_element("xpath", f"./div[{i}]").text))
+    for i in range(2, 7):
+        ranks.append(int(rank_root2.find_element("xpath", f"./div[{i}]").text))
+
+    ranking = Ranking(
+        *ranks,
+    )
+
+    class_ = root.find_element("xpath", "./div[1]/div[2]/div[3]").text.replace(
+        "-", ""
+    )  # "-9A", "11A"
+
+    score = float(
+        root.find_element("xpath", "./div[5]/div/div[1]/div/div")
+        .text.replace(",", ".")
+        .split(" ")[-1]
+    )  # "score: 123,456"
+
+    result_data = {}
+
+    def to_lesson_result(elem: WebElement) -> LessonBasedResult:
+        """Convert the given element to a lesson based result.
+
+        Args:
+            elem: The element that will be converted.
+
+        Returns:
+            The converted element.
+        """
+        name = elem.find_element("xpath", "./div[1]/div").text
+        count = int(elem.find_element("xpath", "./div[2]/div[2]/div[1]").text)
+        true = int(elem.find_element("xpath", "./div[2]/div[2]/div[2]").text)
+        false = int(elem.find_element("xpath", "./div[2]/div[2]/div[3]").text)
+        empty = count - true - false
+        net = float(
+            elem.find_element("xpath", "./div[2]/div[2]/div[4]").text.replace(",", ".")
+        )
+        return LessonBasedResult(
+            full_name=name,
+            question_count=count,
+            true=true,
+            false=false,
+            empty=empty,
+            net=net,
         )
 
-    ret.genel = available_heads.get(naming_aliases.get("genel", "Toplam"))
-    ret.edb = available_heads.get(naming_aliases.get("edb", "TYT Türkçe Testi Toplamı"))
-    ret.trh = available_heads.get(naming_aliases.get("trh", "Tarih-1"))
-    ret.cog = available_heads.get(naming_aliases.get("cog", "Coğrafya-1"))
-    ret.din = available_heads.get(naming_aliases.get("din", "Din Kül. ve Ahl. Bil."))
-    ret.mat = available_heads.get(naming_aliases.get("mat", "TYT Matematik Testi Toplamı"))
-    ret.fiz = available_heads.get(naming_aliases.get("fiz", "Fizik"))
-    ret.kim = available_heads.get(naming_aliases.get("kim", "Kimya"))
-    ret.biy = available_heads.get(naming_aliases.get("biy", "Biyoloji"))
-    ret.fel = available_heads.get(naming_aliases.get("fel", "Felsefe"))
-    ret.sfl = available_heads.get(naming_aliases.get("sfl", "Felsefe (Seçmeli)"))
+    for i in root.find_elements("xpath", "./div[7]/div/div[*]/div[1]"):
+        if i.find_element("xpath", "./div[2]/div[2]/div[1]").text:
+            r = to_lesson_result(i)
+            result_data[r.full_name] = r
+
+    response = {}
+    for export, (d) in deneme_lesson_names.items():
+        name = d["name"]
+        count = d["question_count"]
+        result = result_data.get(name, LessonBasedResult.create_empty(count, name))
+        response[export] = result
+
+    total = to_lesson_result(root.find_element("xpath", "./div[6]/div/div/div[1]"))
 
+    result = LessonResultContainer(
+        response,
+    )
 
-    return ret
+    denek.add_report(
+        Report(
+            score=score,
+            denek_class=class_,
+            ranking=ranking,
+            result=total,
+            lessons=result,
+            deneme_name=deneme_name,
+        )
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `denemesonuc-0.1.7/pyproject.toml` & `denemesonuc-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 [tool.poetry]
 name = "denemesonuc"
-version = "0.1.7"
+version = "0.2.0"
 description = "orbim ölçme değerlendirme şeyi için bir modül"
 authors = ["insanolanbiri <erenakgun2007@hotmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com:/insanolanbiri/denemesonuc"
 classifiers = [
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/insanolanbiri/denemesonuc/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.10"
 selenium = "^4.8.2"
 
 [tool.poetry.dev-dependencies]
+black = "^23.3.0"
+isort = "^5.12.0"
+pydocstyle = "^6.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+profile = "black"
```

### Comparing `denemesonuc-0.1.7/PKG-INFO` & `denemesonuc-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: denemesonuc
-Version: 0.1.7
+Version: 0.2.0
 Summary: orbim ölçme değerlendirme şeyi için bir modül
 Home-page: https://github.com:/insanolanbiri/denemesonuc
 License: GPL-3.0-only
 Author: insanolanbiri
 Author-email: erenakgun2007@hotmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: selenium (>=4.8.2,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/insanolanbiri/denemesonuc/issues
 Project-URL: Repository, https://github.com:/insanolanbiri/denemesonuc
 Description-Content-Type: text/markdown
```

