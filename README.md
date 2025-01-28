### Falak Shahzad 
###### Roll No 163
###### BsAi 1C

# Summary of Steps

1. **Imported pandas library**
    ```python
    ```

2. **Loaded the dataset from 'dirty_cafe_sales.csv'**
    ```python
    df = pd.read_csv('dirty_cafe_sales.csv')
    df
    ```

3. **Displayed the first few rows of the dataframe**
    ```python
    df.head()
    ```

4. **Displayed the last 9 rows of the dataframe**
    ```python
    df.tail(9)
    ```

5. **Displayed the columns of the dataframe**
    ```python
    df.columns
    ```

6. **Renamed columns 'Item' and 'Quantity' to 'A'**
    ```python
    df.rename(columns={'Item':'A','Quantity':'A'}, inplace=True)
    ```

7. **Checked for missing values in the dataframe**
    ```python
    df.isnull().sum()
    ```

8. **Displayed the columns of the dataframe again**
    ```python
    df.columns
    ```

9. **Grouped the dataframe by 'Quantity' and displayed descriptive statistics**
    ```python
    df.groupby('Quantity').describe()
    ```

10. **Plotted a bar chart of 'Quantity' value counts**
    ```python
    df['Quantity'].value_counts().plot(kind='bar', title="new", color='blue')
    ```

11. **Saved the dataframe to 'data3.csv'**
    ```python
    df.to_csv('data3.csv')
    ```

12. **Selected rows 1 to 4 of the 'Quantity' column**
    ```python
    df[1:4]['Quantity']
    ```

13. **Displayed the 'Quantity' column**
    ```python
    df['Quantity']
    ```

14. **Displayed descriptive statistics for all columns**
    ```python
    df.describe(include='all')
    ```

15. **Displayed the mode of the 'Quantity' column**
    ```python
    df['Quantity'].mode()[0]
    ```

16. **Checked for missing values in the dataframe again**
    ```python
    df.isnull().sum()
    ```

17. **Assigned the value 89 to variable `a`**
    ```python
    a = 89
    ```

18. **Checked for missing values in the 'Quantity' column**
    ```python
    df['Quantity'].isnull()
    ```

19. **Displayed the 'Price Per Unit' column and grouped by it to display descriptive statistics**
    ```python
    df['Price Per Unit']
    df.groupby('Price Per Unit').describe()
    ```

20. **Plotted a pie chart of 'Quantity' value counts**
    ```python
    df['Quantity'].value_counts().plot(kind='pie', title="new")
    ```