
# Project Description: Data Analysis and Statistics for Organisational Metrics

This project consists of a series of functions designed to process and analyze data from a CSV file containing information about various organisations across different countries. The code includes functions to calculate key statistics and correlations related to organisational performance, with a focus on employee numbers, median salaries, and profits. Each function performs a specific analysis, and the results can be used to gain insights into the relationship between various organisational factors.

## Functions Overview:

### 1. `file_content(csvfile)`:
   - This function reads the contents of a CSV file, processes it by splitting lines into lists, and converts numeric values where applicable. It returns the processed data as a list of lists.
   - The function also handles missing data by appending 'null' when values are missing.

### 2. `calculate_max_min(csvfile, country)`:
   - This function identifies the organisations in a specific country (provided as input) that were founded between 1981 and 2000. It then determines which organisation has the highest and lowest number of employees, returning these organisations' names.

### 3. `standard_deviation(csvfile, country)`:
   - This function calculates the standard deviation of the median salaries of organisations in a specific country, as well as the standard deviation of median salaries across all countries. It provides insights into salary distribution within a country and globally.

### 4. `calculate_ratio(csvfile, country)`:
   - This function calculates the ratio of profit increases to profit decreases between the years 2020 and 2021 for organisations in a specific country. It helps measure the overall profit performance and financial stability of organisations within that country.

### 5. `correlation(csvfile, country)`:
   - This function computes the correlation between median salary and profit for organisations in a specific country. It helps identify potential relationships between salary levels and profitability in the selected country.

### 6. `main(csvfile, country)`:
   - This is the main function that integrates all the above functions. It processes the data and calls the individual functions to calculate the following for a specific country:
     - The organisation with the highest and lowest number of employees.
     - The standard deviation of median salaries for the country and globally.
     - The ratio of profit increase vs. profit decrease.
     - The correlation between median salary and profit.
   - The results are returned as a tuple containing all the calculated metrics.
