# Dynamic Sales Dashboard — Excel Module

## Project Overview
The **Dynamic Sales Dashboard** is an interactive Excel-based dashboard built as part of a Data Science course. It visualizes retail ecommerce data to analyze sales performance, customer behavior, and key business metrics. The data is ingested from a GitHub repository to ensure reproducibility and version control.

## Key Features
- Monthly and daily sales trends  
- Product/category-level revenue analysis  
- Customer segmentation (new vs returning)  
- Return rate and refund analysis  
- Dynamic filters (date range, region, product category)  
- Interactive charts and pivot tables  
- Automated data refresh using Power Query  

## Dataset
**Primary Table:** `ecommerce`  
This dataset is ingested from GitHub and stored in the `data/` folder. Power Query is used to clean and prepare the data for dashboard visualizations.

### Workflow
1. Load raw data from GitHub (`data/ecommerce.csv`)  
2. Clean and transform using Power Query  
3. Load transformed data into pivot tables  
4. Build dynamic charts and slicers on the Dashboard sheet  

## Project Structure
/
├─ data/
│ └─ ecommerce.csv
├─ dashboard/
│ └─ SalesDashboard.xlsx
├─ scripts/
│ └─ powerquery_steps.txt
└─ README.md

markdown
Copy code

## How to Use
1. Clone or download this repository.  
2. Open `dashboard/SalesDashboard.xlsx`.  
3. Ensure the `ecommerce.csv` file is present in the `data/` folder.  
4. Go to **Data → Refresh All** to load the latest data.  
5. Use the dashboard slicers to explore insights interactively.

## Data Processing (Power Query)
- Load CSV from GitHub  
- Convert data types (dates, numbers)  
- Clean text fields (trim, remove errors)  
- Remove duplicates  
- Add calculated columns (e.g., `Revenue = Quantity * UnitPrice`)  
- Load to Excel Data Model  

## Example Columns (placeholders)
- `order_id`  
- `order_date`  
- `customer_id`  
- `product_id`  
- `category`  
- `quantity`  
- `unit_price`  
- `revenue`  
- `is_returned`  

*(These will be updated once you provide the actual ecommerce sample.)*

## Tools & Requirements
- Microsoft Excel 2016+ / Excel 365  
- Power Query  
- Optional: Power BI Desktop  

## Best Practices
- Do not modify raw data directly—always refresh from source.  
- Document transformation steps inside Power Query.  
- Maintain versioned copies of the dashboard before major updates.  

## Next Steps
- Add Data Dictionary using actual column names  
- Insert sample preview of the dataset  
- Document dashboard layout and visuals  
