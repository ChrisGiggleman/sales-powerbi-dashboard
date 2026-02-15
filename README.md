# Sales Performance Dashboard (Power BI)

## Overview

This project demonstrates building an interactive sales analytics dashboard using Power BI.

The dashboard provides insights into:

* Revenue trends over time
* Revenue by region
* Revenue by product
* Top customers by revenue
* Average order value (AOV)

This project demonstrates skills in:

* Data modeling
* DAX measures
* Interactive dashboard design
* Business KPI visualization

---

## Dataset

The dataset contains simulated sales data including:

* OrderID
* Date
* Customer
* Region
* Product
* Quantity
* Price

---

## Data Model

A calculated column is used to compute revenue:

```
revenue = [Quantity] * [Price]
```

---

## DAX Measures

Total Revenue

```
Total Revenue = SUM(Sheet1[revenue])
```

Total Orders

```
Total Orders = DISTINCTCOUNT(Sheet1[OrderID])
```

Total Quantity

```
Total Quantity = SUM(Sheet1[Quantity])
```

Average Order Value

```
AOV = DIVIDE([Total Revenue], [Total Orders])
```

---

## Dashboard Features

The dashboard includes:

* Region slicer
* Date range filter
* Revenue KPI card
* Revenue trend chart
* Revenue by region chart
* Revenue by product chart
* Top customer visualization
* Average order value KPI

---

## Screenshot

![Dashboard](screenshots/dashboard.png)

---

## Tools Used

* Power BI Desktop
* Excel
* DAX

---

## Author

Christopher Giggleman
