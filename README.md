
**COMPANY** : CODTECH IT SOLUTIONS

 **NAME** : NERUSU MADHU JAHNAVI

**INTERNID** : CT6WNSZ

**DOMAIN** : POWER BI

**DURATION** : 6 WEEKS


#### DESCRIPTION ####


******DATA INTEGRATION FROM MULTIPLE SOURCES(EXCEL AND POSTGRESQL SERVER) ********

### Step-by-Step Process:

#### Step 1: Load Data into Power BI

1. **Load Excel Data (Sales Data) into Power BI:**
   - Open **Power BI Desktop**.
   - Go to **Home > Get Data > Excel**.
   - Select the Excel file containing the sales data.
   - Choose the relevant sheet or table (e.g., Salesdata) and click **Load**.

2. **Load PostgreSQL Data (Information ) into Power BI:**
   - Go to **Home > Get Data > PostgresqlL Server**.
   - Enter the server and database information for the Postgresql server.
   - Choose the table or view containing the customer information (e.g., Customer Data).
   - Click **Load** and **Transform**

#### Step 2: Create Relationships Between Tables
- Go to the **Model** view in Power BI.
- Drag and drop CustomerID from the Sales Data table to CustomerID in the Information table to create a relationship.
  - Ensure the relationship is **one-to-many** (one customer can have many sales).

#### Step 3: Data Integration and Calculation
Now that the data is integrated,  can create new columns or measures.
Measure:
      1.Total Sales = SUM(SalesData[SalesAmount])
      2.Average Date of birth = AVERAGE(CustomerData[Date of birth])
 

#### Step 4: Build Visualizations
Now  can create visuals based on the integrated data.

1.  Sales by Region:
   - **Axis**: Region (from the Information table).
   - **Values**: Total sales (the measure  created from the Sales Data table).
   - This shows the total sales per region.

2. **Sales Trend over Time:**
   - **Axis**: Sale Date (from Sales Data).
   - **Values**: Total Sales
   - This shows sales trends over time.

3. **Customer Demographics:**
   - Show a table with columns: Customer Name, Region,Date of birth.
   - This gives a detailed breakdown of customer demographics alongside sales data.

4. **Top 5 Products Sold:**
   - **Axis**: Product (from Sales Data).
   - **Values**: Total Sales.
   - Filter to show only the top 5 products by sales amount.

#### Step 5: Apply Slicers 
  - **Slicer 1**: Region (from Information).
  - **Slicer 2**: Product (from Sales Data).
  - **Slicer 3**: SaleDate (for date filtering).

#### Step 6: Finalizing and Publishing the Report

- When ready, go to **File > Publish** and select  workspace to publish the report to Power BI Service.

Output Report::


![Data integration from multiple sources output](https://github.com/user-attachments/assets/82a6ed72-7ff8-4b45-bc9b-2e8e509e5293)
