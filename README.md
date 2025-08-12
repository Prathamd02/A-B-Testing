# A/B Testing Analysis in Python

## Overview
This project applies A/B testing techniques to compare the performance of two advertising campaigns: **Control** and **Test**. Using campaign data, we evaluate engagement, conversion rates, and cost-effectiveness to determine which campaign is more suitable for different marketing strategies.

## Goal
To figure out:
- Which campaign reaches and engages more users
- Which one is better at turning engagement into purchases
- Which is more efficient in terms of money spent

## Dataset Information
Two datasets are used:
- **control_group.csv** – Data for the control campaign
- **test_group.csv** – Data for the test campaign  

Each dataset contains columns such as Date, Amount Spent, Impressions, Reach, Website Clicks, Searches, Content Viewed, Added to Cart, and Purchases.

## Steps Followed
1. **Data Import & Cleaning**  
   Load CSV files into Pandas, handle missing values by filling them with the mean of each column.

2. **Merging & Sorting Data**  
   Combine both datasets using an outer join, sort them chronologically, and reset the index for consistency.

3. **Metric Comparison**  
   Compare impressions, clicks, content views, add-to-cart counts, and purchases between campaigns.

4. **Insights**  
   Evaluate conversion rates, spending efficiency, and engagement depth.

5. **Final Recommendation**  
   Decide which campaign is better suited for broad promotion and which is more effective for targeted marketing.

## How to Run
```bash
# Clone this repository
git clone https://github.com/your-username/ab-testing-python.git
cd ab-testing-python

# Install required packages
pip install pandas plotly

# Open the analysis notebook
jupyter notebook "AB_Testing_Analysis.ipynb"
