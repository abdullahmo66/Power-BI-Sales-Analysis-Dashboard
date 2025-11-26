# 📊 Power BI Sales Analysis Dashboard

This repository contains a **Power BI interactive dashboard** designed
to analyze sales performance across multiple dimensions, including
customers, products, territories, and time.

## 🚀 Features

### ✔ Key Metrics

-   Total Sales\
-   Total Profit\
-   Total Quantity\
-   KPI indicators for performance tracking\
-   Year-over-Year comparison

### ✔ Visual Insights

-   Trend analysis over time\
-   Profit and sales by territory\
-   Top & bottom performing products\
-   Customer segmentation\
-   Dynamic slicers for flexible filtering

## 🛠 Data Modeling

The model follows a **Star Schema** and includes:

-   **Fact Table**
    -   Sales (SalesAmount, Profit, Quantity, Dates, ProductID,
        CustomerID, TerritoryID)
-   **Dimension Tables**
    -   DimProduct\
    -   DimCustomer\
    -   DimTerritory (TerritoryID, Territory, TerritoryGroup)\
    -   DimDate

## 📘 DAX Measures (Examples)

    Total Sales = SUM(Sales[SalesAmount])

    Total Profit = SUM(Sales[Profit])

    Total Quantity = SUM(Sales[OrderQuantity])

    Sales KPI = 
    IF([Total Sales] >= [Sales Target], "On Track", "Below Target")

## 📂 File Contents

  -----------------------------------------------------------------------
  File                   Description
  ---------------------- ------------------------------------------------
  **Session6\_.pbix**    Power BI report containing all visuals, KPIs,
                         and data modeling

  -----------------------------------------------------------------------

## 📥 How to Use

1.  Download the `.pbix` file\
2.  Open it in **Power BI Desktop**\
3.  Refresh data if required\
4.  Explore the interactive visuals

## 🤝 Contributions

Open to suggestions and improvements.

## 📄 License

MIT License
