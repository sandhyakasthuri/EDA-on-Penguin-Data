# EDA-on-Penguin-Data
Exploratory Data Analysis

Data Overview:

The dataset contains information about penguins, including their species, island habitat, physical measurements, and sex.
There are a total of 344 entries with 7 columns: 'species', 'island', 'culmen_length_mm', 'culmen_depth_mm', 'flipper_length_mm', 'body_mass_g', and 'sex'.
The 'sex' column has missing values, which were removed during data cleaning. 

Data Cleaning:

Missing values were handled by dropping rows with missing values in any column. This ensured data integrity and completeness.

Species and Island: There are no missing values in the "Species" and "Island" columns, indicating that every entry in these columns has been properly recorded.

Physical Measurements (Culmen Length, Culmen Depth, Flipper Length, Body Mass): Each of these columns has 2 missing values. This suggests that for 2 entries in the dataset, measurements for culmen length, culmen depth, flipper length, and body mass were not recorded.

Sex: The "Sex" column has 10 missing values, indicating that the gender information is missing for 10 entries in the dataset.

There are different ways to handle the missing values.
Imputation: Filling missing values with mean, median, or mode values of the respective column.
Dropping: Removing rows or columns with missing values if they are not crucial for the analysis.
Advanced Techniques: Utilizing predictive models to estimate missing values based on other available data.
Impact on Analysis: It's essential to consider the impact of missing values on the analysis. Missing data may skew statistical analysis results or affect the performance of machine learning models if not handled properly. Therefore, careful consideration and appropriate handling of missing values are crucial to ensure the reliability and accuracy of the analysis results.

In this case, the number of missing values is not large, hence the rows and columns with missing values have been removed.

Erroneous values, such as '.' in the 'sex' column, were removed to maintain consistency and accuracy in the dataset.

Data Exploration:

Unique values for categorical features like 'species', 'island', and 'sex' were examined to understand the diversity within the dataset.
Relationships between numerical features were explored through scatter plots, revealing patterns and potential correlations between physical measurements.

Visualization:

Scatter plots were utilized to visualize the relationships between culmen length and depth, flipper length and body mass, etc.
Histograms were plotted to visualize the distribution of physical measurements for each penguin species, aiding in identifying patterns and potential classification features.

Scatter Plots:

Culmen Length vs. Culmen Depth: The scatter plot shows the relationship between the length and depth of the culmen (bill) for different penguin species. It reveals distinct clusters for each species, indicating differences in bill morphology. Adelie penguins generally have shorter and deeper bills compared to Gentoo and Chinstrap penguins.

Flipper Length vs. Body Mass: This scatter plot illustrates the relationship between flipper length and body mass for various penguin species. While there isn't a clear linear relationship, Gentoo penguins tend to have longer flippers and higher body mass compared to Adelie and Chinstrap penguins.

Culmen Depth vs. Body Mass: The scatter plot depicts the relationship between culmen depth and body mass. It shows that Gentoo penguins, despite having lower culmen depth, exhibit higher body mass compared to other species.

Culmen Length vs. Body Mass: This scatter plot indicates that Adelie penguins generally have shorter culmen lengths and lower body mass compared to Chinstrap and Gentoo penguins.
Histograms:

Histograms with histplots illustrate the distributions of physical measurements (culmen length, culmen depth, flipper length, and body mass) for each penguin species. These visualizations provide insights into the spread and overlap of measurements among different species. For example, the histograms reveal distinct peaks and variations in physical characteristics across species.
Histograms with histplots can help indicate the potential classification features by observing the overlap of the distribution of the various features, 
If all the features are overlapped with each other we cant quite observe the classification features.

Boxplots:
boxplots provide insights into the distribution of each feature across different penguin species, highlighting potential outliers and the general trend of each feature within each species. These visualizations can help identify patterns and differences in the physical characteristics of different penguin species

Culmen Length vs. Species:
The boxplot for culmen length shows that the Gentoo species has some outliers, indicating that there are a few data points that lie significantly away from the majority of observations for this species.
The skewness of the culmen length feature is slightly right, suggesting that the distribution is slightly skewed towards higher values, but not excessively so.

Culmen Depth vs. Species:
Similar to culmen length, the boxplot for culmen depth indicates that the Gentoo species has some outliers.
The skewness of the culmen depth feature is slightly right, indicating a slight skew towards higher values, although not extreme.

Flipper Length vs. Species:
The boxplot for flipper length does not mention any specific outlier observations for any species.
The skewness of feature flipper_length_mm is slightly right, as it doesn't have very high or very low values.

Body Mass vs. Species:
The boxplot for body mass mentions that the Adelie species has some outliers.
The skewness of feature body_mass_g is slightly right, as it doesn't have very high or very low values

Correlation Analysis:

A correlation matrix was generated to quantify the relationships between numerical features.
Strong positive correlations were observed between flipper length and body mass, as well as between culmen length and flipper length.
Moderate positive correlations were found between culmen length and body mass.
Weak negative correlations were observed between culmen length and culmen depth, as well as between culmen depth and body mass.

Insights and Interpretations:

Positive correlations suggest that certain physical measurements tend to increase together, indicating potential relationships between penguin characteristics.
Negative correlations indicate an inverse relationship between physical measurements, providing insights into the trade-offs or differences between features.
Understanding these correlations can offer insights into the physical characteristics and interdependencies among penguin species, which may be useful for further analysis or modelling.