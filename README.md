# Vendor-Performance-Analysis
This project focuses on comprehensive exploratory data analysis (EDA) of large-scale inventory and vendor transactions in a business environment. Utilizing over 
**1 crore **(**10 million**) dataset entries, the analysis uncovers actionable insights to optimize inventory management, vendor relationships, and profitability.

Absolutely! Here’s a tailored README.md file you can use for your GitHub project, based on your detailed report and the datasets you've analyzed.

# Exploratory Data Analysis of Inventory & Vendor Transactions

## Overview

This project focuses on comprehensive exploratory data analysis (EDA) of large-scale inventory and vendor transactions in a business environment. Utilizing over **1 crore (10 million)** dataset entries, the analysis uncovers actionable insights to optimize inventory management, vendor relationships, and profitability.

## Datasets Analyzed

The EDA leverages the following key datasets:

1. **begin_inventory** - Opening inventory records.
2. **end_inventory** - Closing inventory records.
3. **purchase_prices** - Historical purchase price data by product and vendor.
4. **purchases** - Transaction logs of all purchases.
5. **sales** - Detailed sales transactions.
6. **vendor_invoice** - Corresponding invoices linked to vendor purchases.

## Key Findings

- **Gross Profit Volatility:** Identified instances of gross profit dropping to -1.25M due to high costs or discounting; highlighted transactions leading to losses (gross profit ≤ 0).
- **Profit Margin Issues:** Revealed negative margins (≤ 0 or -∞), often where no revenue was booked or total costs exceeded sales.
- **Freight Costs:** Observed a broad range in freight costs (₹0.09 to ₹2,57,000), pointing to both bulk shipments and potential logistics inefficiencies.
- **Bulk Order Advantage:** Vendors placing large orders achieved the lowest unit prices, confirming that volume-based pricing improves margins if managed properly.
- **Slow-Moving Inventory Impact:** Noted that slow-moving items increase storage costs and reduce cash flow efficiency, negatively impacting overall profitability.
- **Vendor Performance:** Statistical analysis of profit margin demonstrated significant gaps between high- and low-performing vendors. (Top Vendors 95% CI: 55.51–62.72, Mean: 59.12)

## Project Structure

```
vendor-performance-analysis/
│
├── data.zip/                               # Raw input datasets (not public)
├── EDA.ipynb/                              # Jupyter notebooks for data analysis
├── Vendor Performance Analysis.ipynb/      # Python scripts (for cleaning, processing, stats)
├── ingestion_db.py/                        #Python script to record the logs
├── ingestion_db.log/                       #Log file
├── Dashboard_VPA.png/                      #Screenshot of Power BI Dashboard
├── REPORT_Exploratory Data Analysis/       # Detailed project and EDA reports
└── README.md/                              # This file is the overall summarized content of the findings
```

## How to Use

1. **Clone this repository** to your machine.
2. Add the dataset files (`CSV` or similar) into the `data/` directory.
3. Open any Jupyter notebook from `notebooks/` to review or repeat the analysis.
4. For detailed procedures or additional findings, refer to the full report in `report/`.

## Recommendations

- **Negotiate Vendor Bulk Discounts:** Encourage larger order sizes for better pricing.
- **Manage Slow-Moving Inventory:** Proactive identification and clearance can reduce costs and improve cash flow.
- **Optimize Freight:** Review high-cost logistics for cost-saving opportunities.
- **Vendor Segmentation:** Use analysis to identify and improve terms with underperforming vendors.
- **Analyze Loss-Making Transactions:** Scrutinize cases of negative profit to guide process improvements.

## Report

A detailed summary of analyses, insights, and recommendations is available in:

- `report/REPORT_Exploratory-Data-Analysis.docx`

## Contributions

Contributions, suggestions, and improvements are welcome! Please open an issue or create a pull request.
