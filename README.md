# Handling-Missing-Value
1. Drop rows or columns that have a missing value - df.dropna()
2. Drop rows or columns, on the basis a missing value frequency - df.dropna(how='all')
3. Drop rows or columns based on a threshold value -- For instance, “thresh=4” means that the rows that have at least 4 non-missing values will be kept. The other ones will be dropped. - df.dropna(thresh=4)
4. Drop based on a particular subset of columns  - df.dropna(subset=['column1','column2'])
5. Fill with a constant value - df.fillna(0)
6. Fill with an aggregated value - df.fillna(df['column1'].mean()) 
7. Replace with the previous or next value  - df.fillna(method='bfill')
8. Fill by using another data frame that have same columns  - df.fillna(df2) 
9. Fill value with predicted value, or generated by ML algorithm with interpolation
