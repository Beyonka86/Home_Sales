# 🏠 **Home Sales Analysis**

### 📘 Module 22 Assignment Instructions

### ✅ Step-by-Step Tasks:

1. **Rename Notebook**

   * Rename `Home_Sales_starter_code.ipynb` to `Home_Sales.ipynb`.

2. **Import Required Libraries**

   * Import all necessary **PySpark SQL functions** to perform data transformations and queries.

3. **Load the Dataset**

   * Read the `home_sales_revised.csv` file into a **Spark DataFrame**.

4. **Create a Temporary Table**

   * Register the DataFrame as a **temporary view** named `home_sales` using `.createOrReplaceTempView()`.

---

### 🔎 SparkSQL Queries (Answer the following):

5. **Average Price of 4-Bedroom Homes by Year**

   * Calculate the **average sale price** for homes with 4 bedrooms grouped by **year sold**.
   * Round the results to **two decimal places**.

6. **Average Price by Year for 3 Bed / 3 Bath Homes**

   * Find the **average sale price** for homes built each year with **3 bedrooms and 3 bathrooms**.
   * Round to two decimal places.

7. **Filtered Average Price by Size and Features**

   * For homes with **3 bedrooms, 3 bathrooms, 2 floors**, and **≥ 2,000 sqft**, calculate the **average price** by year built.
   * Round to two decimal places.

8. **View Rating vs. Average Price**

   * Determine the **average home price per "view" rating** where the **average price is ≥ \$350,000**.
   * Measure and report the **query runtime**.
   * Round average prices to two decimal places.

---

### ⚡ Caching & Performance Optimization:

9. **Cache the Temporary Table**

   * Cache the `home_sales` temporary table.

10. **Verify Cache**

* Confirm that the table is successfully cached using PySpark.

11. **Re-run Query with Cache**

* Re-execute the query from Step 8 using the **cached data**.
* Measure and compare the **runtime** to the uncached version.

---

### 📦 Parquet and Partitioning:

12. **Partition Data by Year Built**

* Save the formatted home sales data as **Parquet**, partitioned by the `date_built` field.

13. **Create Temporary Table from Parquet**

* Register the partitioned Parquet data as a **new temporary view**.

14. **Re-run View Rating Query on Partitioned Data**

* Run the same **"view" rating average price query** again.
* Record and compare **runtime performance**.

---

### 🧹 Cleanup:

15. **Uncache Table**

* Uncache the `home_sales` temporary table.

16. **Verify Uncache**

* Use PySpark to confirm that the table has been uncached.

---
