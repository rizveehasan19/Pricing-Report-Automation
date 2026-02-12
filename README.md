## Pricing-Report-Automation
Automated supplier comparison and margin optimization platform that transforms raw pricing data into actionable business intelligence.

In the competitive retail and wholesale environments, pricing decisions directly impact profitability. Manual comparison of supplier costs, shipping fees, and retail prices across hundreds of SKUs is time-intensive, error-prone, and unscalable. This is an intelligent automation engine that processes multi-supplier pricing data, calculates true landed costs, identifies optimal suppliers per SKU, and flags products requiring price adjustments — all in seconds.

# 🔧 Technical Architecture

┌─────────────────┐     ┌──────────────────┐     ┌─────────────────┐
│  Data Ingestion │────▶│  Logic Engine    │────▶│  Export Module  │
│  (Excel Upload) │     │  (Cost Analysis) │     │  (Formatted XLS)│
└─────────────────┘     └──────────────────┘     └─────────────────┘
         │                       │                         │
    Excel Files          Pandas DataFrames          XlsxWriter Output
    (3 sources)          (Merge/Calculate)          (Conditional Format)

# Core Dependencies:
pandas>=1.3.0       # Data manipulation and analysis
numpy>=1.20.0       # Numerical operations
xlsxwriter>=3.0.0   # Advanced Excel formatting

# 🚀 Getting Started
1. Prerequisites

Python 3.8+ installed (or Google Colab account - recommended)
Input Files in Excel format:

2. Installation
Google Colab (Recommended for non-technical users)

> Open the Colab notebook
> Click Runtime → Run all
> Upload your Excel files when prompted
> Download the generated report

# 🎓 Use Cases
1. Regular Pricing Reviews
Scenario: Monthly pricing audits for 800-SKU catalog
Outcome: Systematic margin protection vs. ad-hoc reactions

2. Supplier Negotiation Prep
Scenario: Annual contract renewal with Supplier A
Outcome: Data-backed negotiating position

3. New Product Onboarding
Scenario: Evaluating 50 new SKUs for catalog addition
Outcome: Prevent adding unprofitable products

5. Market Price Change Response
Scenario: Competitor drops prices on 20 core products
Outcome: Rapid competitive response capability
