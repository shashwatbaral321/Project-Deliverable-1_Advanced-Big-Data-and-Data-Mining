# Project Deliverable 1: Data Collection, Cleaning, and Exploration

## Dataset Description
The dataset is "Mobile Phone Usage Statistics," containing 6 attributes such as country name, mobile usage values, region, and ranking for over 200 countries. It is appropriate due to its size and real-world relevance for analyzing mobile adoption trends.

## Data Cleaning Steps
- Fixed encoding issues using utf-8-sig.
- Converted 'value' column from string with commas to numeric.
- Filled missing values in 'value' with median to avoid bias.
- Dropped rows missing 'region' since regional data is important for analysis.
- Removed duplicates to ensure data quality.
- Identified and removed outliers using the IQR method.

## Exploratory Data Analysis (EDA)
- Distribution of mobile usage is right-skewed.
- China and India lead usage by a large margin.
- Usage varies significantly across regions.
- Correlation matrix shows moderate correlation between ranking and usage.
- Outliers mainly in countries with extremely high or low usage.

## Insights and Future Work
- Regional differences suggest models must incorporate region-based features.
- Outlier removal will help build more stable predictive models.
- Scaling and discretization planned for next phases.

## Challenges
- BOM encoding issue required adjusting file reading.
- Numeric data cleaning was needed to convert strings with commas.
- Deciding when to fill vs drop missing data required careful judgment.

