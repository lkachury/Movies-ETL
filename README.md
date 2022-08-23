# Movies-ETL

## Overview

Background:
"Amazing Prime loves the dataset and wants to keep it updated on a daily basis. Britta needs your help to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. You’ll need to refactor the code from this module to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database."

## Resources
### Data Source 
- ?

### Software
- Python 3.7.6
- PostgreSQL and pgAdmin 6.8
- Visual Studio Code 1.69
- Conda 4.13.0
- Jupyter Notebook 
- Dependencies:
  - Python JSON Library
  - Python Pandas Library
  - Python Numpy Library
  - Python re Library
  - sqlalchemy Module 
  - psycopg2 Module

## Results

### Deliverable 1: Write an ETL Function to Read Three Data Files
Using Python, Pandas, the ETL process, and code refactoring, a function was written that reads in the three data files and creates three separate DataFrames.
The full Jupyter Notebook for this deliverable can be referenced here: [ETL_function_test.ipynb](https://github.com/lkachury/Movies-ETL/blob/main/ETL_function_test.ipynb)

An ETL function was written to read in the three data files with the following code:
![image](https://user-images.githubusercontent.com/108038989/186045392-8326d522-01ff-4845-98fa-23d1e78ea69a.png)

The function converts the Wikipedia JSON file to a Pandas DataFrame:
![image](https://user-images.githubusercontent.com/108038989/186045508-bd46e001-665d-462d-a4bd-46b59f8e3bc0.png)

The function converts the Kaggle metadata file to a Pandas DataFrame:
![image](https://user-images.githubusercontent.com/108038989/186045547-05d05aa5-9e23-4642-b1a2-91083b5dcc55.png)

The function converts the MovieLens ratings data file to a Pandas DataFrame:
![image](https://user-images.githubusercontent.com/108038989/186045585-3d0378d5-d651-4c4d-84c0-12876ed4ca54.png)

### Deliverable 2: Extract and Transform the Wikipedia Data
Using your knowledge of Python, Pandas, the ETL process, and code refactoring, extract and transform the Wikipedia data so you can merge it with the Kaggle metadata. While extracting the IMDb IDs using a regular expression string and dropping duplicates, use a try-except block to catch errors.

### Deliverable 3: Extract and Transform the Kaggle Data
Using your knowledge of Python, Pandas, the ETL process, and code refactoring, extract and transform the Kaggle metadata and MovieLens rating data, then convert the transformed data into separate DataFrames. Then, you’ll merge the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create the movies_df DataFrame. Finally, you’ll merge the MovieLens rating data DataFrame with the movies_df DataFrame to create the movies_with_ratings_df.

### Deliverable 4: Create the Movie Database
Use your knowledge of Python, Pandas, the ETL process, code refactoring, and PostgreSQL to add the movies_df DataFrame and MovieLens rating CSV data to a SQL database.
