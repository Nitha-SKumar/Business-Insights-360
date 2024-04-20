# Business-Insights-360
## Project Overview: Implementing Data Analytics with Power BI at AtliQ Hardware

AtliQ Hardware, experiencing rapid growth in recent years, is embarking on a transformative journey by integrating data analytics through Power BI. This strategic initiative aims to propel the company ahead of competitors while fostering a culture of data-driven decision-making.

### Objectives:

The primary aim of this endeavor is to equip stakeholders across finance, sales, marketing, and supply chain functions with actionable insights derived from robust data analytics. By leveraging Power BI, AtliQ Hardware endeavors to elevate decision-making processes, optimizing performance across all facets of the business.

### Scope:

The project entails a comprehensive examination of finance, sales, marketing, and supply chain dynamics. Leveraging Power BI's capabilities, data from diverse internal and external sources will be harmonized to provide a comprehensive understanding of the business landscape.


I undertook this project guided by the Codebasics Power BI Course


[Live Report Link](https://app.powerbi.com/view?r=eyJrIjoiMmIwNzU1NDAtNTFkMy00MTA0LTg5NjItNjQyY2RiODQ3MjVhIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

### Technology Stack:

- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)
- Project charter file

### Learned PowerBI Techniques:

- Understanding project prerequisites
- Formulating key project questions
- Utilizing calculated columns
- Implementing measures with DAX language
- Executing data modeling
- Employing Bookmarks for visual switching
- Navigating pages using buttons
- Preventing zero division errors with the divide function
- Generating date tables using M language
- Creating dynamic titles based on applied filters
- Incorporating KPI indicators
- Implementing data validation techniques
- Exploring PowerBI services
- Publishing reports to PowerBI services
- Configuring personal gateway for data auto-refresh
- Creating PowerBI Apps
- Collaborating on workspaces and managing access permissions in PowerBI services


### Business Terminology:

- Gross price
- Gross Margin
- Net sales
- Net Invoice sale
- Net profit
- COGS - Cost of Goods Sold
- Pre-invoice deductions
- Post-invoice deductions
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer


### Company Overview:

AtliQ Hardware has experienced significant growth in recent years, expanding its operations globally. Specializing in the sale of computers and computer accessories, the company operates through three main channels:

- Retailers
- Direct sales
- Distributors


However, AtliQ Hardware recently faced unexpected losses, notably with the opening of a store in America. Despite relying on surveys, intuition, and basic Excel analysis, the company found itself at a disadvantage compared to competitors equipped with dedicated analytics teams. Recognizing the need for data-driven insights and decisions, AtliQ Hardware is now taking steps to establish its own analytics team to enhance its competitive position in the industry.

### Project Kickoff Considerations:

Before diving into dashboard development, it's essential to address several key questions in the project kickoff session:

### Questions to Consider Before Dashboard Development:

- What are the primary objectives of building this Power BI dashboard?
- How will the success of this project be measured?
- What is the expected timeline for project completion?
- Do stakeholders require a preview before the official release?
- What are the stakeholders' expectations and desired outcomes for this project?
- What concerns or fears do stakeholders have regarding dashboard development?
- Who will be the primary users of the dashboard, and what will be its primary use cases?
- What specific deliverables are stakeholders anticipating upon completion of this project?
- What potential challenges or risks might impact the project's success?
- What data sources and resources are necessary to construct the dashboard?
- Have stakeholders provided input on dashboard design and visualization preferences?


Following the project kickoff meetings, the data engineering team has provided the requested datasets to the data analytics team. Now, let's delve into understanding the dataset:

### Dataset Overview:

Understanding the available data is crucial for effective analysis. Before delving into analysis, it's essential to gain a comprehensive understanding of the dataset.

### Dimension Tables:

#### dim_customer:
- Contains static data such as customer and product details.
- 27 distinct markets (e.g., India, USA, Spain).
- 75 distinct customers across markets.
- Two types of platforms: Brick & Mortar (physical/offline store) and E-commerce (online store).
= Three channels: Retailer, Direct, and Distributors.
#### dim_market:
- Includes 27 distinct markets with 7 sub-zones and 4 regions (APAC, EU, LATAM).
#### dim_product:
- Divisions: P & A (Peripherals & Accessories), PC (Personal Computer), N & S (Networking & Storage).
14 different categories (e.g., Internal HDD, Keyboard).
-Various product variants.
### Fact Tables:

#### fact_forecast_monthly:
- Used for forecasting customer needs in advance.
- Denormalized for analytical purposes.
- Contains columns with the start date of each month and forecasted quantity needed by customers.
#### fact_sales_monthly:
- Similar to fact_forecast_monthly but with actual sold quantities instead of forecasted values.
### Additional Tables:

#### gdb056_freight_cost:
-Details of travel and other costs for each market per fiscal year.
#### gdb056_gross_price:
- Contains gross prices with product codes.
#### gdb056_manufacturing_cost:
- Provides manufacturing cost details with product codes and years.
#### gdb056_Pre_invoice_dedutions:
- Details of pre-invoice deductions percentages for each customer per year.
#### gdb056_Post_invoice_deductions:
- Details of post-invoice deductions and other deductions.
 
The provided dataset offers a wealth of information that will be instrumental in conducting comprehensive analyses and deriving valuable insights.

Importing data into Power BI from a MySQL database is a crucial step in this project. Access credentials for the database will be required to establish the connection and import the datasets.

### Data Model:

- Data modeling forms the foundation of the report-building process in Power BI. All visualizations are constructed based on the data model, making it a critical component.

- In this project, we have adopted the Snowflake data modeling method, which involves organizing data into multiple normalized tables connected by foreign key relationships. This approach facilitates efficient querying and analysis while maintaining data integrity.

- By implementing sound data modeling practices and leveraging the Snowflake method, we aim to create a robust foundation for our Power BI reports, enabling us to derive meaningful insights and drive informed decision-making.





