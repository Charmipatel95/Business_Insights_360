# Business_Insights_360
## Project Overview

AtliQ Hardware is growing really fast, and now they're jumping into using PowerBI to look at data for the first time. They want to beat their competitors and make better decisions using data. This project is all about giving clear answers to questions about money, sales, advertising, and how they get their products to customers.
I worked on this project by following the Codebasics PowerBi Course

[Live Report Link](https://app.powerbi.com/view?r=eyJrIjoiZGE5Y2M2YzQtOTI3Ny00NGQyLWExYTUtZjAyYmE0YmVhNzYwIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

Here's a rundown of everything I've learned:
## Key Skills:

- Using SQL
- PowerBi Desktop for data analysis
- Excel for spreadsheet tasks
- DAX language for advanced calculations
- DAX Studio for report optimization
- Project charter file for project management

## PowerBi Techniques:
- Asking the right questions before starting a project
- Creating calculated columns and measures
- Data modelling
- Utilizing Bookmarks for goal-switching
- Page navigation with buttons
- Preventing zero division errors with the divide function
- Creating date tables using M language
- Dynamic titles based on applied filters
- Using KPI indicators and conditional formatting
- Data validation techniques
- Publishing reports and setting up auto refresh in PowerBi services
- Creating PowerBi apps
- Understanding collaboration, workspaces, and access permissions

## Business related terminologies
- Gross price, Pre-invoice deductions, Post-Invoice deductions, Net Invoice sale
- Gross Margin, net sales, net profit
- COGS (Cost of Goods Sold), YTD (Year to Date), YTG (Year to Go)
- Direct, Retailer, Distributors, Consumer

## Other Insights:
- Resume tips
- Questioning techniques
- Problem-solving mindset
- Interview strategies

## Company’s background

AltiQ Hardware has expanded globally and sells computers and accessories through three main channels: 
- Retailers,
- Direct sales
- Distributors.
Unfortunately, a recent venture into the American market resulted in unexpected losses, based on surveys, intuition, and basic Excel analysis. Unlike their competitors, who have robust analytics teams, AltiQ realizes they need to invest in their own analytics team to make smarter decisions and thrive in the industry. 

### Dataset **Understanding.**
In simpler terms, here's what data we have available for analysis:

- **Dimension Tables**: These contain static information about customers and products.
  - dim_customer
    - **27** distinct markets (ex India, USA, spain)
      - **75** distinct customers thorough out the market
       - **2** types of platforms
           - Brick & Motors - Physical/offline store
           - E-commerce - Online Store (Amazon, flipkart)
      - Three channels
         - Retailer
          - Direct
        - Distributors

    - **dim_market**: Information about different markets, including sub-zones and regions.
        - **27** distinct markets (ex India, USA, spain)
        - 7 sub-zones
        - 4 regions
            - APAC
            - EU
            - nan
            - LATAM
  
  - **dim_product**: Breakdown of products into divisions, categories, and variants.
        - Divisions
            - P & A
                - Peripherals
                - Accessories
            - PC
                - Notebook
                - Desktop
            - N & S
                - Networking
                - Storage
        - There are 14 different categories, Like Internal HDD, keyboard
        - There are different variants available for the same product
  
- **Fact Tables**: These contain transactional data.
  - **fact_forecast_monthly**: Used for forecasting customer needs, with details like start date of the month and forecasted quantities.
      - This table is used to forecast the customer’s need in advance, which can help in
        - Higher customer satisfaction
        - Reduced cost in warehouses for storage purpose
    - The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
    - All the date of the month will be replaced by the start date of the month
    - It will have all the column names and in the end it will have the forecast quantity need of the customer
    
  - **fact_sales_monthly**: Similar to the forecast table but with actual sold quantities instead of forecasted ones.

- **Additional Tables**:
  - **freight_cost**: Details about travel and other costs for each market.
  - **gross_price**: Information about gross prices linked to product codes.
  - **manufacturing_cost**: Details of manufacturing costs linked to product codes and years.
  - **Pre_invoice_deductions**: Information about pre-invoice deductions for each customer.
  - **Post_invoice_deductions**: Details about post-invoice deductions and other deductions.

Understanding this data will help us conduct thorough analysis and make informed decisions to improve business outcomes.

## Importing data into PowerBi

- Since our project uses MySQL as the database, we'll need to import datasets from MySQL into PowerBI. To do this, we'll need to provide the necessary credentials to access the database.

## Data Model

- Think of data modeling as the blueprint for our reports—it's the backbone that everything else relies on. If our blueprint isn't strong, our reports won't perform well. So, we'll make sure our data modeling is spot-on.
- We're using the Snowflake method to keep everything neat and tidy.

![bi 360- data model](https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/2fc1a90e-544b-468b-b40e-5cde0876d493)

### Dashboard designing

Once we've got the mockups as our guide, it's full steam ahead for the team to start crafting visuals and whipping up measures whenever they're needed.

## Home view

On the main Home view, you'll see a menu with various options like Information, Finance, Sales, Marketing, Supply Chain, Executive, Products, and Support. Just choose the one you're interested in by clicking its button, and you'll be whisked away to that specific view page in no time.

![bi 360- homepage](https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/5f30ad75-ceef-4c8f-80f4-f84e5f140f20)

## Overall Report
https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/f5ca1ab0-0b02-4ea4-8a2c-6fb22120022f


## Finance View

https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/40f1b044-cf40-49e6-9685-81f80ba4481a

## Sales View

https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/9252244b-f03f-43ab-a5a6-15ce6f383007

## Marketing View

https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/2929963d-3ef9-49d6-b456-f0569e94f18e

## Supply chain View

https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/bcefafec-9fc4-458f-8250-7d3fdd62e5aa

## Executive View

https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/e109fceb-42dc-4d14-9eac-d6413b35e445

you can check the [live dashboard](https://app.powerbi.com/view?r=eyJrIjoiZGE5Y2M2YzQtOTI3Ny00NGQyLWExYTUtZjAyYmE0YmVhNzYwIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

## Project Outcome

This report empowers decision-making through data-driven insights, enabling users to address various "why" questions that arise in different situations.
