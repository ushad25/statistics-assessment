# Statistics Assessment

## Summary
This analysis aimed to understand the price per square foot of properties in Bangalore. Basic Exploratory Data Analysis (EDA) provided insights into the data structure, and various methods were used to detect and remove outliers. The normality of the data was checked and addressed through transformations. Finally, correlations between variables were explored to identify significant relationships. This comprehensive approach ensures a thorough understanding and preparation of the data, making it suitable for further modeling and analysis.

## Formative Assessment: Bangalore House Price Analysis

### Q1. Perform Basic EDA (Exploratory Data Analysis)
To start the analysis, the dataset was loaded, and the following steps were performed:
- **Viewing the First and Last Few Rows:** This helps in understanding the structure and contents of the dataset.
- **Checking the Shape and Column Names:** Provides information on the number of rows and columns, and the names of the columns.
- **Identifying Numerical and Categorical Columns:** Distinguishes between the types of data.
- **Checking for Duplicate Rows:** Ensures data quality by identifying and quantifying duplicate entries.
- **Displaying Basic Statistics of Numerical Columns:** Summary statistics such as mean, median, standard deviation, etc., are calculated to understand the distribution and central tendency of the data.
- **Creating Histograms and Box Plots for the `price_per_sqft` Column:** Visualizes the distribution and identifies potential outliers.
- **Creating Histograms and Box Plots for All Numerical Columns:** Similar visualization for all numerical features to detect outliers and understand distributions.

### Q2. Detect and Remove Outliers
Outliers can skew the analysis, so they were detected and removed using various methods:
- **Mean and Standard Deviation Method:** Data points outside the range of mean ± 3 standard deviations were considered outliers.
- **Percentile Method:** Data points below the 5th percentile and above the 95th percentile were treated as outliers.
- **IQR (Interquartile Range) Method:** Data points outside the range of Q1 - 1.5IQR to Q3 + 1.5IQR were identified as outliers.
- **Z Score Method:** Data points with Z scores greater than 3 or less than -3 were considered outliers.

### Q3. Create Box Plot to Determine Outliers
- **Box Plot Creation:** A box plot was created to visually inspect the distribution of the `price_per_sqft` and other numerical columns. This plot helps in identifying any remaining outliers after initial removal steps.

## Conclusion
The analysis provided valuable insights into the price per square foot of properties in Bangalore. By performing EDA, detecting and removing outliers, and checking for data normality, the data was prepared for further modeling and analysis. The use of various outlier detection methods and visualizations ensured a robust understanding of the dataset and its characteristics.

mine Best Outlier Removal Method
Box plots were created for each outlier removal method to visually inspect their effectiveness.

Mean and Standard Deviation Method: If significant outliers remain, this method might not be effective.
Percentile Method: Effective in removing extreme values but may also remove valid data points.
IQR Method: Typically effective for normally distributed data, removing points outside the middle 50% range.
Z Score Method: Standardizes data and removes extreme deviations, effective for normally distributed data.
Q4. Check Normality and Transform Data
Histogram: The distribution of the price_per_sqft column was visualized using a histogram.
Skewness and Kurtosis: Calculated before and after transformations to quantify the asymmetry and peakedness of the data distribution.
Log Transformation: Applied to reduce skewness and make the distribution more normal-like. Post-transformation skewness and kurtosis were recalculated to assess the improvement.
Q5. Correlation and Heatmap
Correlation Matrix: Calculated to quantify the linear relationships between numerical variables.
Heatmap: Visualized the correlation matrix to easily identify strong positive or negative correlations between features.
Q6. Scatter Plots to Check Correlations
Scatter Plots: Created for pairs of variables to visually inspect the strength and direction of their relationships.
