Cost of Living in the USA — Data Visualization & Analysis Project
Author: Aayan Ali Peerzada
Course: Data Visualization
Tools: Python (Spyder), Pandas, NumPy, Matplotlib, Seaborn, Plotly, Scikit‑Learn

Project Overview
This project analyzes the US Family Budget Dataset, which provides cost‑of‑living estimates for 1,877 counties and metro areas across the United States. The dataset includes 31,430 observations and 15 variables, covering expenses such as housing, food, transportation, healthcare, childcare, taxes, and total family budget requirements.

The goal of this project is to perform exploratory data analysis (EDA) and create interactive and static visualizations to understand cost‑of‑living patterns across states and counties. The project also incorporates regression, outlier detection, 3D visualization, and dimensionality reduction (PCA & NMF).

 Dataset Description
The dataset contains the following variables:

state
isMetro
areaname
county
family_member_count
housing_cost
food_cost
transportation_cost
healthcare_cost
other_necessities_cost
childcare_cost
taxes
total_cost
median_family_income
The variable case_id was removed as instructed.

1. Data Cleaning
Removed missing values using dropna()
Verified data types and ensured categorical vs quantitative variables were correctly identified
Dropped the case_id column

2. Interactive Summary Table
An interactive summary table was created using Plotly to display mean values of quantitative variables grouped by state.

3. State‑Level Analysis
For each state, visualizations were created for:

Transportation Cost
Healthcare Cost
Childcare Cost
Taxes
Median Family Income
Family Member Count
Boxplots were used to compare distributions across states and identify high‑cost regions.

4. Grouped State Table with Color Formatting
A color‑graded table (using Pandas styling) highlights state‑level averages for key cost variables.

5. Choropleth Map
A US choropleth map visualizes average transportation cost by state.
This map is compared with earlier boxplots to confirm consistency in high‑cost regions.

6. Cost Relationship Plots (Colored by State)
Scatterplots were created for:

Total Cost vs Transportation Cost
Childcare Cost vs Taxes
Median Family Income vs Taxes
Housing Cost vs Taxes
These visualizations reveal trends, correlations, and state‑specific clusters.

7. Top 12 Most Expensive Counties (Childcare)
A ranked bar chart highlights the 12 counties with the highest childcare costs.

8. Top 12 Highest‑Tax Counties
A similar bar chart identifies the counties with the highest tax burdens.

9. Correlation Matrix
A heatmap of all quantitative variables shows:
Strong positive correlations between total cost and major expense categories
Relationships between income, taxes, and cost of living

10. Regression: Total Cost vs Taxes
A simple linear regression model was fitted:
Regression line plotted
Slope and intercept reported
Interpretation included in the report

11. Outlier Detection for Food Cost (by State)
State‑level boxplots were used to identify unusually high or low food costs.

12–13. Bubble Plots
Two bubble plots were created:

Food Cost vs Taxes
Bubble size: Childcare Cost

Color: Metro vs Non‑Metro

Housing Cost vs Taxes
Bubble size: Transportation Cost

Color: State

These reveal multi‑dimensional relationships between cost drivers.

14–15. 3D Visualizations
Two 3D scatterplots were created using Plotly:

Transportation vs Healthcare vs Childcare Cost

Childcare Cost vs Taxes vs Median Family Income (colored by state)

These help visualize multi‑variable interactions.

16. PCA (3 Components)
Standardized quantitative variables

Extracted 3 principal components

Visualized in 3D

Reported explained variance ratios

17. NMF (3 Components)
Applied Non‑Negative Matrix Factorization

Interpreted component loadings

Visualized counties in NMF‑space

 Conclusion / Reflection
The analysis reveals clear geographic patterns in cost of living across the United States. States with large metropolitan areas tend to have higher housing, childcare, and transportation costs. Taxes and total cost of living show a moderately strong relationship, while PCA and NMF highlight underlying cost structures that differ across regions. These insights can help policymakers, families, and researchers better understand economic pressures across U.S. counties.
