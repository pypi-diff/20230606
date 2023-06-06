# Comparing `tmp/qtgql-0.119.7.tar.gz` & `tmp/qtgql-0.119.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.119.7.tar", max compression
+gzip compressed data, was "qtgql-0.119.9.tar", max compression
```

## Comparing `qtgql-0.119.7.tar` & `qtgql-0.119.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1064 2023-06-05 12:12:53.216019 qtgql-0.119.7/LICENSE
--rw-r--r--   0        0        0     1805 2023-06-05 12:12:53.216019 qtgql-0.119.7/README.md
--rw-r--r--   0        0        0     4445 2023-06-05 12:13:20.364525 qtgql-0.119.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0        0 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/compiler/__init__.py
--rw-r--r--   0        0        0     1782 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/compiler/builtin_scalars.py
--rw-r--r--   0        0        0    13094 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/compiler/operation.py
--rw-r--r--   0        0        0     3940 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/compiler/template.py
--rw-r--r--   0        0        0     2167 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/config.py
--rw-r--r--   0        0        0     1246 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/cppref.py
--rw-r--r--   0        0        0       41 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/exceptions.py
--rw-r--r--   0        0        0     3187 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/graphql_ref.py
--rw-r--r--   0        0        0    18043 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/introspection.py
--rw-r--r--   0        0        0    12736 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/objecttype.py
--rw-r--r--   0        0        0        0 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/runtime/__init__.py
--rw-r--r--   0        0        0     1571 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/runtime/custom_scalars.py
--rw-r--r--   0        0        0      488 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0      536 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/config.jinja.hpp
--rw-r--r--   0        0        0     5016 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/macros.jinja.hpp
--rw-r--r--   0        0        0     4917 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0      816 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/schema.jinja.cpp
--rw-r--r--   0        0        0     4552 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0     1028 2023-06-05 12:12:53.228020 qtgql-0.119.7/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-06 13:37:08.285462 qtgql-0.119.9/LICENSE
+-rw-r--r--   0        0        0     1805 2023-06-06 13:37:08.285462 qtgql-0.119.9/README.md
+-rw-r--r--   0        0        0     4445 2023-06-06 13:37:29.057539 qtgql-0.119.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/compiler/__init__.py
+-rw-r--r--   0        0        0     1782 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/compiler/builtin_scalars.py
+-rw-r--r--   0        0        0    13094 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/compiler/operation.py
+-rw-r--r--   0        0        0     3940 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/compiler/template.py
+-rw-r--r--   0        0        0     2167 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0     1246 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/cppref.py
+-rw-r--r--   0        0        0       41 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/exceptions.py
+-rw-r--r--   0        0        0     3187 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/graphql_ref.py
+-rw-r--r--   0        0        0    18043 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/introspection.py
+-rw-r--r--   0        0        0    12771 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/objecttype.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/runtime/__init__.py
+-rw-r--r--   0        0        0     1571 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/runtime/custom_scalars.py
+-rw-r--r--   0        0        0      488 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0      536 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/config.jinja.hpp
+-rw-r--r--   0        0        0     5385 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/macros.jinja.hpp
+-rw-r--r--   0        0        0     5042 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0      816 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/schema.jinja.cpp
+-rw-r--r--   0        0        0     4552 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0     1028 2023-06-06 13:37:08.301462 qtgql-0.119.9/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.9/PKG-INFO
```

### Comparing `qtgql-0.119.7/LICENSE` & `qtgql-0.119.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/README.md` & `qtgql-0.119.9/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/pyproject.toml` & `qtgql-0.119.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.119.7"
+version = "0.119.9"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.119.7/qtgqlcodegen/cli.py` & `qtgql-0.119.9/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/compiler/builtin_scalars.py` & `qtgql-0.119.9/qtgqlcodegen/compiler/builtin_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/compiler/operation.py` & `qtgql-0.119.9/qtgqlcodegen/compiler/operation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/compiler/template.py` & `qtgql-0.119.9/qtgqlcodegen/compiler/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/config.py` & `qtgql-0.119.9/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/cppref.py` & `qtgql-0.119.9/qtgqlcodegen/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/graphql_ref.py` & `qtgql-0.119.9/qtgqlcodegen/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/introspection.py` & `qtgql-0.119.9/qtgqlcodegen/introspection.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/objecttype.py` & `qtgql-0.119.9/qtgqlcodegen/objecttype.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,22 +63,23 @@
 @define(slots=False)
 class QtGqlVariableDefinition(Generic[T], QtGqlBaseTypedNode):
     default_value: Optional[T] = UNSET
 
     def json_repr(self, attr_name: Optional[str] = None) -> str:
         if not attr_name:
             attr_name = self.name
+        attr_name += ".value()"  # unwrap optional
         if self.type.is_input_object_type:
-            return f"{attr_name}.value().to_json()"
+            return f"{attr_name}.to_json()"
         elif self.type.is_builtin_scalar:
-            return f"{attr_name}.value()"
+            return f"{attr_name}"
         elif enum_def := self.type.is_enum:
-            return f"Enums::{enum_def.map_name}::name_by_value({attr_name}.value())"
+            return f"Enums::{enum_def.map_name}::name_by_value({attr_name})"
         elif self.is_custom_scalar:
-            raise NotImplementedError
+            return f"{attr_name}.serialize()"
 
         raise NotImplementedError(f"{self.type} is not supported as an input type ATM")
 
 
 @define(slots=False)
 class BaseQtGqlFieldDefinition(QtGqlBaseTypedNode):
     description: Optional[str] = ""
```

### Comparing `qtgql-0.119.7/qtgqlcodegen/runtime/custom_scalars.py` & `qtgql-0.119.9/qtgqlcodegen/runtime/custom_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/templates/config.jinja.hpp` & `qtgql-0.119.9/qtgqlcodegen/templates/config.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/templates/macros.jinja.hpp` & `qtgql-0.119.9/qtgqlcodegen/templates/macros.jinja.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,22 @@
 
 if ({% if include_selection_check %}👉config_name👈.selections.contains("👉f.name👈") && {% endif %} !data.value("👉f.name👈").isNull()){
 {% if f.type.is_builtin_scalar %}
 auto new_👉f.name👈 = data.value("👉f.name👈").👉 f.type.is_builtin_scalar.from_json_convertor 👈;
 if (👉private_name👈 != new_👉f.name👈){
     👉fset_name👈(new_👉f.name👈);
 }
+{% elif f.type.is_custom_scalar %}
+auto new_👉f.name👈 = 👉 f.is_custom_scalar.type_name 👈();
+new_👉f.name👈.deserialize(data.value("👉f.name👈"));
+if (👉private_name👈 != new_👉f.name👈){
+    👉fset_name👈(new_👉f.name👈);
+}
 {% else %}
-throw "not implemented";
+throw qtgql::exceptions::NotImplementedError({"👉f.type👈 is not supporting updates ATM"});
 {% endif %}
 }
 {%- endmacro %}
 
 
 {% macro initialize_proxy_field(field) %}
 {%set instance_of_concrete -%}
@@ -112,22 +118,22 @@
 concrete
 {% else %}
 m_inst->👉field.definition.getter_name 👈()
 {% endif %}{% endset -%}
 
 {% if field.type.is_object_type  and field.type.is_optional() %}
 if (👉 instance_of_concrete 👈){
-👉field.private_name👈 = new 👉field.type_name👈(this, 👉 instance_of_concrete 👈);
+👉field.private_name👈 = new 👉field.type_name👈(this, 👉 instance_of_concrete 👈, metadata);
 }
 else{
 👉field.private_name👈 = nullptr;
 }
 {% elif field.type.is_object_type %}
-👉field.private_name👈 = new 👉field.type_name👈(this, 👉 instance_of_concrete 👈);
+👉field.private_name👈 = new 👉field.type_name👈(this, 👉 instance_of_concrete 👈, metadata);
 {% elif field.type.is_model.is_object_type %}
 auto init_list_👉 field.name 👈 =  std::make_unique<QList<👉field.narrowed_type.name👈*>>();
-for (const auto & node: 👉 instance_of_concrete 👈.value(OPERATION_ID)){
-init_list_👉 field.name 👈->append(new 👉field.narrowed_type.name👈(this, node));
+for (const auto & node: 👉 instance_of_concrete 👈.value(metadata.operation_id)){
+init_list_👉 field.name 👈->append(new 👉field.narrowed_type.name👈(this, node, metadata));
 }
 👉field.private_name👈 = new 👉 field.type_name 👈(this, std::move(init_list_👉 field.name 👈));
 {% endif %}
 {% endmacro %}
```

### Comparing `qtgql-0.119.7/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.119.9/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #pragma once
 #include "./schema.hpp"
 #include <qtgql/gqlwstransport/gqlwstransport.hpp>
 #include <QObject>
 
 namespace 👉 context.config.env_name 👈{
 namespace 👉context.ns👈{
-const auto OPERATION_ID = QUuid::fromString("👉 context.operation.operation_id👈");
 
 {% for t in context.operation.narrowed_types %}
 class 👉 t.name 👈: public QObject{
 /*
 👉 t.doc_fields 👈
  */
     Q_OBJECT
@@ -33,15 +32,17 @@
 👉ref_field.property_type👈 m_👉ref_field.name👈 = {};
 {% endfor %}
 {%- for model_field in t.models -%}
 👉 model_field.property_type 👈 m_👉model_field.name👈;
 {% endfor %}
 
 public:
-👉 t.name 👈(QObject* parent, const std::shared_ptr<👉 t.definition.name 👈> &inst ): m_inst{inst}, QObject::QObject(parent){
+👉 t.name 👈(QObject * parent,
+        const std::shared_ptr<👉 t.definition.name 👈> &inst,
+        qtgql::bases::OperationMetadata & metadata): m_inst{inst}, QObject::QObject(parent){
 {% for field in t.fields -%}
 👉 macros.initialize_proxy_field(field) 👈
 {# updates logic -#}
 connect(m_inst.get(), &👉context.schema_ns👈::👉t.definition.name👈::👉 field.definition.signal_name 👈, this,
         [&](){emit 👉 field.definition.signal_name 👈();});
 {% endfor %}
 }
@@ -70,56 +71,62 @@
 
 
 
 inline const QString &ENV_NAME() override{
     static const auto ret = QString("👉 context.config.env_name 👈");
     return ret;
     }
-
-inline const qtgql::bases::OperationMetadata & OPERATION_METADATA() override{
-auto static ret = qtgql::bases::OperationMetadata{
-        OPERATION_ID,
+inline const qtgql::bases::SelectionsConfig & SELECTIONS_CONFIG() override{
+    static auto ret = qtgql::bases::SelectionsConfig(
         {👉 context.operation.root_field.as_conf_string() 👈}
-};
-return ret;
-};
+    );
+    return ret;
+}
+
+
 public:
 👉 context.operation.name 👈(): qtgql::gqlwstransport::OperationHandlerABC(qtgql::gqlwstransport::GqlWsTrnsMsgWithID(qtgql::gqlwstransport::OperationPayload(
         {%- for line in context.operation.query.splitlines() %}"👉 line 👈"{% endfor -%}
-        ), OPERATION_ID)){};
+        ))){
+m_message_template.op_id = m_operation_id;
+};
 
 QTGQL_STATIC_MAKE_SHARED(👉 context.operation.name 👈)
 
-inline const QUuid &operation_id() const override{
-return OPERATION_ID;
+inline qtgql::bases::OperationMetadata operation_metadata() override{
+return qtgql::bases::OperationMetadata(operation_id());
+};
+
+
+inline const QUuid & operation_id() const override{
+return m_operation_id;
 }
 
 
 void on_next(const QJsonObject &message) override{
     if (!m_data && message.contains("data")){
         auto data = message.value("data").toObject();
+        auto metadata = operation_metadata();
         if (data.contains("👉 context.operation.root_field.definition.name 👈")){
 {%- set do_after_deserialized -%} 👉 macros.initialize_proxy_field(context.operation.root_field) 👈 {% endset -%}
             👉 macros.deserialize_field(context.operation.root_field.definition,
                                     "auto concrete", False,
-                                    "OPERATION_METADATA().selections",
-                                    "OPERATION_METADATA()",
+                                    "SELECTIONS_CONFIG()",
+                                    "metadata",
                                     do_after_deserialized,
                                     ) 👈
-        // initialize proxy
-
         }
     }
 }
 inline const 👉 context.operation.root_field.property_type 👈 get_data(){
     return m_data.value();
 }
-inline void loose(){
+inline void loose() override{
     {% if context.operation.root_field.type.is_object_type %}
-    👉 context.operation.root_field.type.is_object_type.name 👈::INST_STORE().get_node(m_data.value()->get_id()).value()->loose(OPERATION_METADATA());
+    👉 context.operation.root_field.type.is_object_type.name 👈::INST_STORE().get_node(m_data.value()->get_id()).value()->loose(operation_metadata());
     {% else %}
     throw "not implemented";
     {% endif %}
 }
 
 {% if context.operation.variables %}
 void set_variables(
```

### Comparing `qtgql-0.119.7/qtgqlcodegen/templates/schema.jinja.cpp` & `qtgql-0.119.9/qtgqlcodegen/templates/schema.jinja.cpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.119.9/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/qtgqlcodegen/utils.py` & `qtgql-0.119.9/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.7/PKG-INFO` & `qtgql-0.119.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.119.7
+Version: 0.119.9
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

