# POWER BI HANDS-ON WORKSHOP - BY SHIVANI TYAGI

## Workshop Details
- **Event**: Data Visualization Workshop
- **Date**: March 20th, 2026
- **Time**: 3:00 PM - 5:00 PM
- **Location**: OM 1335
- **Speaker**: Shivani Tyagi (Power BI)
- **Institution**: Thompson Rivers University
- **Hosted by**: TRUSU Data Science Club

Power BI is one of the most popular & powerful data visualization tools in the world, of course it is within the Microsoft ecosystem.

Companies that use MICROSOFT as their computing & communication stack will 100% have access to the MICROSOFT Suite which includes POWER BI.

We might not be able to cover everything in this session but I will try my best. We will start with some of the basics of just creating some visualizations but we will dive into other things as well.

## Table of Contents
- [Prerequisites](#prerequisites)
- [PART I: Getting Started with Power BI Desktop](#part-i-getting-started-with-power-bi-desktop)
- [PART II: How to Use Power Query Tool in Power BI](#part-ii-how-to-use-power-query-tool-in-power-bi)
- [PART III: Relationships in Power BI](#part-iii-relationships-in-power-bi)
- [Additional Features](#additional-features)
- [Getting Started](#getting-started)
- [Resources](#resources)

## Prerequisites
- Power BI Desktop installed (Windows) or access to Power BI Online (MacOS).
- Basic understanding of Excel and data concepts.
- Download the workshop datasets from the `Power BI Tutorial Datasets/` folder.

## PART I: Getting Started with Power BI Desktop

### INSTALLATION / DOWNLOADING Power BI Desktop
- **Windows**: Free download via Microsoft Store.
- **MacOS**: Unfortunately, no native app available. Use Power BI online instead (interface is slightly different).

### UI Interface: Let's Get Started
1. Search for Power BI and open the application.
2. Click on **"GET DATA"** to start importing data.
3. A window opens with various data source options (some free, some require upgrade).

### Data Import and Exploration
4. For this workshop, we'll use Excel files from the `Power BI Tutorial Datasets/` folder.
   - **Dataset for Part I**: [Emergency Food Prep.xlsx](Power%20BI%20Tutorial%20Datasets/Emergency%20Food%20Prep.xlsx)
5. Select **Excel** > **Connect** > Navigate to and select `Emergency Food Prep.xlsx`.
6. In the **Navigator** window, select the relevant sheets (if multiple).
7. Choose between:
   - **Load**: Directly to Reporting/Visual view
   - **Transform Data**: Opens Power Query Editor for data preparation

### Quick Glance at Power Query Editor
8. Power Query Editor is a window to transform your data and prepare it for visualization (similar to Excel, Python, etc.).
9. Data checks:
   - Ensure dates are in `date_purchased` format
   - Filter products (e.g., remove items like milk that don't last long)
10. **Close & Apply** to load the data.

### Applied Steps and Data Tab Exploration
11. In the **Data Tab**, explore your data. Example scenario: Tracking purchases of different products across months and locations to find where you're spending less money, or if certain products are cheaper at specific stores (e.g., Costco vs. Walmart).

### Report Tab: Building Visualizations
12. Switch to **Report Tab** to create visualizations.
13. Use the **Visualizations Panel** (right side) for dashboard creation.
14. **Fields Panel**: Based on Sheet 1 data.

#### Key Questions to Answer:
- Where are we spending the least amount of money?
- Should we buy all items at one store, or are certain products cheaper at specific stores?

#### Visualization #1: Store & Price Comparison
- Select **Stacked Column Chart**
- Add **Store** to Legend for color coding

#### Visualization #2: Product, Price & Store Analysis
- Select **Clustered Column Chart**
- Examples: Rice at Target/BW vs. Costco, DB at Costco, CV at other stores
- Enable **Data Labels** in Format > Visual > Data Labels > On
- Customize **Title** in Format > General > Title

## PART II: How to Use Power Query Tool in Power BI

### Dataset II: Advanced Data Preparation
- **Dataset for Part II**: [Emergency Food Prep - Power Query Editor Tutorial.xlsx](Power%20BI%20Tutorial%20Datasets/Emergency%20Food%20Prep%20-%20Power%20Query%20Editor%20Tutorial.xlsx)
- This dataset includes Pivot Tables and Purchase Overview.

### Loading and Transforming Data
1. Load the Excel file and select **Transform Data** to open Power Query Editor.
2. In **Query Settings** (top ribbon), rename the query to something like "PT 2026".
3. Handle data types:
   - ABC columns: Ensure text format
   - 123 columns: Ensure numeric format
4. **Remove Top Rows**: Home > Remove Rows > Remove Top Rows > 2 (to remove headers)
5. **First Row as Header**: Transform > Use First Row as Headers
6. Convert to appropriate data types (e.g., Fixed Decimal Number for prices).
7. Remove unnecessary rows like Totals.
8. Filter locations: Remove empty values using Text Filters.
9. Remove Grand Total column: Home > Remove Columns
10. Transpose dates: Select date columns > Transform > Unpivot Columns
    - Rename: Attribute to "DT", Value to "Product_Cost", etc.
11. **Close & Apply** to load the transformed data.
12. Rename the table to "Pivot Table 2022" or similar.

## PART III: Relationships in Power BI

### Dataset III: Building Relationships
- **Dataset for Part III**: [Emergency Food Prep - Relationship Tutorial.xlsx](Power%20BI%20Tutorial%20Datasets/Emergency%20Food%20Prep%20-%20Relationship%20Tutorial.xlsx)
- Use this dataset to learn about creating relationships between multiple tables in Power BI.

### Steps for Relationships
1. Load the Excel file with multiple sheets/tables.
2. In the **Model Tab**, create relationships between tables by dragging fields.
3. Ensure proper cardinality (e.g., One-to-Many, Many-to-One).
4. Use relationships to enable cross-table analysis in visualizations.

## Additional Features
- **Report Tab**: Add more data sources, create new visuals, add text boxes, perform calculations.
- **Publish & Share**: Share dashboards/reports online via Power BI Service.

## Getting Started
1. Clone or download this repository.
2. Open Power BI Desktop.
3. Follow the steps in each part using the provided datasets.
4. Experiment with visualizations and data transformations.

## Resources
- [Power BI Official Documentation](https://docs.microsoft.com/en-us/power-bi/)
- [Power BI Community](https://community.powerbi.com/)
- [Thompson Rivers University Data Science Club](https://www.trusu.ca/)


## Getting Started
1. Clone or download this repository.
2. Open Power BI Desktop.
3. Follow the steps in each part using the provided datasets.
4. Experiment with visualizations and data transformations.

Helping you become a Data Analyst using Power BI.
