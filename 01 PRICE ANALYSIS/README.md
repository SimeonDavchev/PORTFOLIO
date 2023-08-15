# Price-comparison-HSN# PROJECT 1: Price comparison HSN

**Confidentiality NOTE:** Prices are publicly available, however in order to not to share confidential information items will be renamed, brand names and invoices are kept under .gitignore, and some functions are left as comments in order not to expose information with outputs. 


**PART I: SUMMARY OF PROCESS AND METHODS USED**

This project originated from my manager asking for help when trying to compare 
the prices of one of our suppliers. The idea of the programme is to provide analysis 
and visualisation of how prices have changed. 

The code consists of 4 main parts:

1. **Sourcing the files**: the public version just uses files from a folder as most of the receipts were already sorted in a folder.
Future NOTE: If this was not the case, it can be done by scrapping the email with the win32.client library.

2. **Extracting the data from invoices**: this proved to be by far the most challenging part as the only way in which the information was available was .pdf and formatting, order and spacing were inconsistent, however some patterns in brand name placement and units were used to extract information reliably. Adaptation for some categories was needed as interpretation of price was different depending on the item and unit used.
Future NOTE: Use RegEx next time.

3. **Filtering the data**: part of this was imbedded in the information extraction function as some of the invoices were send without prices. This step also lead to modifications of the exraction function, to help with corner cases of formatting.

4. **Analysis and visualisation**: the owners were interested in 2 questions:

   4.1 How much has the total price or the invoices risen?

   4.2 Which items have increased the most in price?

   (4.3) I allowed myself however to include a third question: Which items' price increase has contributed the most to the specific orders of the hotel? Here in order to compare how different items affect the total increase, I defined their impact as the quantity ordered times the price increase at the time)

A really interesting problem that was discovered in this step was that there were 
invoices which had much lower prices than the rest, which was altering the analysis. Later it was discovered that it is due to the fact that there is a separate type of orders, that were in the invoices and there was no way to tell them appart besides with the magnitude of the price, so both visual inspection and k-means clustering was used to separate them out.


**PART II: RESULTS AND INTERPRETATION**




