
# PROJECT 1: Price Analysis

This project aims to provide a comprehensive analysis and visualization of price changes for a supplier's items over time. It's a practical solution to a real-world challenge, offering insights that can be instrumental for business decisions.

## Confidentiality NOTE:
Prices are publicly available. However, to ensure confidentiality:
- Items are renamed.
- Brand names and invoices are kept under `.gitignore`, which itself was hidden.
- Some functions are commented out to prevent exposing sensitive outputs.

## PART I: SUMMARY OF PROCESS AND METHODS USED

The project was inspired by a request from my manager to compare the prices of one of our suppliers. The code has four main components:

1. **Sourcing the files**: For this public version, files are sourced from a folder where most receipts were already organized.
   - *Future NOTE*: Email scraping can be done using the `win32.client` library if necessary.
2. **Extracting data from invoices**: The primary challenge was extracting data from inconsistently formatted PDF invoices. Reliable extraction was achieved by identifying patterns in brand name placements and units.
   - *Future NOTE*: Consider using RegEx for improved extraction.
3. **Filtering the data**: Invoices without prices were filtered out. The extraction function was refined for specific formatting corner cases.
4. **Analysis and visualization**: The primary questions addressed were:
   - 1: Which items have seen the most significant price increase?
   - 2: How has the total invoice price changed over time?
   - (3): An additional analysis was conducted to determine the items whose price increase had the most impact on specific hotel orders.

During the analysis, it was observed that some invoices had significantly lower prices. It was determined that these belonged to a different order type, distinguishable only by price. Both visual inspection and K-means clustering were used to segregate them.

## PART II: RESULTS AND INTERPRETATION

The focus here is on the latter two questions as they provide the most actionable insights:

**Question 2**: Has the invoice amount increased?
![Invoice Increase Analysis](https://github.com/SimeonDavchev/PORTFOLIO/assets/113254668/13198a3d-5bb8-435a-8c48-a8897e6d9a5d)

The analysis, detailed in the code, revealed two types of invoices. K-means clustering helped segregate them. The green cluster, which was the focus, shows that on average, the bill has risen by ~100EUR per order.

**Question 3**: Which items have had the most impact on price changes?

Arguably there are many ways to do this, but the way I did it is to multiply the changes in price per the quantity ordered as they occur and call this the 'impact' (i.e. if eggs increased with 1 EUR by 6 June but 10 EUR by today, the values before 6 June will be multiplied by 1 not 10)
and then do a ordered bar chart to visualise it.

![Items Impact Analysis](https://github.com/SimeonDavchev/PORTFOLIO/assets/113254668/de5ee2e7-44bb-49d8-b25c-64ae7830b5c5)

Item009 stands out. While it ranked 11th in price change, its overall impact, when weighted by order quantity, accounted for almost 1/5 of the total price difference over the year. Other notable items include 018 and 013. Focusing on these three items could yield significant cost-saving effects.

## Conclusion and Future Work
The project successfully provides insights into price changes and their impacts. By focusing on a few key items, businesses can make informed decisions to achieve substantial savings. For future iterations, refining data extraction techniques and expanding the dataset could provide even deeper insights.

