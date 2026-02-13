# Pricing-Report-Automation
This is an automated supplier-comparison and margin-optimization script that transforms raw pricing data into actionable business intelligence.

# 📊 Project Overview
In retail and e-commerce, sourcing costs are often scattered across multiple vendor spreadsheets, with inconsistent naming conventions and hidden fees (such as shipping). This project automates the ingestion, normalization, and analysis of these sources to identify the most profitable sourcing options and flag products requiring immediate price adjustments.

# 🛠️ Technical Implementation

The pipeline is engineered for data integrity and scalability, moving away from "flat-file" merging to a robust Logic Engine approach.

> Schema Mapping & Normalization: Programmatically resolves disparate column headers (e.g., ItemID vs SKU) into a unified key for relational joins.

> Landed Cost Calculation: Isolates specific vendor overheads (Shipping Fees) to ensure an "apples-to-apples" comparison between raw wholesale costs and landed costs.

> High-Precision Formatting: Implements a strict 0.00% decimal mask in the final export to prevent rounding bias in marginal profitability analysis.

> XlsxWriter Engine: Bypasses standard CSV limitations by applying cell-level formatting, freeze panes, and conditional logic directly within the Python script.


<img width="1047" height="300" alt="image" src="https://github.com/user-attachments/assets/d2c6615a-ff9b-476b-9287-079dfdd07e85" />


# Core Dependencies:

pandas>=1.3.0       # Data manipulation and analysis

numpy>=1.20.0       # Numerical operations

xlsxwriter>=3.0.0   # Advanced Excel formatting


# 📈 Business Impact

This tool replaces hours of manual VLOOKUP tasks with a single-click audit of an entire inventory.

> Optimal Sourcing Selection: Automatically identifies the lowest-cost provider between multiple suppliers, directly impacting the bottom line.

> Risk Mitigation: The "Action Status" engine uses conditional formatting to instantly flag "at-risk" products where margins have slipped below the 20% threshold.

> Executive Readability: Uses data bars and color-coded alerts to allow stakeholders to perform a 10-second "visual audit" of inventory health.

> Scalable Foundation: Built as a modular engine, the script can be expanded to include AI-driven price forecasting or real-time API price scraping.


# 📂 System Architecture

The code follows a 4-stage pipeline:

> Ingestion: Loading fragmented .xlsx dataframes.

> Logic Engine: Executing cost comparisons and margin calculations.

> Formatting: Defining strict currency and percentage masks.

> Reporting: Generating a polished, client-ready Executive Dashboard.

# 🚀 How to Use

> Open the Google Colab Notebook.

> Ensure your vendor files follow the standardized headers or update the Schema Mapping section.

> Run all cells to generate Pricing_Analysis_Report.xlsx.

