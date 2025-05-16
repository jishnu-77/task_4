# Visualization Documentation

## 1. Bar Chart: Total Profit by Country  
![Bar Chart](images/barchart.png)  

### Description  
This bar chart visualizes the total **Profit** (in thousands) for each **Country** in the dataset. The countries included are:  
- Canada  
- France  
- Germany  
- Mexico  
- United States of America  

### Key Insights  
- **Germany** and **Mexico** have the highest profits, driven by large-scale government and enterprise sales (e.g., high-value `Paseo` and `Velo` product sales in Germany).  
- **United States of America** shows moderate profits, primarily from midmarket and small business segments.  
- **Canada** has consistent profits across government and channel partner segments.  


## 2. Density Chart: Sales Distribution by Month-Year  
![Density Chart](images/densitychart.png)  

### Description  
This density chart illustrates the distribution of **Gross Sales** over time, aggregated by `MonthYear` (e.g., "April 2014"). The chart highlights periods with concentrated sales activity.  

### Key Insights  
- Peaks in **June 2014** and **December 2013**, driven by holiday season discounts and year-end deals (e.g., `Carretera` and `Montana` products with "Low" and "Medium" discount bands).  
- Lower activity in **September 2013** and **October 2013**, likely due to seasonal fluctuations.  
- A secondary spike in **August 2014**, attributed to enterprise sales in the United States and Mexico.  


## 3. Pie Chart: Total Sales by Country  
![Pie Chart](images/piechart.png)  

### Description  
This pie chart shows the proportional distribution of **Total Sales** (in thousands) across countries. The slices represent:  
- Canada  
- France  
- Germany  
- Mexico  
- United States of America  

### Key Insights  
- **Germany** dominates with **38%** of total sales, driven by high-value government contracts (e.g., `Paseo` sales at $352,100).  
- **Mexico** follows with **32%**, largely from midmarket and small business segments (e.g., `Montana` and `VTT` products).  
- The **United States of America** and **Canada** contribute **18%** and **9%**, respectively, with diversified sales across segments.  
- **France** accounts for the smallest share (**3%**), with limited enterprise activity.  

### Data Processing  
- Aggregated the `Sales` column grouped by `Country`.  
- Converted absolute sales values to percentages for visual clarity.  

## How to Reproduce  
1. **Dataset**: Use the provided `Financials.csv`.  
2. **Tools**:  
   - Python (Pandas for aggregation, Matplotlib/Seaborn for plotting).  
   - Tableau/Power BI for interactive visualizations.  
3. **Steps**:  
   - **Bar Chart**: Group by `Country`, sum `Profit`, and plot as bars.  
   - **Density Chart**: Extract `Month` and `Year` from `Date`, aggregate `Gross Sales`, and visualize density.  
   - **Pie Chart**: Group by `Country`, sum `Sales`, and plot percentages.  

## Notes  
- The `Discount Band` and `Product` columns significantly influence sales and profit trends.  
- Anomalies:  
  - A December 2014 record in Canada (`Carretera` product) shows an unusually high profit of $236,716 due to a large government contract.  
  - Germany’s sales are inflated by recurring bulk orders for `Velo` and `Paseo` products.  
