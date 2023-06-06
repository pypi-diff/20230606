# Comparing `tmp/caqui-1.0.8.tar.gz` & `tmp/caqui-1.9.0.tar.gz`

## Comparing `caqui-1.0.8.tar` & `caqui-1.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.0.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 caqui-1.0.8/sample.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 caqui-1.0.8/test-requirements.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.0.8/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.0.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.0.8/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.0.8/.vscode/settings.json
--rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/__init__.py
--rw-r--r--   0        0        0     8430 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/asynchronous.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/constants.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/exceptions.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/helper.py
--rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 caqui-1.0.8/caqui/synchronous.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/constants.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/fake_responses.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/test_sniffer.py
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/feature/test_sync_and_async.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/html/playground.html
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/integration/test_async_scenarios.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/integration/test_sync_scenarios.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/unit/__initi__.py
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/unit/test_async_unit.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/unit/test_helper.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 caqui-1.0.8/tests/unit/test_sync_unit.py
--rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-1.0.8/utils/coverage.sh
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.0.8/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.0.8/LICENSE
--rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 caqui-1.0.8/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 caqui-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 caqui-1.9.0/sample.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 caqui-1.9.0/test-requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.9.0/.vscode/settings.json
+-rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/__init__.py
+-rw-r--r--   0        0        0    10603 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/asynchronous.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/constants.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/exceptions.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/helper.py
+-rw-r--r--   0        0        0    10062 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/synchronous.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/constants.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/fake_responses.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/test_sniffer.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/feature/test_sync_and_async.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/html/playground.html
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/integration/test_async_scenarios.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/integration/test_sync_scenarios.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/__initi__.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/test_async_unit.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/test_helper.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/test_sync_unit.py
+-rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-1.9.0/utils/coverage.sh
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.9.0/LICENSE
+-rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 caqui-1.9.0/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 caqui-1.9.0/PKG-INFO
```

### Comparing `caqui-1.0.8/CODE_OF_CONDUCT.md` & `caqui-1.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/sample.py` & `caqui-1.9.0/sample.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/.github/ISSUE_TEMPLATE/bug_report.md` & `caqui-1.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/.github/ISSUE_TEMPLATE/feature_request.md` & `caqui-1.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/.github/workflows/python-app.yml` & `caqui-1.9.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/.github/workflows/python-publish.yml` & `caqui-1.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/caqui/__init__.py` & `caqui-1.9.0/caqui/__init__.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/caqui/asynchronous.py` & `caqui-1.9.0/caqui/asynchronous.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,26 +31,87 @@
             async with session.get(url, headers=HEADERS) as resp:
                 response = await resp.json()
                 return response
     except Exception as error:
         raise WebDriverError("'GET' request failed.") from error
 
 
+async def clear_element(driver_url, session, element):
+    """Clear the element text"""
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/clear"
+        payload = json.dumps({"id": element})
+        await __post(url, payload)
+        return True
+    except Exception as error:
+        raise WebDriverError("Failed to clear the element text.") from error
+
+
+async def is_element_enabled(driver_url, session, element):
+    """Check if element is enabled"""
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/enabled"
+        response = await __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to check if element is enabled.") from error
+
+
+async def get_css_value(driver_url, session, element, property_name):
+    """Check if element is selected"""
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/css/{property_name}"
+        response = await __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to check if element is selected.") from error
+
+
+async def is_element_selected(driver_url, session, element):
+    """Check if element is selected"""
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/selected"
+        response = await __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to check if element is selected.") from error
+
+
+async def get_window_rectangle(driver_url, session):
+    """Get window rectangle"""
+    try:
+        url = f"{driver_url}/session/{session}/window/rect"
+        response = await __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to get window rectangle.") from error
+
+
+async def get_window_handles(driver_url, session):
+    """Get window handles"""
+    try:
+        url = f"{driver_url}/session/{session}/window/handles"
+        response = await __get(url)
+        return response.get("value")
+    except Exception as error:
+        raise WebDriverError("Failed to get window handles.") from error
+
+
 async def close_window(driver_url, session):
     """Close active window"""
     try:
         url = f"{driver_url}/session/{session}/window"
         response = await __delete(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to close active window.") from error
 
 
 async def get_window(driver_url, session):
-    """Get window handle"""
+    """Get window"""
     try:
         url = f"{driver_url}/session/{session}/window"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
         raise WebDriverError("Failed to get window.") from error
```

### Comparing `caqui-1.0.8/caqui/synchronous.py` & `caqui-1.9.0/caqui/synchronous.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,25 +28,81 @@
 def __delete(url):
     try:
         return requests.request("DELETE", url, headers={}, data={}).json()
     except Exception as error:
         raise WebDriverError("'DELETE' request failed.") from error
 
 
+def clear_element(driver_url, session, element):
+    """Clear the element text"""
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/clear"
+        payload = json.dumps({"id": element})
+        __post(url, payload)
+        return True
+    except Exception as error:
+        raise WebDriverError(f"Failed to clear the element text.") from error
+
+
+def is_element_enabled(driver_url, session, element):
+    """Check if element is enabled"""
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/enabled"
+        return __get(url).get("value")
+    except Exception as error:
+        raise WebDriverError(f"Failed to check if element is enabled.") from error
+
+
+def get_css_value(driver_url, session, element, property_name):
+    """Get the css property value"""
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/css/{property_name}"
+        return __get(url).get("value")
+    except Exception as error:
+        raise WebDriverError(f"Failed to get the css property value.") from error
+
+
+def is_element_selected(driver_url, session, element):
+    """Check if element is selected"""
+    try:
+        url = f"{driver_url}/session/{session}/element/{element}/selected"
+        return __get(url).get("value")
+    except Exception as error:
+        raise WebDriverError(f"Failed to check if element is selected.") from error
+
+
+def get_window_rectangle(driver_url, session):
+    """Get window rectangle"""
+    try:
+        url = f"{driver_url}/session/{session}/window/rect"
+        return __get(url).get("value")
+    except Exception as error:
+        raise WebDriverError(f"Failed to get window rectangle.") from error
+
+
+def get_window_handles(driver_url, session):
+    """Get window handles"""
+    try:
+        url = f"{driver_url}/session/{session}/window/handles"
+        return __get(url).get("value")
+    except Exception as error:
+        raise WebDriverError(f"Failed to get window handles.") from error
+
+
 def close_window(driver_url, session):
     """Close active window"""
     try:
         url = f"{driver_url}/session/{session}/window"
         return __delete(url).get("value")
     except Exception as error:
         raise WebDriverError(f"Failed to close active window.") from error
 
 
 def get_window(driver_url, session):
-    """Get window handle"""
+    """Get window"""
     try:
         url = f"{driver_url}/session/{session}/window"
         return __get(url).get("value")
     except Exception as error:
         raise WebDriverError(f"Failed to get window.") from error
```

### Comparing `caqui-1.0.8/tests/fake_responses.py` & `caqui-1.9.0/tests/fake_responses.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,17 +26,55 @@
 
 FIND_ELEMENT = DEFAULT
 SEND_KEYS = DEFAULT
 CLICK = DEFAULT
 CLOSE_SESSION = DEFAULT
 GO_TO_PAGE = DEFAULT
 
+GET_WINDOW_RECTANGLE = dict_to_json(
+    {
+        "sessionId": "79e4bd950a886e0119e3760d201b059e",
+        "status": 0,
+        "value": {"height": 600, "width": 800, "x": 0, "y": 0},
+    }
+)
+
+
+CLEAR_ELEMENT = dict_to_json(
+    {"sessionId": "486fa32a9876b4519e149b39135edcb5", "status": 0, "value": None}
+)
+
+IS_ELEMENT_ENABLED = dict_to_json(
+    {"sessionId": "e0e43cd1ce532b5aa62b6df0de11e3bd", "status": 0, "value": True}
+)
+
+GET_CSS_COLOR_VALUE = dict_to_json(
+    {
+        "sessionId": "e7f659e7183778e98ce9357051e40a47",
+        "status": 0,
+        "value": "rgba(0, 0, 0, 1)",
+    }
+)
+
+IS_ELEMENT_SELECTED = dict_to_json(
+    {"sessionId": "341d21063846141d2716d300652ddd81", "status": 0, "value": False}
+)
+
+GET_WINDOW_HANDLES = dict_to_json(
+    {
+        "sessionId": "b3f92cf70d734ecc6fcddbd88671998a",
+        "status": 0,
+        "value": ["2E55CCE389196328988ED244DAA52A5D"],
+    }
+)
+
 CLOSE_WINDOW = dict_to_json(
     {"sessionId": "48399161591a0bc1dffaa2ff2d65aa0f", "status": 0, "value": []}
 )
+
 GET_WINDOW = dict_to_json(
     {
         "sessionId": "ce68162d420e9cb2b1617c2d1a800f85",
         "status": 0,
         "value": "845623CAE8115F2B60C9AE8596F13D94",
     }
 )
```

### Comparing `caqui-1.0.8/tests/test_sniffer.py` & `caqui-1.9.0/tests/test_sniffer.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,14 +23,21 @@
     driver.get(PAGE_URL)
     driver
     yield driver
     driver.quit()
 
 
 @mark.skip("used just to discover request data")
+def test_clear(setup):
+    driver = setup
+    element = driver.find_element("xpath", "//input")
+    assert element.clear() == "any"
+
+
+@mark.skip("used just to discover request data")
 def test_back(setup):
     assert setup.back() == "any"
 
 
 @mark.skip("used just to discover request data")
 def test_get_title(setup):
     assert setup.title == "any"
```

### Comparing `caqui-1.0.8/tests/feature/test_sync_and_async.py` & `caqui-1.9.0/tests/feature/test_sync_and_async.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,14 +21,92 @@
         session,
         PAGE_URL,
     )
     yield driver_url, session
     synchronous.close_session(driver_url, session)
 
 
+@mark.asyncio
+async def test_clear_element(__setup):
+    driver_url, session = __setup
+    locator_type = "xpath"
+    locator_value = "//input"
+    text = "any"
+
+    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
+    synchronous.send_keys(driver_url, session, element, text)
+    assert synchronous.clear_element(driver_url, session, element) is True
+
+    synchronous.send_keys(driver_url, session, element, text)
+    assert await asynchronous.clear_element(driver_url, session, element) is True
+
+
+@mark.asyncio
+async def test_is_element_enabled(__setup):
+    driver_url, session = __setup
+    locator_type = "xpath"
+    locator_value = "//input"
+
+    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
+
+    assert synchronous.is_element_enabled(driver_url, session, element) is True
+    assert await asynchronous.is_element_enabled(driver_url, session, element) is True
+
+
+@mark.asyncio
+async def test_get_css_value(__setup):
+    driver_url, session = __setup
+    locator_type = "xpath"
+    locator_value = "//input"
+    property_name = "color"
+    expected = "rgba(0, 0, 0, 1)"
+
+    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
+
+    assert (
+        synchronous.get_css_value(driver_url, session, element, property_name)
+        == expected
+    )
+    assert (
+        await asynchronous.get_css_value(driver_url, session, element, property_name)
+        == expected
+    )
+
+
+@mark.asyncio
+async def test_is_element_selected(__setup):
+    driver_url, session = __setup
+    locator_type = "xpath"
+    locator_value = "//input"
+
+    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
+
+    assert synchronous.is_element_selected(driver_url, session, element) is False
+    assert await asynchronous.is_element_selected(driver_url, session, element) is False
+
+
+@mark.asyncio
+async def test_get_window_rectangle(__setup):
+    driver_url, session = __setup
+    expected = "height"
+
+    assert expected in synchronous.get_window_rectangle(driver_url, session)
+    rectangle = await asynchronous.get_window_rectangle(driver_url, session)
+    assert expected in rectangle
+
+
+@mark.asyncio
+async def test_get_window_handles(__setup):
+    driver_url, session = __setup
+
+    assert isinstance(synchronous.get_window_handles(driver_url, session), list)
+    handles = await asynchronous.get_window_handles(driver_url, session)
+    assert isinstance(handles, list)
+
+
 def test_close_window_sync(__setup):
     driver_url, session = __setup
     assert isinstance(synchronous.close_window(driver_url, session), list)
 
 
 @mark.asyncio
 async def test_close_window_async(__setup):
```

### Comparing `caqui-1.0.8/tests/html/playground.html` & `caqui-1.9.0/tests/html/playground.html`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/tests/integration/test_async_scenarios.py` & `caqui-1.9.0/tests/integration/test_async_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/tests/integration/test_sync_scenarios.py` & `caqui-1.9.0/tests/integration/test_sync_scenarios.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import json
 from caqui.synchronous import (
     find_element,
     get_session,
     click,
     send_keys,
     get_text,
     close_session,
     go_to_page,
     get_property,
+    clear_element,
 )
 from tests.constants import PAGE_URL
 from pytest import fixture
 
 
 @fixture
 def __setup():
     driver_url = "http://127.0.0.1:9999"
     capabilities = {
         "desiredCapabilities": {
-            "browserName": "firefox",
+            "browserName": "chrome",
             "marionette": True,
             "acceptInsecureCerts": True,
             "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
         }
     }
     session = get_session(driver_url, capabilities)
     go_to_page(
@@ -38,14 +38,16 @@
     driver_url, session = __setup
     expected = "end"
     locator_type = "xpath"
 
     input = find_element(driver_url, session, locator_type, locator_value="//input")
     send_keys(driver_url, session, input, "any")
     assert get_property(driver_url, session, input, property="value") == "any"
+    clear_element(driver_url, session, input)
+    assert get_property(driver_url, session, input, property="value") == ""
 
     anchor = find_element(driver_url, session, locator_type, locator_value="//a")
     assert (
         get_property(driver_url, session, anchor, property="href") == "http://any1.com/"
     )
 
     button = find_element(driver_url, session, locator_type, locator_value="//button")
```

### Comparing `caqui-1.0.8/tests/unit/test_async_unit.py` & `caqui-1.9.0/tests/unit/test_async_unit.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,183 +3,243 @@
 
 from pytest import mark
 from caqui import asynchronous
 from tests import fake_responses
 from unittest.mock import patch
 
 
-async def mock_post(*args):
+async def mock_request(*args):
     pass
 
 
 @mark.asyncio
+async def test_clear_element():
+    async def mock_request(*args):
+        return fake_responses.CLEAR_ELEMENT
+
+    with patch("caqui.asynchronous.__post", mock_request):
+        assert await asynchronous.clear_element("", "", "") is True
+
+
+@mark.asyncio
+async def test_is_element_enabled():
+    async def mock_request(*args):
+        return fake_responses.IS_ELEMENT_ENABLED
+
+    with patch("caqui.asynchronous.__get", mock_request):
+        assert await asynchronous.is_element_enabled("", "", "") is True
+
+
+@mark.asyncio
+async def test_get_css_value():
+    expected = "rgba(0, 0, 0, 1)"
+
+    async def mock_request(*args):
+        return fake_responses.GET_CSS_COLOR_VALUE
+
+    with patch("caqui.asynchronous.__get", mock_request):
+        assert await asynchronous.get_css_value("", "", "", "") == expected
+
+
+@mark.asyncio
+async def test_is_element_selected():
+    async def mock_request(*args):
+        return fake_responses.IS_ELEMENT_SELECTED
+
+    with patch("caqui.asynchronous.__get", mock_request):
+        assert await asynchronous.is_element_selected("", "", "") is False
+
+
+@mark.asyncio
+async def test_get_window_rectangle():
+    expected = "height"
+
+    async def mock_request(*args):
+        return fake_responses.GET_WINDOW_RECTANGLE
+
+    with patch("caqui.asynchronous.__get", mock_request):
+        assert expected in await asynchronous.get_window_rectangle("", "")
+
+
+@mark.asyncio
+async def test_get_window_handles():
+    expected = ["2E55CCE389196328988ED244DAA52A5D"]
+
+    async def mock_request(*args):
+        return fake_responses.GET_WINDOW_HANDLES
+
+    with patch("caqui.asynchronous.__get", mock_request):
+        assert await asynchronous.get_window_handles("", "") == expected
+
+
+@mark.asyncio
 async def test_close_window():
     expected = []
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.CLOSE_WINDOW
 
-    with patch("caqui.asynchronous.__delete", mock_post):
+    with patch("caqui.asynchronous.__delete", mock_request):
         assert await asynchronous.close_window("", "") == expected
 
 
 @mark.asyncio
 async def test_get_window():
     expected = "845623CAE8115F2B60C9AE8596F13D94"
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.GET_WINDOW
 
-    with patch("caqui.asynchronous.__get", mock_post):
+    with patch("caqui.asynchronous.__get", mock_request):
         assert await asynchronous.get_window("", "") == expected
 
 
 @mark.asyncio
 async def test_go_back():
-    with patch("caqui.asynchronous.__post", mock_post):
+    with patch("caqui.asynchronous.__post", mock_request):
         assert await asynchronous.go_back("", "") is True
 
 
 @mark.asyncio
 async def test_get_property():
     expected = "any_value"
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.GET_PROPERTY_VALUE
 
-    with patch("caqui.asynchronous.__get", mock_post):
+    with patch("caqui.asynchronous.__get", mock_request):
         assert await asynchronous.get_property("", "", "", "") == expected
 
 
 @mark.asyncio
 async def test_get_attribute():
     expected = "any_value"
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.GET_ATTRIBUTE_VALUE
 
-    with patch("caqui.asynchronous.__get", mock_post):
+    with patch("caqui.asynchronous.__get", mock_request):
         assert await asynchronous.get_attribute("", "", "", "") == expected
 
 
 @mark.asyncio
 async def test_get_url():
     expected = "playground.html"
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.GET_URL
 
-    with patch("caqui.asynchronous.__get", mock_post):
+    with patch("caqui.asynchronous.__get", mock_request):
         response = await asynchronous.get_url("", "")
         assert expected in response
 
 
 @mark.asyncio
 async def test_get_timeouts():
     expected = "implicit"
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.GET_TIMEOUTS
 
-    with patch("caqui.asynchronous.__get", mock_post):
+    with patch("caqui.asynchronous.__get", mock_request):
         response = await asynchronous.get_timeouts("", "")
         assert expected in response
 
 
 @mark.asyncio
 async def test_get_status():
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.GET_STATUS
 
-    with patch("caqui.asynchronous.__get", mock_post):
+    with patch("caqui.asynchronous.__get", mock_request):
         response = await asynchronous.get_status("")
         assert response.get("value").get("ready") is True
 
 
 @mark.asyncio
 async def test_get_title():
     expected = "Sample page"
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.GET_TITLE
 
-    with patch("caqui.asynchronous.__get", mock_post):
+    with patch("caqui.asynchronous.__get", mock_request):
         assert await asynchronous.get_title("", "") == expected
 
 
 @mark.asyncio
 async def test_get_cookies():
     expected = []
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.GET_COOKIES
 
-    with patch("caqui.asynchronous.__get", mock_post):
+    with patch("caqui.asynchronous.__get", mock_request):
         assert await asynchronous.get_cookies("", "") == expected
 
 
 @mark.asyncio
 async def test_get_text():
     expected = "any"
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.GET_TEXT
 
-    with patch("caqui.asynchronous.__get", mock_post):
+    with patch("caqui.asynchronous.__get", mock_request):
         assert await asynchronous.get_text("", "", "") == expected
 
 
 @mark.asyncio
 async def test_close_session():
-    with patch("caqui.asynchronous.__delete", mock_post):
+    with patch("caqui.asynchronous.__delete", mock_request):
         assert await asynchronous.close_session("", "") is True
 
 
 @mark.asyncio
 async def test_go_to_page():
-    with patch("caqui.asynchronous.__post", mock_post):
+    with patch("caqui.asynchronous.__post", mock_request):
         assert await asynchronous.go_to_page("", "", "") is True
 
 
 @mark.asyncio
 async def test_send_keys():
-    with patch("caqui.asynchronous.__post", mock_post):
+    with patch("caqui.asynchronous.__post", mock_request):
         assert await asynchronous.send_keys("", "", "", "") is True
 
 
 @mark.asyncio
 async def test_click():
-    with patch("caqui.asynchronous.__post", mock_post):
+    with patch("caqui.asynchronous.__post", mock_request):
         assert await asynchronous.click("", "", "") is True
 
 
 @mark.asyncio
 async def test_find_elements():
     element = "C230605181E69CB2C4C36B8E83FE1245_element_2"
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.FIND_ELEMENTS
 
-    with patch("caqui.asynchronous.__post", mock_post):
+    with patch("caqui.asynchronous.__post", mock_request):
         assert element in await asynchronous.find_elements("", "", "", "")
 
 
 @mark.asyncio
 async def test_find_element():
     element = "0.8851292311864847-1"
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.FIND_ELEMENT
 
-    with patch("caqui.asynchronous.__post", mock_post):
+    with patch("caqui.asynchronous.__post", mock_request):
         assert await asynchronous.find_element("", "", "", "") == element
 
 
 @mark.asyncio
 async def test_get_session():
     expected = "4358a5b53794586af59678fc1653dc40"
 
-    async def mock_post(*args):
+    async def mock_request(*args):
         return fake_responses.GET_SESSION
 
-    with patch("caqui.asynchronous.__post", mock_post):
+    with patch("caqui.asynchronous.__post", mock_request):
         assert await asynchronous.get_session("", {}) == expected
```

### Comparing `caqui-1.0.8/tests/unit/test_helper.py` & `caqui-1.9.0/tests/unit/test_helper.py`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/tests/unit/test_sync_unit.py` & `caqui-1.9.0/tests/unit/test_sync_unit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,47 @@
 from unittest.mock import patch
 from caqui import synchronous
 from tests import fake_responses
 
 
+@patch("requests.request", return_value=fake_responses.CLEAR_ELEMENT)
+def test_clear_element(*args):
+    assert synchronous.clear_element("", "", "") is True
+
+
+@patch("requests.request", return_value=fake_responses.IS_ELEMENT_ENABLED)
+def test_is_element_enabled(*args):
+    assert synchronous.is_element_enabled("", "", "") is True
+
+
+@patch("requests.request", return_value=fake_responses.GET_CSS_COLOR_VALUE)
+def test_get_css_value(*args):
+    expected = "rgba(0, 0, 0, 1)"
+    assert synchronous.get_css_value("", "", "", "") == expected
+
+
+@patch("requests.request", return_value=fake_responses.IS_ELEMENT_SELECTED)
+def test_is_element_selected(*args):
+    assert synchronous.is_element_selected("", "", "") is False
+
+
+@patch("requests.request", return_value=fake_responses.GET_WINDOW_RECTANGLE)
+def test_get_window_rectangle(*args):
+    expected = "height"
+
+    assert expected in synchronous.get_window_rectangle("", "")
+
+
+@patch("requests.request", return_value=fake_responses.GET_WINDOW_HANDLES)
+def test_get_window_handles(*args):
+    expected = "2E55CCE389196328988ED244DAA52A5D"
+
+    assert expected in synchronous.get_window_handles("", "")
+
+
 @patch("requests.request", return_value=fake_responses.CLOSE_WINDOW)
 def test_close_window(*args):
     expected = []
 
     assert synchronous.close_window("", "") == expected
```

### Comparing `caqui-1.0.8/.gitignore` & `caqui-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/LICENSE` & `caqui-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/README.md` & `caqui-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `caqui-1.0.8/pyproject.toml` & `caqui-1.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 include = ["caqui*"]
 exclude = ["tests*", "utils", ".vscode", ".git*", "dist"]
 
 [project]
 name = "caqui"
-version = "1.0.8"
+version = "1.9.0"
 authors = [
   { name="Douglas Cardoso", email="noemail@noemail.com" },
 ]
 description = "Run asynchronous commands in WebDrivers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `caqui-1.0.8/PKG-INFO` & `caqui-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caqui
-Version: 1.0.8
+Version: 1.9.0
 Summary: Run asynchronous commands in WebDrivers
 Project-URL: Homepage, https://github.com/douglasdcm/caqui
 Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso <noemail@noemail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caqui Version: 1.0.8 Summary: Run asynchronous
+Metadata-Version: 2.1 Name: caqui Version: 1.9.0 Summary: Run asynchronous
 commands in WebDrivers Project-URL: Homepage, https://github.com/douglasdcm/
 caqui Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
 Author-email: Douglas Cardoso
 noemail.com> License-File: LICENSE Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
 Python: >=3.7 Requires-Dist: aiohttp Requires-Dist: requests Description-
```

