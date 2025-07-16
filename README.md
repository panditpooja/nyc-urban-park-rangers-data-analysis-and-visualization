# Urban Park Rangers Data Analysis
## Description
This repository contains Python code and outputs in PDF format for analyzing the duties of Urban Park Rangers in New York City over time, specifically focusing on requests for animal assistance, relocation, and/or rescue. The dataset used for analysis is provided by the city of New York.

## Scenario Questions
Used the dataset to answer the following questions:
1. How has the number of animals sent to rehabilitators or animal care centers changed over time?
2. How has the type of animal being reported changed over time?
3. How has the source of information (call source) changed over time?

## Additional Considerations: 
- The dataset contains unnecessary information, so filtering and selection of relevant data points are crucial so I have provided thorough explanations and summaries in my python code and detailed PDF report.
## Project Overview
This project was conducted using Google Colab, an online platform for Jupyter notebooks that offers free GPU and TPU resources, making it ideal for data-intensive tasks and machine learning experiments.
## Project Steps:
1. **Subset Relevant Columns:**
   - Choose columns necessary for answering the dataset questions: 'Date and Time of initial call', 'Animal Class', 'Call Source', and '# of Animals'.
2. **Data Cleaning:**
   - Convert Date Column: Change the datatype of 'Date and Time of initial call' from 'Object' to 'DateTime' format for proper date handling.
   - Clean Animal Class Column: Extract and clean the 'Animal Class' column to ensure consistent and usable data by removing unwanted characters and keeping only relevant labels.
   - Handle Missing Values: Drop rows with missing values in the '# of Animals' column since they are minimal relative to the dataset size.
3. **Data Transformation:**
   - Add Year Column: Create a new column 'Report_Year' by extracting the year from the 'Date and Time of initial call' column. This facilitates annual trend analysis.
4. **Store Filtered Dataframe in Excel:**
   - Create a subset of the cleaned dataset containing only the columns 'Report_Year', '# of Animals', 'Animal Class', and 'Call Source'. This subset will serve as the importable table for further analysis in Python.
   - Save the filtered dataframe to a new Excel file named "Pooja_Output_File.xlsx" with a sheet named "Importable Table".
5. **Read and Inspect the "Importable Table" Dataset:**
   - Load the "Importable Table" dataset from the Excel file and inspect its structure and contents to ensure data was correctly saved.
6. **Perform Grouping and Aggregation:**
   - Use pandas to group and aggregate data to answer the specific three questions related to the dataset.
7. **Data visualization:**
   - Perform data visualization for each question to understand the trend over time effectively.
8. **Develop Publication Table:**
   - Create a publication-ready table that adheres to table anatomy guidelines and clearly presents the findings related to the three specific questions posed by the dataset.

## Expected Output:
1. Generate two tables:
   - Publication Table: Formatted with a caption following text and format considerations.
   - Importable Table: Includes only necessary columns ready to be imported into a Python Notebook.
2. Prepare final pdf report with publication table, importale table and python code snippet.

Note:  Raw data folder contains messy dataset to be analysed and also have data description file. The solutions folder contains python code and pdf report that answers all the three questions.

---
## ✍️ Author

**Pooja Pandit**  
Master’s Student in Information Science (Machine Learning)  
The University of Arizona  

[![GitHub](https://img.shields.io/badge/GitHub-panditpooja-black?logo=github)](https://github.com/panditpooja)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pooja--pandit-0077B5?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pooja-pandit-177978135/)  
