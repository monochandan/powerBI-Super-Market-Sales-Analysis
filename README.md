
# Super Market Sales Analysis

### Dashboard Link : working on it.....

## Problem Statement

This dashboard helps the Supermarket Management understand their customers better. It helps to understand which product is more profitable for their busuiness. Through different graph, they get to know their improvement area, & thus they can improve their services by identifying these area. It also lets them know the average daily sales and profits. 

There was 50% customers have no membership. So they can introduce some membership adventages which make them to become a memeber and attract more customer towards them




### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : In the report view, under the view tab, theme was selected.
- Step 5 : Slicer for analysing date wise. In slicer setting changed the style option to dropdown for selecting particular date to analysis.
- Step 6 : There is 2 clustered bar chart. One for overall quantity for different product category. Which will help us to track is there enough product availiable for particular 
date.  Other one show us rating of particular product category.
- Step 7 : Stacked area chart (Average sales and profit) show the average sales and profit.
 - Step 8 : There are 2 card. one showes total product soled. Another one show the highest sold product. For that I had to creat a custome measure.          
           Although, by default, while calculating average, blank values are ignored.
- Step 9 : I used 2 pie chart for catagorized customer by gender and how many of them have membership (also catagorized by gender).
- Step 10 : From the datasheet I have understand that this supermarket company's shopes are availiable in 3 cities with 3 branches in each. So to get the top sell from city-wise, I use again clustered bar chart

- Step 11: Tree map showes the femous payment method

- Step 12: Clustered column chart used to show the cost of each product category



        
- Step 13 : New measure was created to find total count of product sold.

Following DAX expression was written for the same,
        
    highest_sold_product = CALCULATE(MAX('supermarket_sales+-+Sheet1'[Product line]), 'supermarket_sales+-+Sheet1'[Quantity] = max('supermarket_sales+-+Sheet1'[Quantity]))
        
A card visual was used to represent count of total sold product.

![Snap_Count](https://github.com/monochandan/powerBI-Super-Market-Sales-Analysis/assets/29684226/e2cb0df7-b8e2-4533-b8b9-97ece7f86a1b)
 

         
### Customer Type

![Snap_Count](https://github.com/monochandan/powerBI-Super-Market-Sales-Analysis/assets/29684226/c8d32e67-70ae-45a7-a1d7-ad2fbe1c3990)

### Profit by branches and sales by city

![Snap_Count](https://github.com/monochandan/powerBI-Super-Market-Sales-Analysis/assets/29684226/3b25b067-d72d-4637-b68e-067c2ffbc83b)

### Most used payment method

![Snap_Count](https://github.com/monochandan/powerBI-Super-Market-Sales-Analysis/assets/29684226/7b78ceba-374e-437e-94ca-ee99bbfb5c11)

### Quantity of product line

![Snap_Count](https://github.com/monochandan/powerBI-Super-Market-Sales-Analysis/assets/29684226/8a8d543a-4ea1-4394-8681-86110727fbb0)

### Average rating of each product category

![Snap_Count](https://github.com/monochandan/powerBI-Super-Market-Sales-Analysis/assets/29684226/8377975c-5c8b-496e-94db-7d608feeb4a3)

### Cost of goods by product line

![Snap_Count](https://github.com/monochandan/powerBI-Super-Market-Sales-Analysis/assets/29684226/50e21799-1be2-442c-ac13-153a18411323)


## Full dashbord view after selecting particuler date (1 february 2019)

![Snap_Count](https://github.com/monochandan/powerBI-Super-Market-Sales-Analysis/assets/29684226/e3a70d23-f169-40da-8ccb-d4c333d750e3)


