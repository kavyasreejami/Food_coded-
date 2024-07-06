# Food_coded-
The code provided performs data cleaning on a dataset by handling missing values and removing duplicates.

Loading the Data:

The dataset is loaded from a CSV file using pandas.read_csv.
Removing Duplicate Rows:

Duplicate rows in the dataset are removed using drop_duplicates. This ensures that each row in the dataset is unique.
Handling Missing Values:

For each column in the dataset, the code checks the data type:
If the column is of type object (usually representing categorical data), missing values are filled with the mode (the most frequent value in the column).
If the column is numerical, missing values are filled with the mean of the column.
This step ensures that there are no missing values in the dataset, which can be crucial for many machine learning algorithms and data analysis tasks.
Removing Duplicate Columns:

The code checks for and removes any duplicate columns using data.loc. This ensures that each column in the dataset is unique and avoids redundant information.
Saving the Cleaned Data:

The cleaned dataset is saved to a new CSV file using data.to_csv. This allows the cleaned data to be easily accessed and used for further analysis or modeling.
Overall, the code prepares the dataset for analysis by ensuring it is free of missing values and duplicates, which helps in maintaining data integrity and quality.
