
# Sales DashBoard 

### Dashboard Link: https://app.powerbi.com/links/g3ey5XU8Nc?ctid=781153e2-8737-4859-b359-072aaf8cf8d6&pbi_source=linkShare

## Problem Statement

This dashboard helps the company to understand their customers' interest in the product, their sales, profit, average sales, and other things better. It helps the company to know which products their customer buy more according to their region, country, and city. The company could also find out the profit on their product which product earns more profit and which is less. They also can find out what channel earns more profit for them. 

By using this they can increase their profit on the channels.

### Steps followed 

- Step 1: Load data into Power BI Desktop, the dataset is an Excel file.
- Step 2: Open the power query editor & in the view tab under the Data Preview section, and check the "column distribution", "column quality" & "column profile" options.
- Step 3: Also since by default, the profile will be opened only for 1000 rows you need to select "column profiling based on the entire dataset".
- Step 4: It was observed that in none of the columns errors & empty values were present except column named "Arrival Delay".
- Step 5: Calculating Total sales, Total profit, average sales, No of products, profit by city, profit by, and profit by region.
- Step 6: In the report view, under the view tab, theme was selected.
- Step 7: Since we want to see the profit according to year we extract the order date column and take only the year value and create new column using Dax. 
- Step 8: Visual filters (Slicers) were added for one field named "Year ".
- Step 9: Four card visuals were added to the canvas, they represent the average sales, total sales, total profit, and no of product.


![cp5](https://github.com/hasanahmad676/Power-bi_project/assets/82166280/7de2e3c1-afa6-4c50-8b54-898182ee4397)
           
           
- Step 10: Two bar chart was also added to the report design area representing the profit by city and sales by city. 

![cp4](https://github.com/hasanahmad676/Power-bi_project/assets/82166280/ea3ff154-61eb-4999-9aaf-f2e352cb4383)


-Step 11: we used one pie chart and one donut chart to see the profit via channel and region.


![cp2](https://github.com/hasanahmad676/Power-bi_project/assets/82166280/febbbc18-e6a6-4809-9453-f0fa3daac0de)

![cp3](https://github.com/hasanahmad676/Power-bi_project/assets/82166280/797d0591-62f3-4596-ba85-67cf4c333454)


-Step 12: we also used the map to show the country where the company earns most of its profit.

![cp1](https://github.com/hasanahmad676/Power-bi_project/assets/82166280/c009fb5d-2481-42ca-bd38-0555208494d1)


- Step 13: In the report view, under the insert tab, using the shapes option from the elements group a rectangle was inserted where the title was added to the report design area. 
- Step 14: Calculated column was created in which, the year value was extracted from the order column.

for creating a new column following the DAX expression was written;
       
        YearOnlyColumn = 
        
        YearOnlyColumn = YEAR('Data'[Order Date])
        
        
        
Snap of the new calculated column,

![Capture](https://github.com/hasanahmad676/Power-bi_project/assets/82166280/f924661a-eeeb-4903-8cc1-77c1a378f6dc)

- Step 15: The report was then published to Power BI Service.
 

![cp6](https://github.com/hasanahmad676/Power-bi_project/assets/82166280/50c201fe-0ec2-421c-a9fd-b8a11c920510)

# Snapshot of Dashboard (Power BI Service)


![cp7](https://github.com/hasanahmad676/Power-bi_project/assets/82166280/678e4ce4-7872-421a-9525-417708ebece8)

# Report Snapshot (Power BI DESKTOP)

 

![cp8](https://github.com/hasanahmad676/Power-bi_project/assets/82166280/35ab0e62-45c8-46c7-861c-69bbe9b105d0)

# Insights

A single-page report was created on Power BI Desktop & it was then published to Power BI Service.

The following inferences can be drawn from the dashboard;


### [1] Total Number of products = 15000
 Top 10 products THAT earn more profit----->
 
  1. Contoso Projector 1080p X980 White = 13 (320513. 2935461144)
  2. Proseware Projector 1080p LCD86 White = 14 (315379.9154591368)
  3. Contoso Projector 1080p X980 Black = 17 (252654.59703150686)
  4. Proseware Projector 1080p LCD86 Black = 14 (232556.5145670583)
  5. Proseware Projector 1080p DLP86 Silver = 14 (228823.61499156008)
  6. Proseware Projector 1080p DLP86 Black = 11 (208705.1012010968)
  7. Fabrikam Independent Filmmaker 1" 25mm X400 Blue = 16 (188427.74576812048)
  8. 182459.4009410981 = 16 (182459.4009410981)
  9. 156805.7685652145 = 14 (156805.7685652145)
  10. Fabrikam Trendsetter 2/3'' 17mm X100 White = 19 (155118.7770490604)
   These 10 products earn most of the profit for the company.

### [2] Profit earned by channel
 In the channel, we can see that

    a) store earn (almost 53 %),
    b) Online(almost 23 %),
    c) Reseller(almost 15 %),
    d) Catalog(almost 9.37 %)
    
Here the company sells different amounts of products each year on this channel and earns  a profit.

   
### [3] Profit earned by region 
  
    a) North America earn 63% of total profit
    b) Europe earns 20% of the total profit
    b) Asia earn 17% of total profit

Here is the percentage of the profit earned by each region.



 

        
