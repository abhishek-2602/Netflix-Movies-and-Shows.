
 Netflix Titles – Data Cleaning (Task 1)

 Task 1: Data Cleaning and Preprocessing

This project is part of a Data Analyst Internship assignment. The objective is to clean and preprocess a raw dataset from Netflix to make it ready for further analysis.


 Dataset Used
**File Name**: `netflix_titles.csv`
**Source**: [Kaggle - Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)


 Tools Used
- Python
- Pandas
- Jupyter Notebook 



Task Objectives
- Identify and handle missing values
- Remove duplicate records
- Standardize column names and text data
- Convert inconsistent date formats
- Fix incorrect data types
- Save and document the cleaned dataset


Cleaning Steps Performed

1. **Loaded the dataset** using Pandas and inspected the structure  
2. **Handled missing values**:
   - Filled `director`, `cast`, and `country` missing values with `'Unknown'`
   - Filled missing `rating` with `'Not Rated'`
   - Used `errors='coerce'` to handle invalid dates in `date_added`
3. **Removed duplicate rows** using `.drop_duplicates()`  
4. **Standardized column headers**:
   - Converted all column names to lowercase and replaced spaces with underscores  
5. **Cleaned categorical columns**:
   - Standardized values in `type`, `rating`, and `country`  
6. **Converted `date_added`** to proper datetime format  
7. **Checked and corrected data types** for `release_year` and others  
8. **Exported the cleaned dataset** to a new CSV file `netflix_titles_cleaned.csv`



 Files in This Repo
- `netflix_titles.csv`: Original dataset  
- `netflix_cleaning.ipynb`: Jupyter Notebook with cleaning code  
- `netflix_titles_cleaned.csv`: Final cleaned dataset  
- `README.md`: Task summary and documentation  



 Key Learnings
- Handling missing, inconsistent, and duplicate data is crucial before analysis  
- Used `fillna()`, `drop_duplicates()`, and `to_datetime()` with `errors='coerce'`  
- Gained hands-on experience in preparing raw data for modeling and visualization  



