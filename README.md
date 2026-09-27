# Premium-MotoSales-Dashboard-Power-BI
A moto themed Power BI dashboard analyzing premium two-wheeler brand performance — pricing strategy, market expansion, seasonal demand, and warranty risk across 10 brands and 10 countries

# Two-Wheeler Premium Brands — Power BI Dashboard

A moto themed Power BI report analyzing premium two-wheeler brand performance (BMW Motorrad, Ducati, Harley-Davidson, Triumph, KTM, Kawasaki, Aprilia, MV Agusta, Indian Motorcycle, Honda Premium) across 2022–2026 and 10 countries. Built on a star-schema data model, in INR, with fully custom moto-themed styling.

## Key DAX Measures

DAX
Total Revenue = SUMX(Fact_Sales, Fact_Sales[Net_Amount_INR])
Total Units Sold = SUM(Fact_Sales[Quantity_Sold])
Market Share % = DIVIDE([Total Units Sold], CALCULATE([Total Units Sold], ALL(Dim_Product[Brand_Name])))


## Business Problems Solved

- **Pricing strategy** — flags brands/models priced too high or too low relative to customer satisfaction
- **Market expansion** — highlights high-demand, high-satisfaction countries worth prioritizing
- **Seasonal planning** — quarterly demand heatmap by country for production/inventory decisions
- **Growth targeting** — direct action list of underexploited high-rating, low-share products

## 📌 Note

All underlying data is synthetically generated for portfolio/practice purposes and does not represent real sales, customers, or dealership data.
