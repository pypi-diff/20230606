# Comparing `tmp/spoiltracker-0.0.7.tar.gz` & `tmp/spoiltracker-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spoiltracker-0.0.7.tar", last modified: Tue Jun  6 17:00:16 2023, max compression
+gzip compressed data, was "spoiltracker-0.0.8.tar", last modified: Tue Jun  6 17:08:39 2023, max compression
```

## Comparing `spoiltracker-0.0.7.tar` & `spoiltracker-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-06 17:00:16.425579 spoiltracker-0.0.7/
--rw-r--r--   0 bloom      (501) staff       (20)     1044 2023-06-06 15:14:11.000000 spoiltracker-0.0.7/LICENSE
--rw-r--r--   0 bloom      (501) staff       (20)    10148 2023-06-06 17:00:16.425404 spoiltracker-0.0.7/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)     9559 2023-06-06 16:50:05.000000 spoiltracker-0.0.7/README.md
--rw-r--r--   0 bloom      (501) staff       (20)      509 2023-06-06 14:31:24.000000 spoiltracker-0.0.7/pyproject.toml
--rw-r--r--   0 bloom      (501) staff       (20)       38 2023-06-06 17:00:16.425615 spoiltracker-0.0.7/setup.cfg
--rw-r--r--   0 bloom      (501) staff       (20)      830 2023-06-06 16:05:07.000000 spoiltracker-0.0.7/setup.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-06 17:00:16.422738 spoiltracker-0.0.7/src/
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-06 17:00:16.425238 spoiltracker-0.0.7/src/spoiltracker.egg-info/
--rw-r--r--   0 bloom      (501) staff       (20)    10148 2023-06-06 17:00:16.000000 spoiltracker-0.0.7/src/spoiltracker.egg-info/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)      201 2023-06-06 17:00:16.000000 spoiltracker-0.0.7/src/spoiltracker.egg-info/SOURCES.txt
--rw-r--r--   0 bloom      (501) staff       (20)        1 2023-06-06 17:00:16.000000 spoiltracker-0.0.7/src/spoiltracker.egg-info/dependency_links.txt
--rw-r--r--   0 bloom      (501) staff       (20)        1 2023-06-06 17:00:16.000000 spoiltracker-0.0.7/src/spoiltracker.egg-info/top_level.txt
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-06 17:08:39.161816 spoiltracker-0.0.8/
+-rw-r--r--   0 bloom      (501) staff       (20)     1044 2023-06-06 15:14:11.000000 spoiltracker-0.0.8/LICENSE
+-rw-r--r--   0 bloom      (501) staff       (20)    10092 2023-06-06 17:08:39.161675 spoiltracker-0.0.8/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)     9503 2023-06-06 17:06:31.000000 spoiltracker-0.0.8/README.md
+-rw-r--r--   0 bloom      (501) staff       (20)      509 2023-06-06 17:08:15.000000 spoiltracker-0.0.8/pyproject.toml
+-rw-r--r--   0 bloom      (501) staff       (20)       38 2023-06-06 17:08:39.161855 spoiltracker-0.0.8/setup.cfg
+-rw-r--r--   0 bloom      (501) staff       (20)      830 2023-06-06 17:08:03.000000 spoiltracker-0.0.8/setup.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-06 17:08:39.160416 spoiltracker-0.0.8/src/
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-06-06 17:08:39.161524 spoiltracker-0.0.8/src/spoiltracker.egg-info/
+-rw-r--r--   0 bloom      (501) staff       (20)    10092 2023-06-06 17:08:39.000000 spoiltracker-0.0.8/src/spoiltracker.egg-info/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)      201 2023-06-06 17:08:39.000000 spoiltracker-0.0.8/src/spoiltracker.egg-info/SOURCES.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        1 2023-06-06 17:08:39.000000 spoiltracker-0.0.8/src/spoiltracker.egg-info/dependency_links.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        1 2023-06-06 17:08:39.000000 spoiltracker-0.0.8/src/spoiltracker.egg-info/top_level.txt
```

### Comparing `spoiltracker-0.0.7/LICENSE` & `spoiltracker-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spoiltracker-0.0.7/PKG-INFO` & `spoiltracker-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,108 +1,108 @@
 Metadata-Version: 2.1
 Name: spoiltracker
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Simple Expiry Management System
 Home-page: https://github.com/psibir/spoiltracker
 Author: psibir
 Author-email: Trevor Bloomfield <bloomfieldtm@gmail.com>
 Project-URL: Homepage, https://github.com/psibir/spoiltracker
 Project-URL: Bug Tracker, https://github.com/psibir/spoilertracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SpoilTracker
+# spoiltracker
 
 ![spoiltracker logo](/spoiltracker_logo.png)
 
-SpoilTracker is a Python package that helps track the expiration dates of products. It calculates expiration dates based on the production dates and shelf life information and generates an expiry report for products that are approaching their expiration dates. It also allows removing expired entries from the history file and clearing the history file.
+Spoiltracker is a Python package that helps track the expiration dates of products. It calculates expiration dates based on the production dates and shelf life information and generates an expiry report for products that are approaching their expiration dates.
 
 ## Simple Product Expiry Management
 
-SpoilTracker is useful for businesses that deal with perishable products and need to keep track of their expiration dates. It can be used in various industries such as food and beverage, agriculture, perishable goods logistics, warehousing, pharmaceuticals, and cosmetics. The package helps businesses to:
+Spoiltracker is useful for businesses that deal with perishable products and need to keep track of their expiration dates. It can be used in various industries such as food and beverage, agriculture, perishable goods logistics, warehousing, pharmaceuticals, and cosmetics. The package helps businesses to:
 
 - Maintain a record of product SKUs, names, brands, and expiration dates.
 - Calculate expiration dates based on the production dates and shelf life information.
 - Generate an expiry report that lists products approaching their expiration dates within a specified number of days.
 - Remove expired entries from the history file to keep the record up to date.
 - Clear the history file when necessary.
 
 ## Business Use Case: Deli and Cheese Counters Spoilage Mitigation
 
-SpoilTracker is a valuable tool for businesses operating deli and cheese counters, as well as any industry where spoilage mitigation is crucial. It helps track the expiration dates of perishable products, such as deli meats, cheeses, and other fresh foods, allowing businesses to effectively manage inventory, reduce waste, and ensure product quality and safety.
+Spoiltracker is a valuable tool for deli and cheese counters, as well as any industry where spoilage mitigation is crucial. It helps track the expiration dates of perishable products, such as deli meats, cheeses, and other fresh foods, allowing businesses to effectively manage inventory, reduce waste, and ensure product quality and safety.
 
-By utilizing SpoilTracker in deli and cheese counters, businesses can:
+By utilizing Spoiltracker in deli and cheese counters, businesses can:
 
-- Optimize inventory management: SpoilTracker enables businesses to keep a record of products along with their production dates and shelf life information. This helps deli and cheese counter managers to efficiently manage their inventory by identifying products that are approaching their expiration dates. By staying proactive, managers can ensure that products are used or sold before they spoil, reducing waste and optimizing stock levels.
+- Optimize inventory management: Spoiltracker enables businesses to keep a record of products along with their production dates and shelf life information. This helps deli and cheese counter managers to efficiently manage their inventory by identifying products that are approaching their expiration dates. By staying proactive, managers can ensure that products are used or sold before they spoil, reducing waste and optimizing stock levels.
 
-- Minimize spoilage and waste: SpoilTracker assists in identifying products that are close to their expiration dates. With the generated expiry reports based on specified criteria, such as the number of days until expiration, businesses can take proactive measures to minimize spoilage and waste. This can include implementing promotional activities, such as discounts or special offers, to encourage customers to purchase products before they expire.
+- Minimize spoilage and waste: Spoiltracker assists in identifying products that are close to their expiration dates. With the generated expiry reports based on specified criteria, such as the number of days until expiration, businesses can take proactive measures to minimize spoilage and waste. This can include implementing promotional activities, such as discounts or special offers, to encourage customers to purchase products before they expire.
 
-- Ensure product quality and safety: Maintaining accurate and up-to-date records of product expiration dates is crucial for ensuring product quality and safety. SpoilTracker allows businesses to monitor and manage expiration dates effectively, reducing the risk of serving or selling expired products to customers. By staying on top of product freshness, businesses can enhance customer satisfaction and reputation.
+- Ensure product quality and safety: Maintaining accurate and up-to-date records of product expiration dates is crucial for ensuring product quality and safety. Spoiltracker allows businesses to monitor and manage expiration dates effectively, reducing the risk of serving or selling expired products to customers. By staying on top of product freshness, businesses can enhance customer satisfaction and reputation.
 
-- Streamline operations: SpoilTracker streamlines the process of managing product expiration dates. With its ability to remove expired entries from the history file and clear the history file, businesses can maintain a clean and organized record of products. This streamlines operations, making it easier for deli and cheese counter staff to access information, plan for product usage, and maintain compliance with food safety regulations.
+- Streamline operations: Spoiltracker streamlines the process of managing product expiration dates. With its ability to remove expired entries from the history file and clear the history file, businesses can maintain a clean and organized record of products. This streamlines operations, making it easier for deli and cheese counter staff to access information, plan for product usage, and maintain compliance with food safety regulations.
 
 ## Installation
 
 The package can be installed using pip:
 
 ```shell
 pip install spoiltracker
 ```
 
 ## Usage
 
-SpoilTracker can be used from the command line or integrated into other Python scripts.
+Spoiltracker can be used from the command line or integrated into other Python scripts.
 
 ### Command Line Usage
 
-To use SpoilTracker from the command line, run the following command:
+To use Spoiltracker from the command line, run the following command:
 
 ```shell
 python -m spoiltracker [csv_file] [production_date] [--days DAYS] [--remove-expired] [--expiry-report-dest FILE] [--clear-history]
 ```
 
-- `[csv_file]` (optional): The path to the CSV file containing the product data. If not provided, SpoilTracker will generate an expiry report based on the existing history file.
-- `[production_date]` (optional): The production date in the format "YYYY-MM-DD". If not provided, SpoilTracker will generate an expiry report based on the existing history file.
+- `[csv_file]` (optional): The path to the CSV file containing the product data. If not provided, Spoiltracker will generate an expiry report based on the existing history file.
+- `[production_date]` (optional): The production date in the format "YYYY-MM-DD". If not provided, Spoiltracker will generate an expiry report based on the existing history file.
 - `--days DAYS` (optional): The threshold for the number of days until expiration. Default is 3 days.
 - `--remove-expired` (optional): Flag to remove expired entries from the history file and clear the expiry report file.
 - `--expiry-report-dest FILE` (optional): Destination file for the expiry report. If not provided, the default file "expiryreport.csv" will be used.
 - `--clear-history` (optional): Flag to clear the history file.
 
 ### Python Script Integration
 
-To use SpoilTracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
+To use Spoiltracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
 
 ```python
 from spoiltracker import ExpiryTracker
 
 expiry_tracker = ExpiryTracker()
 expiry_tracker.run(csv_file="sku_list.csv", production_date="2023-06-01", days=5, remove_expired=True)
 ```
 
 ### Shelf Life Data
 
-SpoilTracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the same directory as the script or package using SpoilTracker. The file should have the following columns: SKU, Name, Brand, Shelf Life (in days).
+Spoiltracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the same directory as the script or package using Spoiltracker. The file should have the following columns: SKU, Name, Brand, Shelf Life (in days).
 
 ```csv
 SKU,Name,Brand,Shelf Life
 123,Product 1,Brand 1,10
 456,Product 2,Brand 2,7
 ```
 
 You can customize the shelf life file path by providing it when creating an instance of `ExpiryTracker`.
 
 ```python
 expiry_tracker = ExpiryTracker(shelf_life_file="custom_shelflife.csv")
 ```
 
-# Functions
+## Functions
 
 - Load Shelf Life Data:
   - The script automatically loads the shelf life data from the `shelflife.csv` file.
 
 - Process CSV File:
   - Specify the input CSV file and the production date using the `--csv-file` and `--production-date` options.
   - The script calculates the expiration dates for the products and writes the data to the history file.
@@ -118,15 +118,15 @@
 - Clear History File:
   - Use the `--clear-history` option to clear the history file.
 
 By running the script with different combinations of these functionalities and adjusting the command-line options accordingly, you can effectively manage product expiration dates, generate reports, and maintain an up-to-date history of your products.
 
 ## Methods
 
-SpoilTracker provides the following functionality:
+Spoiltracker provides the following functionality:
 
 ### Load Shelf Life Data
 
 The `load_shelf_life_data` method loads the shelf life data from the shelf life file. It
 
  reads the CSV file and stores the data in memory for later use.
 
@@ -160,12 +160,16 @@
 
 ### Process CSV
 
 The `process_csv` method processes the provided CSV file and generates the history data. It reads the CSV file, retrieves the shelf life information for each SKU, calculates the expiration dates, and writes the data to the history file. It returns the history data.
 
 ### Run
 
-The `run` method is the main entry point for using SpoilTracker. It accepts command line arguments or direct parameters and executes the necessary functions based on the provided options.
+The `run` method is the main entry point for using Spoiltracker. It accepts command line arguments or direct parameters and executes the necessary functions based on the provided options.
 
-## Error Handling
+### Error Handling
 
-SpoilTracker provides basic error handling for file not found errors and invalid date formats. If the shelf life file, history file, or expiry report file is not found, an error message is displayed. If an invalid date format is encountered in the CSV files, an error message is displayed as well.
+Spoiltracker provides basic error handling for file not found errors and invalid date formats. If the shelf life file, history file, or expiry report file is not found, an error message is displayed. If an invalid date format is encountered in the CSV files, an error message is displayed as well.
+
+## Contributions
+
+See [Contributions](/CONTRIBUTIONS).
```

### Comparing `spoiltracker-0.0.7/README.md` & `spoiltracker-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-# SpoilTracker
+# spoiltracker
 
 ![spoiltracker logo](/spoiltracker_logo.png)
 
-SpoilTracker is a Python package that helps track the expiration dates of products. It calculates expiration dates based on the production dates and shelf life information and generates an expiry report for products that are approaching their expiration dates. It also allows removing expired entries from the history file and clearing the history file.
+Spoiltracker is a Python package that helps track the expiration dates of products. It calculates expiration dates based on the production dates and shelf life information and generates an expiry report for products that are approaching their expiration dates.
 
 ## Simple Product Expiry Management
 
-SpoilTracker is useful for businesses that deal with perishable products and need to keep track of their expiration dates. It can be used in various industries such as food and beverage, agriculture, perishable goods logistics, warehousing, pharmaceuticals, and cosmetics. The package helps businesses to:
+Spoiltracker is useful for businesses that deal with perishable products and need to keep track of their expiration dates. It can be used in various industries such as food and beverage, agriculture, perishable goods logistics, warehousing, pharmaceuticals, and cosmetics. The package helps businesses to:
 
 - Maintain a record of product SKUs, names, brands, and expiration dates.
 - Calculate expiration dates based on the production dates and shelf life information.
 - Generate an expiry report that lists products approaching their expiration dates within a specified number of days.
 - Remove expired entries from the history file to keep the record up to date.
 - Clear the history file when necessary.
 
 ## Business Use Case: Deli and Cheese Counters Spoilage Mitigation
 
-SpoilTracker is a valuable tool for businesses operating deli and cheese counters, as well as any industry where spoilage mitigation is crucial. It helps track the expiration dates of perishable products, such as deli meats, cheeses, and other fresh foods, allowing businesses to effectively manage inventory, reduce waste, and ensure product quality and safety.
+Spoiltracker is a valuable tool for deli and cheese counters, as well as any industry where spoilage mitigation is crucial. It helps track the expiration dates of perishable products, such as deli meats, cheeses, and other fresh foods, allowing businesses to effectively manage inventory, reduce waste, and ensure product quality and safety.
 
-By utilizing SpoilTracker in deli and cheese counters, businesses can:
+By utilizing Spoiltracker in deli and cheese counters, businesses can:
 
-- Optimize inventory management: SpoilTracker enables businesses to keep a record of products along with their production dates and shelf life information. This helps deli and cheese counter managers to efficiently manage their inventory by identifying products that are approaching their expiration dates. By staying proactive, managers can ensure that products are used or sold before they spoil, reducing waste and optimizing stock levels.
+- Optimize inventory management: Spoiltracker enables businesses to keep a record of products along with their production dates and shelf life information. This helps deli and cheese counter managers to efficiently manage their inventory by identifying products that are approaching their expiration dates. By staying proactive, managers can ensure that products are used or sold before they spoil, reducing waste and optimizing stock levels.
 
-- Minimize spoilage and waste: SpoilTracker assists in identifying products that are close to their expiration dates. With the generated expiry reports based on specified criteria, such as the number of days until expiration, businesses can take proactive measures to minimize spoilage and waste. This can include implementing promotional activities, such as discounts or special offers, to encourage customers to purchase products before they expire.
+- Minimize spoilage and waste: Spoiltracker assists in identifying products that are close to their expiration dates. With the generated expiry reports based on specified criteria, such as the number of days until expiration, businesses can take proactive measures to minimize spoilage and waste. This can include implementing promotional activities, such as discounts or special offers, to encourage customers to purchase products before they expire.
 
-- Ensure product quality and safety: Maintaining accurate and up-to-date records of product expiration dates is crucial for ensuring product quality and safety. SpoilTracker allows businesses to monitor and manage expiration dates effectively, reducing the risk of serving or selling expired products to customers. By staying on top of product freshness, businesses can enhance customer satisfaction and reputation.
+- Ensure product quality and safety: Maintaining accurate and up-to-date records of product expiration dates is crucial for ensuring product quality and safety. Spoiltracker allows businesses to monitor and manage expiration dates effectively, reducing the risk of serving or selling expired products to customers. By staying on top of product freshness, businesses can enhance customer satisfaction and reputation.
 
-- Streamline operations: SpoilTracker streamlines the process of managing product expiration dates. With its ability to remove expired entries from the history file and clear the history file, businesses can maintain a clean and organized record of products. This streamlines operations, making it easier for deli and cheese counter staff to access information, plan for product usage, and maintain compliance with food safety regulations.
+- Streamline operations: Spoiltracker streamlines the process of managing product expiration dates. With its ability to remove expired entries from the history file and clear the history file, businesses can maintain a clean and organized record of products. This streamlines operations, making it easier for deli and cheese counter staff to access information, plan for product usage, and maintain compliance with food safety regulations.
 
 ## Installation
 
 The package can be installed using pip:
 
 ```shell
 pip install spoiltracker
 ```
 
 ## Usage
 
-SpoilTracker can be used from the command line or integrated into other Python scripts.
+Spoiltracker can be used from the command line or integrated into other Python scripts.
 
 ### Command Line Usage
 
-To use SpoilTracker from the command line, run the following command:
+To use Spoiltracker from the command line, run the following command:
 
 ```shell
 python -m spoiltracker [csv_file] [production_date] [--days DAYS] [--remove-expired] [--expiry-report-dest FILE] [--clear-history]
 ```
 
-- `[csv_file]` (optional): The path to the CSV file containing the product data. If not provided, SpoilTracker will generate an expiry report based on the existing history file.
-- `[production_date]` (optional): The production date in the format "YYYY-MM-DD". If not provided, SpoilTracker will generate an expiry report based on the existing history file.
+- `[csv_file]` (optional): The path to the CSV file containing the product data. If not provided, Spoiltracker will generate an expiry report based on the existing history file.
+- `[production_date]` (optional): The production date in the format "YYYY-MM-DD". If not provided, Spoiltracker will generate an expiry report based on the existing history file.
 - `--days DAYS` (optional): The threshold for the number of days until expiration. Default is 3 days.
 - `--remove-expired` (optional): Flag to remove expired entries from the history file and clear the expiry report file.
 - `--expiry-report-dest FILE` (optional): Destination file for the expiry report. If not provided, the default file "expiryreport.csv" will be used.
 - `--clear-history` (optional): Flag to clear the history file.
 
 ### Python Script Integration
 
-To use SpoilTracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
+To use Spoiltracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
 
 ```python
 from spoiltracker import ExpiryTracker
 
 expiry_tracker = ExpiryTracker()
 expiry_tracker.run(csv_file="sku_list.csv", production_date="2023-06-01", days=5, remove_expired=True)
 ```
 
 ### Shelf Life Data
 
-SpoilTracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the same directory as the script or package using SpoilTracker. The file should have the following columns: SKU, Name, Brand, Shelf Life (in days).
+Spoiltracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the same directory as the script or package using Spoiltracker. The file should have the following columns: SKU, Name, Brand, Shelf Life (in days).
 
 ```csv
 SKU,Name,Brand,Shelf Life
 123,Product 1,Brand 1,10
 456,Product 2,Brand 2,7
 ```
 
 You can customize the shelf life file path by providing it when creating an instance of `ExpiryTracker`.
 
 ```python
 expiry_tracker = ExpiryTracker(shelf_life_file="custom_shelflife.csv")
 ```
 
-# Functions
+## Functions
 
 - Load Shelf Life Data:
   - The script automatically loads the shelf life data from the `shelflife.csv` file.
 
 - Process CSV File:
   - Specify the input CSV file and the production date using the `--csv-file` and `--production-date` options.
   - The script calculates the expiration dates for the products and writes the data to the history file.
@@ -102,15 +102,15 @@
 - Clear History File:
   - Use the `--clear-history` option to clear the history file.
 
 By running the script with different combinations of these functionalities and adjusting the command-line options accordingly, you can effectively manage product expiration dates, generate reports, and maintain an up-to-date history of your products.
 
 ## Methods
 
-SpoilTracker provides the following functionality:
+Spoiltracker provides the following functionality:
 
 ### Load Shelf Life Data
 
 The `load_shelf_life_data` method loads the shelf life data from the shelf life file. It
 
  reads the CSV file and stores the data in memory for later use.
 
@@ -144,12 +144,16 @@
 
 ### Process CSV
 
 The `process_csv` method processes the provided CSV file and generates the history data. It reads the CSV file, retrieves the shelf life information for each SKU, calculates the expiration dates, and writes the data to the history file. It returns the history data.
 
 ### Run
 
-The `run` method is the main entry point for using SpoilTracker. It accepts command line arguments or direct parameters and executes the necessary functions based on the provided options.
+The `run` method is the main entry point for using Spoiltracker. It accepts command line arguments or direct parameters and executes the necessary functions based on the provided options.
 
-## Error Handling
+### Error Handling
 
-SpoilTracker provides basic error handling for file not found errors and invalid date formats. If the shelf life file, history file, or expiry report file is not found, an error message is displayed. If an invalid date format is encountered in the CSV files, an error message is displayed as well.
+Spoiltracker provides basic error handling for file not found errors and invalid date formats. If the shelf life file, history file, or expiry report file is not found, an error message is displayed. If an invalid date format is encountered in the CSV files, an error message is displayed as well.
+
+## Contributions
+
+See [Contributions](/CONTRIBUTIONS).
```

### Comparing `spoiltracker-0.0.7/setup.py` & `spoiltracker-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "spoiltracker",
-    version = "0.0.7",
+    version = "0.0.8",
     author = "psibir",
     author_email = "bloomfieldtm@gmail.com",
     description = "Simple Product Expiry Management",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/psibir/spoiltracker",
     project_urls = {
```

### Comparing `spoiltracker-0.0.7/src/spoiltracker.egg-info/PKG-INFO` & `spoiltracker-0.0.8/src/spoiltracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,108 +1,108 @@
 Metadata-Version: 2.1
 Name: spoiltracker
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Simple Expiry Management System
 Home-page: https://github.com/psibir/spoiltracker
 Author: psibir
 Author-email: Trevor Bloomfield <bloomfieldtm@gmail.com>
 Project-URL: Homepage, https://github.com/psibir/spoiltracker
 Project-URL: Bug Tracker, https://github.com/psibir/spoilertracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# SpoilTracker
+# spoiltracker
 
 ![spoiltracker logo](/spoiltracker_logo.png)
 
-SpoilTracker is a Python package that helps track the expiration dates of products. It calculates expiration dates based on the production dates and shelf life information and generates an expiry report for products that are approaching their expiration dates. It also allows removing expired entries from the history file and clearing the history file.
+Spoiltracker is a Python package that helps track the expiration dates of products. It calculates expiration dates based on the production dates and shelf life information and generates an expiry report for products that are approaching their expiration dates.
 
 ## Simple Product Expiry Management
 
-SpoilTracker is useful for businesses that deal with perishable products and need to keep track of their expiration dates. It can be used in various industries such as food and beverage, agriculture, perishable goods logistics, warehousing, pharmaceuticals, and cosmetics. The package helps businesses to:
+Spoiltracker is useful for businesses that deal with perishable products and need to keep track of their expiration dates. It can be used in various industries such as food and beverage, agriculture, perishable goods logistics, warehousing, pharmaceuticals, and cosmetics. The package helps businesses to:
 
 - Maintain a record of product SKUs, names, brands, and expiration dates.
 - Calculate expiration dates based on the production dates and shelf life information.
 - Generate an expiry report that lists products approaching their expiration dates within a specified number of days.
 - Remove expired entries from the history file to keep the record up to date.
 - Clear the history file when necessary.
 
 ## Business Use Case: Deli and Cheese Counters Spoilage Mitigation
 
-SpoilTracker is a valuable tool for businesses operating deli and cheese counters, as well as any industry where spoilage mitigation is crucial. It helps track the expiration dates of perishable products, such as deli meats, cheeses, and other fresh foods, allowing businesses to effectively manage inventory, reduce waste, and ensure product quality and safety.
+Spoiltracker is a valuable tool for deli and cheese counters, as well as any industry where spoilage mitigation is crucial. It helps track the expiration dates of perishable products, such as deli meats, cheeses, and other fresh foods, allowing businesses to effectively manage inventory, reduce waste, and ensure product quality and safety.
 
-By utilizing SpoilTracker in deli and cheese counters, businesses can:
+By utilizing Spoiltracker in deli and cheese counters, businesses can:
 
-- Optimize inventory management: SpoilTracker enables businesses to keep a record of products along with their production dates and shelf life information. This helps deli and cheese counter managers to efficiently manage their inventory by identifying products that are approaching their expiration dates. By staying proactive, managers can ensure that products are used or sold before they spoil, reducing waste and optimizing stock levels.
+- Optimize inventory management: Spoiltracker enables businesses to keep a record of products along with their production dates and shelf life information. This helps deli and cheese counter managers to efficiently manage their inventory by identifying products that are approaching their expiration dates. By staying proactive, managers can ensure that products are used or sold before they spoil, reducing waste and optimizing stock levels.
 
-- Minimize spoilage and waste: SpoilTracker assists in identifying products that are close to their expiration dates. With the generated expiry reports based on specified criteria, such as the number of days until expiration, businesses can take proactive measures to minimize spoilage and waste. This can include implementing promotional activities, such as discounts or special offers, to encourage customers to purchase products before they expire.
+- Minimize spoilage and waste: Spoiltracker assists in identifying products that are close to their expiration dates. With the generated expiry reports based on specified criteria, such as the number of days until expiration, businesses can take proactive measures to minimize spoilage and waste. This can include implementing promotional activities, such as discounts or special offers, to encourage customers to purchase products before they expire.
 
-- Ensure product quality and safety: Maintaining accurate and up-to-date records of product expiration dates is crucial for ensuring product quality and safety. SpoilTracker allows businesses to monitor and manage expiration dates effectively, reducing the risk of serving or selling expired products to customers. By staying on top of product freshness, businesses can enhance customer satisfaction and reputation.
+- Ensure product quality and safety: Maintaining accurate and up-to-date records of product expiration dates is crucial for ensuring product quality and safety. Spoiltracker allows businesses to monitor and manage expiration dates effectively, reducing the risk of serving or selling expired products to customers. By staying on top of product freshness, businesses can enhance customer satisfaction and reputation.
 
-- Streamline operations: SpoilTracker streamlines the process of managing product expiration dates. With its ability to remove expired entries from the history file and clear the history file, businesses can maintain a clean and organized record of products. This streamlines operations, making it easier for deli and cheese counter staff to access information, plan for product usage, and maintain compliance with food safety regulations.
+- Streamline operations: Spoiltracker streamlines the process of managing product expiration dates. With its ability to remove expired entries from the history file and clear the history file, businesses can maintain a clean and organized record of products. This streamlines operations, making it easier for deli and cheese counter staff to access information, plan for product usage, and maintain compliance with food safety regulations.
 
 ## Installation
 
 The package can be installed using pip:
 
 ```shell
 pip install spoiltracker
 ```
 
 ## Usage
 
-SpoilTracker can be used from the command line or integrated into other Python scripts.
+Spoiltracker can be used from the command line or integrated into other Python scripts.
 
 ### Command Line Usage
 
-To use SpoilTracker from the command line, run the following command:
+To use Spoiltracker from the command line, run the following command:
 
 ```shell
 python -m spoiltracker [csv_file] [production_date] [--days DAYS] [--remove-expired] [--expiry-report-dest FILE] [--clear-history]
 ```
 
-- `[csv_file]` (optional): The path to the CSV file containing the product data. If not provided, SpoilTracker will generate an expiry report based on the existing history file.
-- `[production_date]` (optional): The production date in the format "YYYY-MM-DD". If not provided, SpoilTracker will generate an expiry report based on the existing history file.
+- `[csv_file]` (optional): The path to the CSV file containing the product data. If not provided, Spoiltracker will generate an expiry report based on the existing history file.
+- `[production_date]` (optional): The production date in the format "YYYY-MM-DD". If not provided, Spoiltracker will generate an expiry report based on the existing history file.
 - `--days DAYS` (optional): The threshold for the number of days until expiration. Default is 3 days.
 - `--remove-expired` (optional): Flag to remove expired entries from the history file and clear the expiry report file.
 - `--expiry-report-dest FILE` (optional): Destination file for the expiry report. If not provided, the default file "expiryreport.csv" will be used.
 - `--clear-history` (optional): Flag to clear the history file.
 
 ### Python Script Integration
 
-To use SpoilTracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
+To use Spoiltracker in a Python script, you can import the `ExpiryTracker` class and create an instance of it. Then, call the `run` method with the desired parameters.
 
 ```python
 from spoiltracker import ExpiryTracker
 
 expiry_tracker = ExpiryTracker()
 expiry_tracker.run(csv_file="sku_list.csv", production_date="2023-06-01", days=5, remove_expired=True)
 ```
 
 ### Shelf Life Data
 
-SpoilTracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the same directory as the script or package using SpoilTracker. The file should have the following columns: SKU, Name, Brand, Shelf Life (in days).
+Spoiltracker requires shelf life data to calculate expiration dates. By default, it expects a CSV file named "shelflife.csv" in the same directory as the script or package using Spoiltracker. The file should have the following columns: SKU, Name, Brand, Shelf Life (in days).
 
 ```csv
 SKU,Name,Brand,Shelf Life
 123,Product 1,Brand 1,10
 456,Product 2,Brand 2,7
 ```
 
 You can customize the shelf life file path by providing it when creating an instance of `ExpiryTracker`.
 
 ```python
 expiry_tracker = ExpiryTracker(shelf_life_file="custom_shelflife.csv")
 ```
 
-# Functions
+## Functions
 
 - Load Shelf Life Data:
   - The script automatically loads the shelf life data from the `shelflife.csv` file.
 
 - Process CSV File:
   - Specify the input CSV file and the production date using the `--csv-file` and `--production-date` options.
   - The script calculates the expiration dates for the products and writes the data to the history file.
@@ -118,15 +118,15 @@
 - Clear History File:
   - Use the `--clear-history` option to clear the history file.
 
 By running the script with different combinations of these functionalities and adjusting the command-line options accordingly, you can effectively manage product expiration dates, generate reports, and maintain an up-to-date history of your products.
 
 ## Methods
 
-SpoilTracker provides the following functionality:
+Spoiltracker provides the following functionality:
 
 ### Load Shelf Life Data
 
 The `load_shelf_life_data` method loads the shelf life data from the shelf life file. It
 
  reads the CSV file and stores the data in memory for later use.
 
@@ -160,12 +160,16 @@
 
 ### Process CSV
 
 The `process_csv` method processes the provided CSV file and generates the history data. It reads the CSV file, retrieves the shelf life information for each SKU, calculates the expiration dates, and writes the data to the history file. It returns the history data.
 
 ### Run
 
-The `run` method is the main entry point for using SpoilTracker. It accepts command line arguments or direct parameters and executes the necessary functions based on the provided options.
+The `run` method is the main entry point for using Spoiltracker. It accepts command line arguments or direct parameters and executes the necessary functions based on the provided options.
 
-## Error Handling
+### Error Handling
 
-SpoilTracker provides basic error handling for file not found errors and invalid date formats. If the shelf life file, history file, or expiry report file is not found, an error message is displayed. If an invalid date format is encountered in the CSV files, an error message is displayed as well.
+Spoiltracker provides basic error handling for file not found errors and invalid date formats. If the shelf life file, history file, or expiry report file is not found, an error message is displayed. If an invalid date format is encountered in the CSV files, an error message is displayed as well.
+
+## Contributions
+
+See [Contributions](/CONTRIBUTIONS).
```

