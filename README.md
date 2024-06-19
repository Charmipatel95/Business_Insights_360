# Business_Insights_360
## Project Overview

AtliQ Hardware is growing really fast, and now they're jumping into using PowerBI to look at data for the first time. They want to beat their competitors and make better decisions using data. This project is all about giving clear answers to questions about money, sales, advertising, and how they get their products to customers.
I worked on this project by following the Codebasics PowerBi Course

:link: [Live Report Link](https://app.powerbi.com/view?r=eyJrIjoiYmNhNzQ0MzAtMDk3Ny00OWU0LTk1MjItYjc0ODE2ZWNlYjQ5IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

:link: [LinkedIn Post](https://www.linkedin.com/posts/charmi-patel-771815242_powerbi-dataanalysis-dashboarddesign-activity-7209242862121627648-hglH?utm_source=share&utm_medium=member_desktop)

Here's a rundown of everything I've learned:
## :mag: Key Skills:

- Using SQL
- PowerBi Desktop for data analysis
- Excel for spreadsheet tasks
- DAX language for advanced calculations
- DAX Studio for report optimization
- Project charter file for project management

## :bulb: PowerBi Techniques:
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

## :dart: Business related terminologies
- Gross price, Pre-invoice deductions, Post-Invoice deductions, Net Invoice sale
- Gross Margin, net sales, net profit
- COGS (Cost of Goods Sold), YTD (Year to Date), YTG (Year to Go)
- Direct, Retailer, Distributors, Consumer

## :white_check_mark: Other Insights:
- Resume tips
- Questioning techniques
- Problem-solving mindset
- Interview strategies

## :office: Company’s background

AltiQ Hardware has expanded globally and sells computers and accessories through three main channels: 
- Retailers,
- Direct sales
- Distributors.
Unfortunately, a recent venture into the American market resulted in unexpected losses, based on surveys, intuition, and basic Excel analysis. Unlike their competitors, who have robust analytics teams, AltiQ realizes they need to invest in their own analytics team to make smarter decisions and thrive in the industry. 

### :chart_with_upwards_trend: Dataset **Understanding.**
In simpler terms, here's what data we have available for analysis:

- :package:**Dimension Tables**: These contain static information about customers and products.
    - :two_men_holding_hands:	**dim_customer**
      - **27** distinct markets (ex India, USA, spain)
      - **75** distinct customers thorough out the market
       - **2** types of platforms
           - Brick & Motors - Physical/offline store
           - E-commerce - Online Store (Amazon, flipkart)
      - Three channels
         - Retailer
          - Direct
        - Distributors

     - 🛒**dim_market**: Information about different markets, including sub-zones and regions.
        - **27** distinct markets (ex India, USA, spain)
        - 7 sub-zones
        - 4 regions
            - APAC
            - EU
            - nan
            - LATAM
  
     - 🏷️**dim_product**: Breakdown of products into divisions, categories, and variants.
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
  
- :package:**Fact Tables**: These contain transactional data.
  - :clipboard:**fact_forecast_monthly**: Used for forecasting customer needs, with details like start date of the month and forecasted quantities.
      - This table is used to forecast the customer’s need in advance, which can help in
        - Higher customer satisfaction
        - Reduced cost in warehouses for storage purpose
    - The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
    - All the date of the month will be replaced by the start date of the month
    - It will have all the column names and in the end it will have the forecast quantity need of the customer
    
  - :calendar:**fact_sales_monthly**: Similar to the forecast table but with actual sold quantities instead of forecasted ones.

- :package:**Additional Tables**:
  - :moneybag:**freight_cost**: Details about travel and other costs for each market.
  - :dollar:**gross_price**: Information about gross prices linked to product codes.
  - :moneybag:**manufacturing_cost**: Details of manufacturing costs linked to product codes and years.
  - 🏷️**Pre_invoice_deductions**: Information about pre-invoice deductions for each customer.
  - 🔖**Post_invoice_deductions**: Details about post-invoice deductions and other deductions.

Understanding this data will help us conduct thorough analysis and make informed decisions to improve business outcomes.

## :inbox_tray: Importing data into PowerBi

- Since our project uses MySQL as the database, we'll need to import datasets from MySQL into PowerBI. To do this, we'll need to provide the necessary credentials to access the database.

## :card_file_box: Data Model

- Think of data modeling as the blueprint for our reports—it's the backbone that everything else relies on. If our blueprint isn't strong, our reports won't perform well. So, we'll make sure our data modeling is spot-on.
- We're using the Snowflake method to keep everything neat and tidy.

![bi 360- data model](https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/2fc1a90e-544b-468b-b40e-5cde0876d493)

### :bar_chart: Dashboard designing

Once we've got the mockups as our guide, it's full steam ahead for the team to start crafting visuals and whipping up measures whenever they're needed.

## :house: Home view

On the main Home view, you'll see a menu with various options like Information, Finance, Sales, Marketing, Supply Chain, Executive, Products, and Support. Just choose the one you're interested in by clicking its button, and you'll be whisked away to that specific view page in no time.

![hp](https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/7196194d-a8e4-455b-a705-6867025cf1c4)

## :chart_with_downwards_trend:	Overall Report
https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/af650d6d-8b2d-4e09-b84c-27b41a8cc00f

## :moneybag: Finance View

https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/65099d0d-74db-464b-8192-c874edd0144f

## 🛒 Sales View

https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/cebe602e-c482-41e3-9315-07973503d694

## :loudspeaker: Marketing View

https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/56e9712f-1afa-4c71-a99d-64322d2c352f

## :truck: Supply chain View

https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/4cf98eb6-c130-455f-bbb7-9fbd8c72db73

## 👩🏻‍💼Executive View

https://github.com/Charmipatel95/Business_Insights_360/assets/154671418/e23cac4a-a4fa-461b-bec1-9538a5ecf938

you can check the [live dashboard](https://app.powerbi.com/view?r=eyJrIjoiYmNhNzQ0MzAtMDk3Ny00OWU0LTk1MjItYjc0ODE2ZWNlYjQ5IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

## :mortar_board:	Project Outcome

This report empowers decision-making through data-driven insights, enabling users to address various "why" questions that arise in different situations.
