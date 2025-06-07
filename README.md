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
