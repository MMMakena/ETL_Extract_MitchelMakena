# ETL_Extract_MitchelMakena

## Description
- On a generated synthetic data`event_dataset,csv`, this notebook, `etl_extract.ipynb`, simulates the ETL (Extract, Transform, Load) extraction process. 
- Both full and incremental data extraction are demonstrated, which is a standard procedure in data pipelines to process only entries that have been added or altered since the prior run. 
- In order to replicate a real-world situation where data is appended, the incremental extraction is mimicked by monitoring the amount of rows processed in a text file`last_extraction.txt`.

## Tool used
- Python: The primary programming language for ETL process scripting.
- Here, the dataset is loaded and processed using Pandas, a robust Python tool for data manipulation and analysis.
- This code is developed and run in an interactive computing environment called Jupyter Notebook, which enables a step-by-step illustration of the ETL procedure.

## How to reproduce:
### How to run the notebook:
- Install Dependencies: Make sure your Python environment has pandas installed.  If not, pip can be used to install it: `pip install pandas`
- Run Jupyter Notebook: Navigate to the directory where you saved `etl_extract.ipynb`, and start the Jupyter Notebook
- Open and Run: Click on `etl_extract.ipynb` to launch it in the Jupyter Notebook interface that appears in your web browser.  After that, you can either run each cell individually or all the cells at once by selecting `Cell > Run All` from the menu.

### Where the data comes from:
- The dataset used for this lab is hardcoded directly within the `etl_extract.ipynb` notebook
- Details such as Event Type, Location,  Attendance and more are all represented in this sample event data.

## Transformation for the data
### Transformation on the full extraction data
- First, Make a copy of the data. Applied 3 transformation requirements; Cleaning,Enrichment and Structural.
- With the Cleaning, I checked if there were any missing values using the `if-else`. There were missing values and I filled them. I also looked for duplicates. Had a 50 rows before and after transformation.
- With the Enrichment, I calculated the total cost,and made it into a column,by multiplying the attendees and cost per attendees. I rounded the decimals to 2.
- With the Structural, I change the datetime into a string format.
- I did a sample of the data to ensure all the transformations worked. Then created the `transformed_full.csv`.

### Transform on the incremental extraction data
- I performed the same requirements on this data. There difference is in the row count, 15.
- Then created the `transformed_incremental.csv`.
