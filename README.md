# statistics-assessment
its a formative assessment from entry elevate in statistics
Summary
This analysis aimed to understand the price per square foot of properties in Bangalore. Basic EDA provided insights into the data structure, and various methods were used to detect and remove outliers. The normality of the data was checked and addressed through transformations. Finally, correlations between variables were explored to identify significant relationships.

This comprehensive approach ensures a thorough understanding and preparation of the data, making it suitable for further modeling and analysis.
Formative Assessment: Bangalore House Price Analysis
Q1. Perform Basic EDA (Exploratory Data Analysis)
To start the analysis, the dataset was loaded and the following steps were performed:

Viewing the first and last few rows: This helps in understanding the structure and contents of the dataset.
Checking the shape and column names: Provides information on the number of rows and columns, and the names of the columns.
Identifying numerical and categorical columns: Distinguishes between the types of data.
Checking for duplicate rows: Ensures data quality by identifying and quantifying duplicate entries.
Displaying basic statistics of numerical columns: Summary statistics such as mean, median, standard deviation, etc., are calculated to understand the distribution and central tendency of the data.
Creating histograms and box plots for the price_per_sqft column: Visualizes the distribution and identifies potential outliers.
Creating histograms and box plots for all numerical columns: Similar visualization for all numerical features to detect outliers and understand distributions.
Q2. Detect and Remove Outliers
Outliers can skew the analysis, so they were detected and removed using various methods:

Mean and Standard Deviation Method: Data points outside the range of mean ± 3 standard deviations were considered outliers.
Percentile Method: Data points below the 5th percentile and above the 95th percentile were treated as outliers.
IQR (Interquartile Range) Method: Data points outside the range of Q1 - 1.5IQR to Q3 + 1.5IQR were identified as outliers.
Z Score Method: Data points with Z scores greater than 3 or less than -3 were considered outliers.
Q3. Create Box Plot to Determine Best Outlier Removal Method
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
