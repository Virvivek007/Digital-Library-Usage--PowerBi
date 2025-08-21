# 📊 Digital Library Usage Visualization (Power BI)

## 📌 Project Overview

This project analyzes **online library usage patterns** by students using **Power BI**.
The dashboard provides insights into which resources (eBooks, Journals, Videos) are most accessed, with filters for **department**, **resource type**, and **date**.

It helps educators and administrators track content usage, identify trends, and optimize digital library resources.

---

## 🎯 Objectives

* Track **resource usage frequency** across different formats.
* Identify **Top-5 most accessed resources**.
* Compare **department-wise access behavior**.
* Visualize **daily and monthly trends** of usage.

---

## 🗂️ Dataset

Sample dataset used for demonstration:

| Date       | Student\_ID | Resource Type | Department |
| ---------- | ----------- | ------------- | ---------- |
| 2025-07-01 | S101        | eBook         | CSE        |
| 2025-07-01 | S102        | Journal       | ECE        |
| 2025-07-02 | S103        | Video         | IT         |
| 2025-07-02 | S104        | Dataset       | ME         |

📌 Columns:

* **Date** – Access date
* **Student\_ID** – Unique student identifier
* **Resource Type** – Type of digital resource (eBook, Journal, Video, etc.)
* **Department** – Student’s academic department

---

## ⚙️ Functional Components

1. **Data Preparation**

   * Load access logs into Power BI
   * Clean and standardize resource type & department names
   * Build a Date table for time-based analysis

2. **DAX Measures**

   * `Accesses = COUNTROWS(FactAccess)`
   * `Distinct Users = DISTINCTCOUNT(FactAccess[Student_ID])`
   * `% Usage Share` for each resource type
   * `Top-5 Resources` using RANKX

3. **Visuals in Dashboard**

   * KPI Cards → Total Accesses, Distinct Users
   * Bar/Column Chart → Resource type usage frequency
   * Heatmap → Department vs Resource Type
   * Line Chart → Daily/Monthly usage trend
   * Top-5 Most Used Resources → Filtered Bar Chart

4. **Filters & Interactivity**

   * Slicers: Department, Resource Type, Date Range
   * Drillthrough for Department-specific usage details
   * Interactive tooltips for additional insights

---

## 🚀 Expected Output

An **interactive Power BI dashboard** showing:
✔ Department-wise and resource-type usage patterns
✔ Top-5 most accessed resources
✔ Daily and monthly usage trends
✔ Filter options by department and resource type

---

## 📷 Dashboard Preview

*https://github.com/Virvivek007/Digital-Library-Usage--PowerBi/blob/main/Dashboard_image.png*

---

## 🛠️ Tools & Technologies

* **Power BI Desktop** – Data modeling & visualization
* **DAX** – Calculations & measures
* **Excel/CSV** – Input dataset

---

## 📌 How to Use

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/Digital-Library-Usage-Visualization.git
   ```
2. Open the `.pbix` file in **Power BI Desktop**.
3. Load your own digital library logs (Excel/CSV).
4. Refresh the dashboard to see updated insights.

---

## 📈 Future Enhancements

* Add **User Type (Student/Faculty)** for segmentation
* Implement **Row-Level Security (RLS)** for department-specific views
* Deploy to **Power BI Service** with scheduled refresh

---

## 👨‍💻 Author

**Vivek Kumar Tiwari**

* 🎓 B.Sc. \[Hons] Computer Science & Data Analytics – IIT Patna
* 💻 Passionate about **Data Analytics, Visualization & Data Science**

