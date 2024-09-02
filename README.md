## 🌟 Business Insights 360

### Project Overview 📊

AtliQ Hardware has been experiencing rapid growth in recent years. To maintain their competitive edge, they decided to implement data analytics using Power BI for the first time. The goal of this project is to empower stakeholders with data-driven insights across all aspects of the business, including finance, sales, marketing, and supply chain.

This project was developed by following the [Codebasics Power BI Course](https://codebasics.io/courses/power-bi-data-analysis-with-end-to-end-project), ensuring that industry best practices were applied throughout.

🔗 [Live Report Link]([https://app.powerbi.com/view?r=eyJrIjoiNzM1M2Y1ODYtNjk4MS00MGI3LTliYjMtODE0MjczNDhlOTQwIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9](https://app.powerbi.com/view?r=eyJrIjoiNzM1M2Y1ODYtNjk4MS00MGI3LTliYjMtODE0MjczNDhlOTQwIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&pageName=a13d39a7dda5a1ca29e3))

### Tech Stack ⚙️

- **SQL**: For database querying and management.
- **Power BI Desktop**: The primary tool for building interactive dashboards and reports.
- **Excel**: Used for data preprocessing and analysis.
- **DAX Language**: For creating calculated columns and measures within Power BI.
- **DAX Studio**: Used for optimizing report performance.
- **Project Charter**: Document outlining the project's scope, objectives, and deliverables.

 

---

## 💡 Power BI Techniques Learned

During this project, I honed several essential Power BI skills and techniques that are crucial for effective data analysis and reporting:

### Key Project Questions to Ask 🔍

- What are the key objectives of this project?
- What metrics define the project's success?
- What is the project timeline?
- What are the stakeholder expectations?
- Who will use the dashboard, and for what purposes?
- What resources are necessary to complete the project?

### Power BI Technical Skills 🛠️

- **Calculated Columns**: Creating calculated columns for enhanced data analysis.
- **DAX Language**: Building complex measures using DAX to drive insights.
- **Data Modeling**: Structuring data models to ensure efficient and accurate reporting.
- **Bookmarks**: Utilizing bookmarks for seamless visual switching.
- **Page Navigation**: Implementing buttons for intuitive page navigation.
- **DIVIDE Function**: Using the DIVIDE function to prevent zero-division errors.
- **Date Table Creation**: Building date tables using M language for time intelligence.
- **Dynamic Titles**: Creating dynamic titles that change based on applied filters.
- **KPI Indicators**: Leveraging KPIs to track and display key performance metrics.
- **Conditional Formatting**: Applying icons or background colors for visual emphasis in reports.
- **Data Validation**: Ensuring data accuracy and consistency with validation techniques.

### Power BI Services 🌐

- **Report Publishing**: Publishing reports to Power BI Service for broader accessibility.
- **Personal Gateway Setup**: Setting up a personal gateway for automatic data refresh.
- **App Creation**: Creating Power BI Apps for easier distribution and access.
- **Collaboration & Permissions**: Managing workspaces, collaboration, and access permissions within Power BI Service.
- And more! 😅

---

## 🧰 GitHub Skills

- **Large File Uploads**: Uploading large files using GitHub LFS (Large File Storage).
- **File Tracking**: Tracking specific file types with LFS for better version control.

---

## 📚 Business-Related Terms

Understanding these key business terms was vital for the project:

- **Gross Price**
- **Pre-Invoice Deductions**
- **Post-Invoice Deductions**
- **Net Invoice Sale**
- **Gross Margin**
- **Net Sales**
- **Net Profit**
- **COGS** (Cost of Goods Sold)
- **YTD** (Year to Date)
- **YTG** (Year to Go)
- **Direct Sales**
- **Retailers**
- **Distributors**
- **Consumers**
---

## 🏢 Company Background

AtliQ Hardware has experienced significant growth in recent years, expanding its business across the globe. The company specializes in selling computers and computer accessories through three primary channels:

1. **Retailers**
2. **Direct Sales**
3. **Distributors**

However, a recent expansion into the American market resulted in unforeseen losses. This decision was based on surveys, intuition, and some Excel analysis. Meanwhile, competitors with strong analytics teams have been making data-driven decisions, leaving AtliQ Hardware with no choice but to build its own analytics team. The goal is to leverage data-driven insights and make informed decisions to stay competitive in the industry.

---

## 🚀 Project Kickoff

-Before diving into the project, it's crucial to clarify its purpose and objectives. Here are the key questions to consider:

### Questions to Ask Before Starting the Dashboard

- **Objective**: What is the main goal of building this Power BI dashboard?
- **Success Criteria**: How will the success of this project be measured?
- **Timeline**: What is the project's deadline?
- **Stakeholder Expectations**: Are stakeholders expecting a preview before the final release?
- **Hopes**: What are the stakeholders hoping to achieve with this project?
- **Fears**: What concerns do stakeholders have about building this dashboard?
- **Users**: Who will be using this dashboard, and for what purpose?
- **Expectations**: What are the stakeholders' expectations upon project completion?
- **Risks**: What potential issues could arise during the project?
- **Resources**: What data and resources are needed to build this dashboard?
- **Design Input**: Do stakeholders have any input on the design and layout of the dashboard?
   After the project kickoff meetings, the data engineering team provided the necessary datasets as requested by the data analytics team. Let's dive into exploring and understanding the data!
---

## 📂 Dataset Understanding

Before diving into the analysis, it's essential to grasp the available data. A clear understanding of the dataset lays the groundwork for meaningful insights.

### Dimension Tables 🗃️

These tables contain static data, such as customer and product details.
- **gdb056**:
 - **dim_customer**:
  - 27 distinct markets (e.g., India, USA, Spain)
  - 75 distinct customers across all markets
  - 2 types of platforms:
    - Brick & Mortar: Physical/offline stores
    - E-commerce: Online stores (e.g., Amazon, Flipkart)
  - 3 sales channels:
    - Retailer
    - Direct
    - Distributors

 - **dim_market**:
  - 27 distinct markets (e.g., India, USA, Spain)
  - 7 sub-zones
  - 4 regions:
    - APAC
    - EU
    - NA
    - LATAM

 - **dim_product**:
  - Divisions:
    - P & A (Peripherals & Accessories)
    - PC (Notebook, Desktop)
    - N & S (Networking & Storage)
  - 14 different categories (e.g., Internal HDD, Keyboard)
  - Various product variants available for the same category

### Fact Tables 📊

These tables capture transactional data.

- **fact_forecast_monthly**:
  - Used for forecasting customer needs in advance, contributing to:
    - Higher customer satisfaction
    - Reduced warehousing costs
  - Denormalized by the data engineering team for analytical work
  - Dates replaced by the start date of the month
  - Includes forecasted quantities needed by customers

- **fact_sales_monthly**:
  - Similar to the `fact_forecast_monthly` table
  - The last column shows sold quantities instead of forecasted values

### Additional Tables 🗂️

- **gdb056**:
  - **freight_cost**:
    - Details travel and other costs for each market by fiscal year
  - **gross_price**:
    - Contains gross prices along with product codes
  - **manufacturing_cost**:
    - Lists manufacturing costs by product code and year
  - **pre_invoice_deductions**:
    - Includes pre-invoice deduction percentages by customer and year
  - **post_invoice_deductions**:
    - Contains post-invoice deductions and other related details

## 🛠️ Importing Data into Power BI

For this project, the database is housed in MySQL. To begin, datasets were imported into Power BI by connecting to the MySQL database using the appropriate access credentials. This step was crucial for pulling in the necessary data to build insightful reports.

## 🗺️ Data Modeling

Data modeling is the foundation of any Power BI report. A well-structured data model ensures that all visuals perform efficiently and accurately. Poor data modeling can significantly degrade report performance, making it critical to follow best practices.

In this project, we adhered to the **Snowflake Data Modeling** method, which organizes the data in a way that supports complex queries and provides a scalable model for future reporting needs.

For more insights on data modeling best practices, you can refer to this [blog](#).



















