# PandasAssignment

Q1. How do you load a CSV file into a Pandas DataFrame?
Ans: ```
  import pandas as pd
  df = pd.read_csv({csv_file_path})
```

Q2. How do you check the data type of a column in a Pandas DataFrame?
`df.dtypes`

Q3. How do you select rows from a Pandas DataFrame based on a condition?
Ans: using `df.loc({condition})` in pandas.

Q4. How do you rename columns in a Pandas DataFrame?
Ans: `df.rename(columns = {'PassengerId': 'passengerId'}, inplace = True)`

Q5. How do you drop columns in a Pandas DataFrame?
ans: `df_manual.drop([{column_name}], axis=1, inplace=True)`

Q6. How do you find the unique values in a column of a Pandas DataFrame?
Ans: `df.{column_name}.unique()`

Q7. How do you find the number of missing values in each column of a Pandas DataFrame?
Ans: `df.isnull().sum()` will give count for each columns having missing values.

Q8. How do you fill missing values in a Pandas DataFrame with a specific value?
ans: `df.fillna({value})` this will fill all NA/None with the mentioned value.

Q9. How do you concatenate two Pandas DataFrames?
Ans: `pd.concat([df1, df2], axis=0)` axis= 0 for vertical concatnenation, axis = 1 for horizontal concatnation.

Q10. How do you merge two Pandas DataFrames on a specific column?
Ans: `df1.merge(df2[{columnName}])`

Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function?
Ans: `df.groupby({column_name}).sum()`

Q12. How do you pivot a Pandas DataFrame?
Ans: 'df.pivot(index, column, values)' => to transform our already existing column and values.

Q13. How do you change the data type of a column in a Pandas DataFrame?
Ans: 'df.astype(dtype)'

Q14. How do you sort a Pandas DataFrame by a specific column?
Ans: `df.sort_values(by=[{column_list}])`

Q15. How do you create a copy of a Pandas DataFrame?
Ans: `df_copy = df.copy()`

Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?
Ans: `df[{condition}]`

Q17. How do you calculate the mean of a column in a Pandas DataFrame?

Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame?

Q19. How do you calculate the correlation between two columns in a Pandas DataFrame?

Q20. How do you select specific columns in a DataFrame using their labels?

Q21. How do you select specific rows in a DataFrame using their indexes?
Ans: `df.iloc[[{indexed}]]`

Q22. How do you sort a DataFrame by a specific column?
Ans: `df.sort_values(by=[{column_list}])`

Q23. How do you create a new column in a DataFrame based on the values of another column?
Ans: `df[{new_column}] = {return object with new column}`

Q24. How do you remove duplicates from a DataFrame?
Ans: `df.drop_duplicates()`

Q25. What is the difference between .loc and .iloc in Pandas?
Ans: Both are used to filter out rows in pandas dataframe. `loc` is label based and `iloc` is index based.
