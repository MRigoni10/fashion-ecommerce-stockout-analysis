# Fashion E-Commerce Stockout & Pricing Analysis (ASOS)

An exploratory data analysis pipeline analyzing size-level stockout rates and quantifying lost revenue potential across fashion brands on the ASOS platform.

## Overview
Broken size curves in fashion retail lead to phantom inventory and lost sales. This project evaluates an ASOS product catalog (~18k SKUs) to detect out-of-stock sizes and segment brands based on average price and fulfillment performance[cite: 1].

## Pipeline
- **Dataset:** ASOS Product Catalog (~18,300 product listings)[cite: 1].
- **Data Prep:** Cleaned price anomalies, extracted structured brand names from text descriptions, and mapped key third-party brands[cite: 1].
- **Feature Engineering:** Parsed comma-delimited size availability strings to compute accurate stockout counts and normalized stockout rates ($0.0$ to $1.0$)[cite: 1].
- **Revenue Impact:** Estimated lost sales per SKU by multiplying the unit price by the number of out-of-stock size variants[cite: 1].

## Key Results
- **Brand Strategy Matrix:** Mapped brands across pricing and availability quadrants to isolate high-demand, high-stockout lines[cite: 1].
- **Fulfillment Bottlenecks:** Premium categories (outerwear, leather lines) displayed the highest revenue leakage due to unfulfilled core sizes[cite: 1].
- **Actionable Takeaway:** Identified priority brands that require higher reorder depths and automated restock triggers[cite: 1].

## Visual Output
![Brand Strategy Matrix](brand_strategy_matrix.png)

## How to Run the Project
The complete code is available in the interactive notebook. You can run it with a single click:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1NgnHWm1v4X6lMRmCFbg_IdE9hfDdRDi1#scrollTo=tUTjonLuR-Uh)
