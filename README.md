---

# 📊 **Car Sales Dashboard – Power BI Project**

*A Data Analytics & BI Dashboard for Sales Performance Tracking*

---

🔗 GitHub Repository: <a href ="https://github.com/Shibaditya00/Car-Sales-Analysis-using-Power-BI">Car Sales Analysis using Power BI</a>

---

Dataset: <a href="https://github.com/Shibaditya00/Car-Sales-Analysis-using-Power-BI/blob/main/Car%20Sales.xlsx">Dataset Link</a>

---

## 🛠️ **Project Overview**

This project focuses on building a fully interactive **Car Sales Dashboard** in **Power BI** for a car dealership company. The dashboard enables the business to monitor key sales metrics, analyze performance trends, and make data-driven decisions.
It converts raw car sales data into actionable insights using **data cleaning, DAX measures, time intelligence, KPIs, and dynamic visualizations**.

---

## 🎯 **Objectives**

* Provide a centralized dashboard to track **YTD, MTD, and YOY sales performance**.
* Create a **Calendar Table** to enable **time intelligence calculations**.
* Build business-relevant **KPIs** based on client requirements.
* Visualize trends in **pricing, car models, colors, body styles, and dealer regions**.
* Enable deep drill-down analysis through **interactive charts and detailed tables**.

---

## 🧹 **Data Preparation**

1. **Data Cleaning**

   * Removed duplicates, null values, and inconsistencies.
   * Standardized car model, body style, color, and region fields.
   * Converted text dates into proper date formats.

2. **Calendar Table Creation**

   * A dedicated Date Table was created using DAX.
   * Includes Year, Month and Week.
   * Enabled **Time Intelligence functions** for KPIs.

3. **Data Modeling**

   * Established star-schema relationships.
   * Fact Table: *Car Sales Data*
   * Dimension Tables: *Calendar, Car Model, Dealer Region, Color, Body Style*

---

## 📌 **KPI Requirements (Problem Statement 1)**

### **1. Sales Overview**

* **YTD Total Sales**
* **MTD Total Sales**
* **YOY Growth in Total Sales**
* **Difference between YTD vs PTYD Sales**

### **2. Average Price Analysis**

* **YTD Average Price**
* **MTD Average Price**
* **YOY Growth in Average Price**
* **Difference between YTD vs PTYD Avg Price**

### **3. Cars Sold Metrics**

* **YTD Cars Sold**
* **MTD Cars Sold**
* **YOY Growth in Cars Sold**
* **Difference between YTD vs PTYD Cars Sold**

These KPIs were built using advanced **DAX Measures** and **Time Intelligence Functions**, ensuring accurate comparisons across years and periods.

---

## 📈 **Visualization Requirements (Problem Statement 2)**

### **1. YTD Sales Weekly Trend**

* Line chart
* X-axis: Weeks
* Y-axis: Total Sales
* Shows weekly performance pattern and sales peaks.

### **2. YTD Sales by Body Style**

* Pie Chart
* Compares how each car body style contributes to total YTD sales.

### **3. YTD Sales by Color**

* Pie Chart
* Displays distribution of total sales based on car color.

### **4. YTD Cars Sold by Dealer Region**

* Map Visualization
* Highlights regional performance using geographic insights.

### **5. Company-Wise Sales Trend (Grid Table)**

* Table with company name + YTD sales
* Helps stakeholders review brand-wise performance.

### **6. Detailed Car Sales Table**

* Complete transaction-level data including:

  * Car Model
  * Body Style
  * Color
  * Dealer Region
  * Sales Amount
  * Date
  * Company
  * Customer details (optional if present)

---

## 🧮 **Key DAX Measures Created**

Some examples include:

* `YTD Total Sales = TOTALYTD(SUM('car_data'[Price ($)]), 'Calendar'[Date])`
* `MTD Total Sales = TOTALMTD(SUM('car_data'[Amount]), 'Calendar'[Date])`
* `YOY Sales Growth = ( [YTD Sales] - [PTYD Sales] ) / [PTYD Total Sales]`
* `YTD Avg Price = TOTALYTD([Avg Price], 'Calendar Table'[Date])`
* `YTD Cars Sold = TOTALYTD(COUNT(car_data[Car_ID]), 'Calendar'[Date])`

---

## 🖥️ **Dashboard Features**

* Fully interactive and filterable dashboard
* Dynamic KPIs: updates based on slicers (Year, Brand, Region, Body Style)
* Clean visual hierarchy and professional theme
* Ability to drill down into detailed transaction-level data
* Weekly, monthly, and yearly trend analysis

---

## 📸 Dashboard Screenshots

### Screenshot 1
https://github.com/Shibaditya00/Car-Sales-Analysis-using-Power-BI/blob/main/Screenshot%20(160).png
<img width="1647" height="924" alt="Screenshot (160)" src="https://github.com/user-attachments/assets/0c3cffec-f94a-4f00-986a-ab7499116890" />


### Screenshot 2
https://github.com/Shibaditya00/Car-Sales-Analysis-using-Power-BI/blob/main/Screenshot%20(161).png
<img width="1650" height="923" alt="Screenshot (161)" src="https://github.com/user-attachments/assets/b0532afa-8b41-4995-ad1f-6d3979b590ce" />



---

## 🚀 **Insights Generated**

* Identified top-performing **car body styles** and **colors**.
* Highlighted regions with highest and lowest sales.
* Analyzed yearly and monthly sales growth patterns.
* Found pricing trends across models and seasons.
* Revealed fluctuations in demand via weekly YTD trends.

---

## 🧾 **Conclusion**

The Car Sales Dashboard delivers a complete analytical solution for monitoring dealership performance. It empowers business leaders with **real-time KPIs**, **visual trends**, and **deep insights**, enabling faster and more informed decision-making.

---
