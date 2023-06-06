# Comparing `tmp/base_decorator-0.1.tar.gz` & `tmp/base_decorator-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\base_decorator-0.1.tar", last modified: Thu Jul  1 06:23:56 2021, max compression
+gzip compressed data, was "dist\base_decorator-0.2.tar", last modified: Tue Jun  6 02:35:13 2023, max compression
```

## Comparing `base_decorator-0.1.tar` & `base_decorator-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2021-07-01 06:23:56.000000 base_decorator-0.1/
-drwxrwxrwx   0        0        0        0 2021-07-01 06:23:56.000000 base_decorator-0.1/base_decorator/
--rw-rw-rw-   0        0        0     3174 2021-07-01 06:20:33.000000 base_decorator-0.1/base_decorator/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-01 06:23:56.000000 base_decorator-0.1/base_decorator.egg-info/
--rw-rw-rw-   0        0        0        1 2021-07-01 06:23:55.000000 base_decorator-0.1/base_decorator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4967 2021-07-01 06:23:55.000000 base_decorator-0.1/base_decorator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        7 2021-07-01 06:23:55.000000 base_decorator-0.1/base_decorator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      234 2021-07-01 06:23:55.000000 base_decorator-0.1/base_decorator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2021-07-01 06:23:55.000000 base_decorator-0.1/base_decorator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4967 2021-07-01 06:23:56.000000 base_decorator-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3286 2021-07-01 06:21:59.000000 base_decorator-0.1/README.md
--rw-rw-rw-   0        0        0       42 2021-07-01 06:23:56.000000 base_decorator-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1706 2021-07-01 06:23:42.000000 base_decorator-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 02:35:13.000000 base_decorator-0.2/
+-rw-rw-rw-   0        0        0     4060 2023-06-06 02:35:13.000000 base_decorator-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3316 2023-06-06 02:29:00.000000 base_decorator-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 02:35:13.000000 base_decorator-0.2/base_decorator/
+-rw-rw-rw-   0        0        0     3343 2023-06-06 02:33:59.000000 base_decorator-0.2/base_decorator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 02:35:13.000000 base_decorator-0.2/base_decorator.egg-info/
+-rw-rw-rw-   0        0        0     4060 2023-06-06 02:35:12.000000 base_decorator-0.2/base_decorator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-06 02:35:12.000000 base_decorator-0.2/base_decorator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 02:35:12.000000 base_decorator-0.2/base_decorator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 02:35:12.000000 base_decorator-0.2/base_decorator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-06 02:35:12.000000 base_decorator-0.2/base_decorator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 02:35:13.000000 base_decorator-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1706 2023-06-06 02:35:03.000000 base_decorator-0.2/setup.py
```

### Comparing `base_decorator-0.1/base_decorator/__init__.py` & `base_decorator-0.2/base_decorator/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import functools
 import abc
 import sys
 
+from typing import TypeVar
+
+F = TypeVar('F')
 
 class Undefind:
     pass
 
 
 class BaseDecorator(metaclass=abc.ABCMeta):
     """
     简化了装饰器的编写。
 
     用户的装饰器需要继承这个，用户可以按需重新定义 before，after，when_exception 方法。
 
     为了一致性和省事，统一采用有参数装饰器，用户的装饰器后面必须带括号。
 
-
+    用户可以选择重写 before  after  when_exception 三个方法
     """
 
     # def __init__(self, *args, **kwargs):
     #     pass
 
     raw_fun = Undefind()
     raw_result = Undefind()
     exc_info = Undefind()
     final_result = Undefind()  # 用户可以自己定义final_result的值，如果定义了就把这个值作为函数的结果，否则把函数原始结果作为结果。
 
-    def __call__(self, fun, *args, **kwargs):
+    def __call__(self, fun:F, *args, **kwargs) -> F:
         # print(locals())
         if not callable(fun) or args or kwargs:  # 正常是只有fun一个参数，除非是装饰器没加括号造成的。
             raise ValueError('为了简单和一致起见，所有装饰器都采用有参数装饰器，被装饰函数上面的装饰器后面别忘了加括号')
         self.raw_fun = fun
         f = functools.partial(BaseDecorator._execute, self)  # 比 self.execute 利于补全
         functools.update_wrapper(f, fun, )
         return f
@@ -91,15 +94,15 @@
 
             return __inner
 
         return _inner
 
 
     @MyDeco(b=4)
-    # @common_deco(b=4)
+    # @common_deco(b=4)  # 这两个装饰器等效，二选一。
     def fun3(x):
         print(x)
         return x * 2
 
 
     print(type(fun3))
     print(fun3)
```

### Comparing `base_decorator-0.1/base_decorator.egg-info/PKG-INFO` & `base_decorator-0.2/base_decorator.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,138 +1,140 @@
 Metadata-Version: 2.1
 Name: base-decorator
-Version: 0.1
+Version: 0.2
 Summary: base_decorator,make decorator easy to write
 Home-page: UNKNOWN
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
-Description: # base_decorator
-        
-        
-        ```
-        通用的装饰器基类，使写装饰器变得更简单。
-        ```
-        
-        ```python
-        import functools
-        import abc
-        import sys
-        
-        
-        class Undefind:
-            pass
-        
-        
-        class BaseDecorator(metaclass=abc.ABCMeta):
-            """
-            简化了装饰器的编写。
-        
-            用户的装饰器需要继承这个，用户可以按需重新定义 before，after，when_exception 方法。
-        
-            为了一致性和省事，统一采用有参数装饰器，用户的装饰器后面必须带括号。
-        
-        
-            """
-        
-            # def __init__(self, *args, **kwargs):
-            #     pass
-        
-            raw_fun = Undefind()
-            raw_result = Undefind()
-            exc_info = Undefind()
-            final_result = Undefind()  # 用户可以自己定义final_result的值，如果定义了就把这个值作为函数的结果，否则把函数原始结果作为结果。
-        
-            def __call__(self, fun, *args, **kwargs):
-                # print(locals())
-                if not callable(fun) or args or kwargs:  # 正常是只有fun一个参数，除非是装饰器没加括号造成的。
-                    raise ValueError('为了简单和一致起见，所有装饰器都采用有参数装饰器，被装饰函数上面的装饰器后面别忘了加括号')
-                self.raw_fun = fun
-                f = functools.partial(BaseDecorator._execute, self)  # 比 self.execute 利于补全
-                functools.update_wrapper(f, fun, )
-                return f
-        
-            def _execute(self, *args, **kwargs):
-                self.before()
-                try:
-                    self.raw_result = self.raw_fun(*args, **kwargs)
-                    self.after()
-                except Exception as e:
-                    self.exc_info = sys.exc_info()
-                    self.when_exception()
-                if not isinstance(self.final_result, Undefind):  # 用户可以自己定义final_result的值，如果定义了就把这个值作为函数的结果。
-                    return self.final_result
-                else:
-                    return self.raw_result
-        
-            def before(self):
-                pass
-        
-            def after(self):
-                pass
-        
-            def when_exception(self):
-                # print(self.exc_info) # (<class 'ZeroDivisionError'>, ZeroDivisionError('division by zero',), <traceback object at 0x000001D22BA3FD48>)
-                raise self.exc_info[1]
-        
-        
-        if __name__ == '__main__':
-            import nb_log  # noqa
-        
-        
-            class MyDeco(BaseDecorator):
-                def __init__(self, a=5, b=6):
-                    self.a = a
-                    self.b = b
-        
-                def before(self):
-                    print('开始执行')
-        
-                # noinspection PyAttributeOutsideInit
-                def after(self):
-                    self.final_result = self.a * self.b * self.raw_result
-        
-        
-            def common_deco(a=5, b=6):
-                """  上面的逻辑如果用常规方式写"""
-        
-                def _inner(f):
-                    @functools.wraps(f)
-                    def __inner(*args, **kwargs):
-                        try:
-                            print('开始执行')
-                            result = f(*args, **kwargs)
-                            return a * b * result
-                        except Exception as e:
-                            raise e
-        
-                    return __inner
-        
-                return _inner
-        
-        
-            @MyDeco(b=4)
-            # @common_deco(b=4)
-            def fun3(x):
-                print(x)
-                return x * 2
-        
-        
-            print(type(fun3))
-            print(fun3)
-            print(fun3.__wrapped__)  # noqa
-            print(fun3(10))
-        
-        ```
 Keywords: base_decorator
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
+
+# base_decorator
+
+pip install base_decorator
+```
+通用的装饰器基类，使写装饰器变得更简单。
+```
+
+```python
+import functools
+import abc
+import sys
+
+
+class Undefind:
+    pass
+
+
+class BaseDecorator(metaclass=abc.ABCMeta):
+    """
+    简化了装饰器的编写。
+
+    用户的装饰器需要继承这个，用户可以按需重新定义 before，after，when_exception 方法。
+
+    为了一致性和省事，统一采用有参数装饰器，用户的装饰器后面必须带括号。
+
+
+    """
+
+    # def __init__(self, *args, **kwargs):
+    #     pass
+
+    raw_fun = Undefind()
+    raw_result = Undefind()
+    exc_info = Undefind()
+    final_result = Undefind()  # 用户可以自己定义final_result的值，如果定义了就把这个值作为函数的结果，否则把函数原始结果作为结果。
+
+    def __call__(self, fun, *args, **kwargs):
+        # print(locals())
+        if not callable(fun) or args or kwargs:  # 正常是只有fun一个参数，除非是装饰器没加括号造成的。
+            raise ValueError('为了简单和一致起见，所有装饰器都采用有参数装饰器，被装饰函数上面的装饰器后面别忘了加括号')
+        self.raw_fun = fun
+        f = functools.partial(BaseDecorator._execute, self)  # 比 self.execute 利于补全
+        functools.update_wrapper(f, fun, )
+        return f
+
+    def _execute(self, *args, **kwargs):
+        self.before()
+        try:
+            self.raw_result = self.raw_fun(*args, **kwargs)
+            self.after()
+        except Exception as e:
+            self.exc_info = sys.exc_info()
+            self.when_exception()
+        if not isinstance(self.final_result, Undefind):  # 用户可以自己定义final_result的值，如果定义了就把这个值作为函数的结果。
+            return self.final_result
+        else:
+            return self.raw_result
+
+    def before(self):
+        pass
+
+    def after(self):
+        pass
+
+    def when_exception(self):
+        # print(self.exc_info) # (<class 'ZeroDivisionError'>, ZeroDivisionError('division by zero',), <traceback object at 0x000001D22BA3FD48>)
+        raise self.exc_info[1]
+
+
+if __name__ == '__main__':
+    import nb_log  # noqa
+
+
+    class MyDeco(BaseDecorator):
+        def __init__(self, a=5, b=6):
+            self.a = a
+            self.b = b
+
+        def before(self):
+            print('开始执行')
+
+        # noinspection PyAttributeOutsideInit
+        def after(self):
+            self.final_result = self.a * self.b * self.raw_result
+
+
+    def common_deco(a=5, b=6):
+        """  上面的逻辑如果用常规方式写"""
+
+        def _inner(f):
+            @functools.wraps(f)
+            def __inner(*args, **kwargs):
+                try:
+                    print('开始执行')
+                    result = f(*args, **kwargs)
+                    return a * b * result
+                except Exception as e:
+                    raise e
+
+            return __inner
+
+        return _inner
+
+
+    @MyDeco(b=4)
+    # @common_deco(b=4)
+    def fun3(x):
+        print(x)
+        return x * 2
+
+
+    print(type(fun3))
+    print(fun3)
+    print(fun3.__wrapped__)  # noqa
+    print(fun3(10))
+    
+```
+
```

### Comparing `base_decorator-0.1/PKG-INFO` & `base_decorator-0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,138 +1,140 @@
 Metadata-Version: 2.1
 Name: base_decorator
-Version: 0.1
+Version: 0.2
 Summary: base_decorator,make decorator easy to write
 Home-page: UNKNOWN
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
-Description: # base_decorator
-        
-        
-        ```
-        通用的装饰器基类，使写装饰器变得更简单。
-        ```
-        
-        ```python
-        import functools
-        import abc
-        import sys
-        
-        
-        class Undefind:
-            pass
-        
-        
-        class BaseDecorator(metaclass=abc.ABCMeta):
-            """
-            简化了装饰器的编写。
-        
-            用户的装饰器需要继承这个，用户可以按需重新定义 before，after，when_exception 方法。
-        
-            为了一致性和省事，统一采用有参数装饰器，用户的装饰器后面必须带括号。
-        
-        
-            """
-        
-            # def __init__(self, *args, **kwargs):
-            #     pass
-        
-            raw_fun = Undefind()
-            raw_result = Undefind()
-            exc_info = Undefind()
-            final_result = Undefind()  # 用户可以自己定义final_result的值，如果定义了就把这个值作为函数的结果，否则把函数原始结果作为结果。
-        
-            def __call__(self, fun, *args, **kwargs):
-                # print(locals())
-                if not callable(fun) or args or kwargs:  # 正常是只有fun一个参数，除非是装饰器没加括号造成的。
-                    raise ValueError('为了简单和一致起见，所有装饰器都采用有参数装饰器，被装饰函数上面的装饰器后面别忘了加括号')
-                self.raw_fun = fun
-                f = functools.partial(BaseDecorator._execute, self)  # 比 self.execute 利于补全
-                functools.update_wrapper(f, fun, )
-                return f
-        
-            def _execute(self, *args, **kwargs):
-                self.before()
-                try:
-                    self.raw_result = self.raw_fun(*args, **kwargs)
-                    self.after()
-                except Exception as e:
-                    self.exc_info = sys.exc_info()
-                    self.when_exception()
-                if not isinstance(self.final_result, Undefind):  # 用户可以自己定义final_result的值，如果定义了就把这个值作为函数的结果。
-                    return self.final_result
-                else:
-                    return self.raw_result
-        
-            def before(self):
-                pass
-        
-            def after(self):
-                pass
-        
-            def when_exception(self):
-                # print(self.exc_info) # (<class 'ZeroDivisionError'>, ZeroDivisionError('division by zero',), <traceback object at 0x000001D22BA3FD48>)
-                raise self.exc_info[1]
-        
-        
-        if __name__ == '__main__':
-            import nb_log  # noqa
-        
-        
-            class MyDeco(BaseDecorator):
-                def __init__(self, a=5, b=6):
-                    self.a = a
-                    self.b = b
-        
-                def before(self):
-                    print('开始执行')
-        
-                # noinspection PyAttributeOutsideInit
-                def after(self):
-                    self.final_result = self.a * self.b * self.raw_result
-        
-        
-            def common_deco(a=5, b=6):
-                """  上面的逻辑如果用常规方式写"""
-        
-                def _inner(f):
-                    @functools.wraps(f)
-                    def __inner(*args, **kwargs):
-                        try:
-                            print('开始执行')
-                            result = f(*args, **kwargs)
-                            return a * b * result
-                        except Exception as e:
-                            raise e
-        
-                    return __inner
-        
-                return _inner
-        
-        
-            @MyDeco(b=4)
-            # @common_deco(b=4)
-            def fun3(x):
-                print(x)
-                return x * 2
-        
-        
-            print(type(fun3))
-            print(fun3)
-            print(fun3.__wrapped__)  # noqa
-            print(fun3(10))
-        
-        ```
 Keywords: base_decorator
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
+
+# base_decorator
+
+pip install base_decorator
+```
+通用的装饰器基类，使写装饰器变得更简单。
+```
+
+```python
+import functools
+import abc
+import sys
+
+
+class Undefind:
+    pass
+
+
+class BaseDecorator(metaclass=abc.ABCMeta):
+    """
+    简化了装饰器的编写。
+
+    用户的装饰器需要继承这个，用户可以按需重新定义 before，after，when_exception 方法。
+
+    为了一致性和省事，统一采用有参数装饰器，用户的装饰器后面必须带括号。
+
+
+    """
+
+    # def __init__(self, *args, **kwargs):
+    #     pass
+
+    raw_fun = Undefind()
+    raw_result = Undefind()
+    exc_info = Undefind()
+    final_result = Undefind()  # 用户可以自己定义final_result的值，如果定义了就把这个值作为函数的结果，否则把函数原始结果作为结果。
+
+    def __call__(self, fun, *args, **kwargs):
+        # print(locals())
+        if not callable(fun) or args or kwargs:  # 正常是只有fun一个参数，除非是装饰器没加括号造成的。
+            raise ValueError('为了简单和一致起见，所有装饰器都采用有参数装饰器，被装饰函数上面的装饰器后面别忘了加括号')
+        self.raw_fun = fun
+        f = functools.partial(BaseDecorator._execute, self)  # 比 self.execute 利于补全
+        functools.update_wrapper(f, fun, )
+        return f
+
+    def _execute(self, *args, **kwargs):
+        self.before()
+        try:
+            self.raw_result = self.raw_fun(*args, **kwargs)
+            self.after()
+        except Exception as e:
+            self.exc_info = sys.exc_info()
+            self.when_exception()
+        if not isinstance(self.final_result, Undefind):  # 用户可以自己定义final_result的值，如果定义了就把这个值作为函数的结果。
+            return self.final_result
+        else:
+            return self.raw_result
+
+    def before(self):
+        pass
+
+    def after(self):
+        pass
+
+    def when_exception(self):
+        # print(self.exc_info) # (<class 'ZeroDivisionError'>, ZeroDivisionError('division by zero',), <traceback object at 0x000001D22BA3FD48>)
+        raise self.exc_info[1]
+
+
+if __name__ == '__main__':
+    import nb_log  # noqa
+
+
+    class MyDeco(BaseDecorator):
+        def __init__(self, a=5, b=6):
+            self.a = a
+            self.b = b
+
+        def before(self):
+            print('开始执行')
+
+        # noinspection PyAttributeOutsideInit
+        def after(self):
+            self.final_result = self.a * self.b * self.raw_result
+
+
+    def common_deco(a=5, b=6):
+        """  上面的逻辑如果用常规方式写"""
+
+        def _inner(f):
+            @functools.wraps(f)
+            def __inner(*args, **kwargs):
+                try:
+                    print('开始执行')
+                    result = f(*args, **kwargs)
+                    return a * b * result
+                except Exception as e:
+                    raise e
+
+            return __inner
+
+        return _inner
+
+
+    @MyDeco(b=4)
+    # @common_deco(b=4)
+    def fun3(x):
+        print(x)
+        return x * 2
+
+
+    print(type(fun3))
+    print(fun3)
+    print(fun3.__wrapped__)  # noqa
+    print(fun3(10))
+    
+```
+
```

### Comparing `base_decorator-0.1/README.md` & `base_decorator-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # base_decorator
 
-
+pip install base_decorator
 ```
 通用的装饰器基类，使写装饰器变得更简单。
 ```
 
 ```python
 import functools
 import abc
@@ -109,9 +109,9 @@
         return x * 2
 
 
     print(type(fun3))
     print(fun3)
     print(fun3.__wrapped__)  # noqa
     print(fun3(10))
-
+    
 ```
```

### Comparing `base_decorator-0.1/setup.py` & `base_decorator-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # filepath = ((Path(__file__).parent / Path('README.md')).absolute()).as_posix()
 filepath = 'README.md'
 print(filepath)
 
 setup(
     name='base_decorator',  #
-    version="0.1",
+    version="0.2",
     description=( 'base_decorator,make decorator easy to write'),
     keywords=("base_decorator",  ),
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description= open(filepath, 'r',encoding='utf8').read(),
     # data_files=[filepath],
     author='bfzs',
@@ -42,13 +42,13 @@
     ]
 )
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
-python setup.py sdist & twine upload dist/base_decorator-0.1.tar.gz
+python setup.py sdist & twine upload dist/base_decorator-0.2.tar.gz
 twine upload dist/*
 
 
 python -m pip install base_decorator --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

