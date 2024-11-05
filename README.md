# Weather Data Analysis

This project provides a step-by-step approach to analyzing weather data with Python. The dataset used includes various weather attributes, such as Wind Speed, Weather Condition, Visibility, Pressure, Relative Humidity, and Temperature. This analysis includes tasks such as finding unique values, filtering records based on conditions, computing statistical measures, and renaming columns.

## Questions & Solutions

### Q1) Find all unique ‘Wind Speed’ values in the data.
- Displayed the top 2 records of the dataframe for reference.
- Used the `nunique()` function on the 'Wind Speed' column to determine that there are 34 unique values.
- Retrieved and displayed these values using the `unique()` function.

### Q2) Count the occurrences of ‘Weather is exactly Clear’.
- Explored three methods: `value_counts`, filtering, and `groupby` with `get_group` to confirm that there are 1326 instances of clear weather.

### Q3) Count the number of times ‘Wind Speed’ was exactly 4 km/h.
- Used filtering on the 'Wind Speed_km/h' column to find 474 instances with exactly 4 km/h.

### Q4) Check for Null (Missing) Values in the data.
- Used `isnull()` and `notnull()` functions to confirm no missing values in any column.

### Q5) Rename the column ‘Weather’ to ‘Weather Condition’.
- Renamed 'Weather' to 'Weather Condition' using the `rename()` function with `inplace=True` for permanence.

### Q6) Calculate the mean ‘Visibility’.
- Used the `mean()` function on 'Visibility_km' to obtain a mean of 27.66.

### Q7) Calculate the Standard Deviation of ‘Pressure’.
- Applied `std()` on 'Press_kPa' resulting in a standard deviation of 0.844.

### Q8) Calculate the Variance of ‘Relative Humidity’.
- Applied `var()` on 'Rel Hum_%' yielding a variance of 286.24.

### Q9) Find all instances where ‘Snow’ was recorded.
- Utilized both `value_counts()` and filtering to find 390 instances with ‘Snow’.

### Q10) Find all instances with ‘Wind Speed above 24’ and ‘Visibility is 25’.
- Used comparison operators and the `&` operator for these combined conditions, resulting in 308 matching records.

### Q11) Calculate the Mean value of each column grouped by ‘Weather Condition’.
- Used `groupby()` with `mean()` to obtain the average values of each column for each weather condition.

### Q12) Calculate Minimum & Maximum values of each column for each ‘Weather Condition’.
- Used `groupby()` with `min()` and `max()` to find minimum and maximum values of each column for each weather condition.

### Q13) Show all records where Weather Condition is ‘Fog’.
- Filtered the data to show 150 records with ‘Fog’ as the Weather Condition.

### Q14) Find all instances where ‘Weather is Clear’ or ‘Visibility is above 40’.
- Applied OR (`|`) operator with two conditions to retrieve 3027 records matching either condition.

### Q15) Find all instances where:
  - A. ‘Weather is Clear’ and ‘Relative Humidity is greater than 50’
  - B. ‘Visibility is above 40’
- Used combined conditions with AND (`&`) and OR (`|`) operators to filter for 2921 matching records.

## Dependencies
- Pandas
- NumPy

## Usage
1. Clone the repository.
2. Run the Python script in your preferred environment.
3. Review the analysis output for insights on weather patterns in the data.

## License
This project is licensed under the MIT License.
