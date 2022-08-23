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
<br /> ![image](https://user-images.githubusercontent.com/108038989/186045392-8326d522-01ff-4845-98fa-23d1e78ea69a.png)

The function converts the Wikipedia JSON file to a Pandas DataFrame:
<br /> ![image](https://user-images.githubusercontent.com/108038989/186045508-bd46e001-665d-462d-a4bd-46b59f8e3bc0.png)

The function converts the Kaggle metadata file to a Pandas DataFrame:
<br /> ![image](https://user-images.githubusercontent.com/108038989/186045547-05d05aa5-9e23-4642-b1a2-91083b5dcc55.png)

The function converts the MovieLens ratings data file to a Pandas DataFrame:
<br /> ![image](https://user-images.githubusercontent.com/108038989/186045585-3d0378d5-d651-4c4d-84c0-12876ed4ca54.png)

### Deliverable 2: Extract and Transform the Wikipedia Data
Using Python, Pandas, the ETL process, and code refactoring, the Wikipedia data was extracted and transformed to merge it with the Kaggle metadata. While extracting the IMDb IDs using a regular expression string and dropping duplicates, a try-except block to catch errors was used.
The full Jupyter Notebook for this deliverable can be referenced here: [ETL_clean_wiki_movies.ipynb]()





### Deliverable 3: Extract and Transform the Kaggle Data
Using Python, Pandas, the ETL process, and code refactoring, the Kaggle metadata and MovieLens rating data were extracted and transformed to convert into separate DataFrames. The Kaggle metadata DataFrame was merged with the Wikipedia movies DataFrame to create the movies_df DataFrame. The MovieLens rating data DataFrame was merged with the movies_df DataFrame to create the movies_with_ratings_df.
The full Jupyter Notebook for this deliverable can be referenced here: []()



### Deliverable 4: Create the Movie Database
using Python, Pandas, the ETL process, code refactoring, and PostgreSQL the movies_df DataFrame and MovieLens rating CSV data were added to a SQL database.
The full Jupyter Notebook for this deliverable can be referenced here: []()



