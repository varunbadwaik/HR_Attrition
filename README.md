# HR_Attrition

HR Attrition Project
Introduction:- This report provides insights into HR attrition, highlighting the number of employees who have left the company and identifying specific patterns and groups where attrition is more prominent. It aims to uncover the key reasons behind employee turnover and dissatisfaction through detailed data analysis. The tasks completed in this project include data cleaning and preprocessing, descriptive analysis of employee attributes, visualization of employee distribution across various roles and departments, correlation analysis to identify key influencing factors, and in-depth attrition analysis. Based on these findings, actionable recommendations are provided to help HR teams enhance employee satisfaction, engagement, and retention strategies.

Data Overview:-
1.	Dataset Size & Structure: The dataset includes 1,470 employee records with 35 columns, covering a wide range of employee information.
2.	Attrition Indicator: The Attrition column shows whether an employee has left the company (Yes or No), which is crucial for analyzing turnover patterns.
3.	Clean Data: There are no missing values, so the dataset is ready for direct analysis without additional preprocessing.
4.	Column Variety: The dataset contains a mix of categorical (e.g., Department, JobRole, Gender) and numerical columns (e.g., Age, MonthlyIncome, TotalWorkingYears), providing a comprehensive view of employee profiles.

Data Preparation:-
1.	Library Import: Essential Python libraries such as Pandas, NumPy, Matplotlib, and Seaborn were imported to handle data manipulation, numerical operations, and visualization.
2.	Data Loading: The HR dataset was loaded using pandas.read_csv(), which allowed easy access to the CSV file and enabled further analysis within a Jupyter Notebook environment.
3.	Data Type Inspection: To understand the structure of each column, the .dtypes function was used, helping identify which columns are categorical and which are numerical.
4.	Missing Value Check: The .isnull().sum() function was applied to detect any missing values across the dataset. The output showed that there were no missing values, confirming the dataset is clean and ready for analysis.

Exploratory Data Analysis (EDA):-
In the initial phase of EDA, we examined the data types of each column using .dtypes to distinguish between numerical and categorical features. We then checked for missing values using .isnull().sum() and found none. Additionally, we explored the unique values in each categorical column and used .value_counts() to understand the distribution of key features like Attrition, Department, and JobRole, which helped identify patterns and prepare for deeper analysis.

Data Visualization:-
1.	Histogram for Satisfaction Levels
A histogram was created using Seaborn to display the distribution of employee satisfaction levels. This helped identify how many employees reported low, medium, or high satisfaction, and revealed any skewness in overall satisfaction trends.
2.	Heatmap for Correlation Analysis
A correlation heatmap was generated to visualize relationships between numerical variables such as SatisfactionLevel, MonthlyIncome, YearsAtCompany, and PerformanceRating. This made it easy to identify strong positive or negative correlations that influence attrition and performance.
3.	Bar Chart for Department-wise Attrition Rates
A bar chart was plotted to compare attrition rates across different departments. This helped highlight which departments were most affected by employee turnover, aiding in targeted retention strategies.
4.	Box Plot for Salary Variations by Job Role
A box plot was used to analyze the distribution of salaries across different job roles. It showed salary medians, ranges, and outliers, making it easier to spot inequality or potential dissatisfaction among roles.
5.	Line Plot for Performance Ratings Over Time
A line plot was created to display trends in performance ratings over time or years at the company. This helped in understanding whether employee performance improves with tenure or drops off, and if any cyclical patterns exist.

Key Findings from EDA and Visualizations
•	Departmental Distribution: Most employees belong to the Research and Development department, while the Human Resources department has the least.
•	Age Distribution: Majority of employees are in their 30s. There is a noticeable decline in employees above 50, suggesting retirement or attrition.
•	Monthly Income: Most employees earn below 7500, showing a skew towards lower-income jobs, which may impact satisfaction.
•	Correlation Insights:
o	Job Level and Monthly Income show a strong positive correlation.
o	Total Working Years is positively correlated with Job Level, indicating experience is valued.
o	Weak correlation between satisfaction level and performance rating, suggesting other factors might influence satisfaction.

Factors Strongly Correlated with Satisfaction and Performance
•	Job Level and Monthly Income influence satisfaction indirectly, as low salary can cause dissatisfaction.
•	Work-life balance and Job Involvement may not be strongly correlated numerically but have visual patterns showing their influence.
•	Performance Ratings show variation across departments, possibly impacted by workload and training.

Recommendations for HR Strategies
•	Increase Compensation Transparency and Growth: Address dissatisfaction among lower-income employees by providing clear career progression and salary increment plans.
•	Retain Mid-Career Professionals: Since most employees are in their 30s, focusing on retention strategies like better work-life balance and recognition will help.
•	Department-Specific Engagement: Provide additional support to departments with higher attrition (like Human Resources or Sales).
•	Tailored Training Programs: Design training modules based on employee performance trends to uplift low performers and retain high performers.
Conclusion:-This HR Attrition project provided a comprehensive analysis of employee turnover using statistical exploration and data visualization. By identifying key factors like department, income, job level, and satisfaction levels, we uncovered patterns contributing to attrition. The insights derived offer valuable direction for HR teams to implement data-driven strategies aimed at improving retention, boosting employee engagement, and fostering a healthier workplace culture.

