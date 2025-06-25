# 🧾 Employee Timesheet Analysis using PySpark + Databricks

## 📌 Project Summary

This project simulates a real-world IT company's employee timesheet tracking system and analyzes working patterns using **Apache Spark**, **Delta Lake**, and **Databricks notebooks**.

---

## 🛠 Tools & Tech Stack

- Apache Spark (PySpark)
- Databricks Community Edition
- Delta Lake (no DBFS dependency)
- SQL, Pandas, Matplotlib
- GitHub for version control

---

## 📁 Dataset Description

- `medium_employees.csv` – 50 employees with department and join date
- `medium_timesheets.csv` – 10-day work logs with hours and project name

---

## 🔄 Key Steps Performed

1. **Data Loading & Joining**
   - Loaded CSVs using Spark
   - Created SQL tables
   - Joined employee and timesheet data

2. **Data Processing**
   - Repartitioned data for performance
   - Converted columns, handled nulls
   - Cached working set for reuse

3. **Delta Table Handling**
   - Saved to Delta Lake
   - Queried using SQL in Unity Catalog
   - Applied `OPTIMIZE` and `ZORDER`

4. **Aggregation**
   - Total hours per employee
   - Avg hours by department
   - Total hours per project

5. **Visualization**
   - Bar chart for top employees
   - Pie chart for avg department hours

---

## 📊 Sample Output

![Bar Chart](./charts/emp_hours_chart.png)

---

## 📌 Learnings

- Partitioning and performance optimization
- Delta table lifecycle: write → optimize → vacuum
- Simulating cloud-scale pipelines in Databricks

---

## 📁 Folder Structure

