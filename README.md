Exploring Socioeconomic Disparities in Chicago Using SQL & Data Visualization
In this project, I worked with a real-world socioeconomic dataset from the City of Chicago Data Portal, storing it in a database, querying it with SQL, and visualizing key insights using Python’s Seaborn and Matplotlib libraries.
The dataset covers 78 Chicago community areas (2008–2012) and contains six socioeconomic indicators of public health significance, along with a Hardship Index — a score from 1 to 100, where higher numbers represent greater socioeconomic hardship.
________________________________________
Dataset Variables
•	Community Area Name & Number – unique identifiers for each region
•	Percent of Housing Crowded – % of occupied units with more than one person per room
•	Percent Households Below Poverty – % of households living below the federal poverty line
•	Percent Aged 16+ Unemployed – % of persons over 16 without jobs
•	Percent Without High School Diploma (25+) – % without a high school education
•	Percent Aged Under 18 or Over 64 – % of dependents in the community
•	Per Capita Income – estimated total income divided by population
•	Hardship Index – composite score derived from the six indicators above
________________________________________
Key Insights from SQL Analysis
Using SQL queries, I discovered:
•	38 communities have a Hardship Index greater than 50.
•	Riverdale has the highest hardship score at 98.
•	Communities like Lake View, Lincoln Park, Near North Side, and Loop enjoy per capita incomes above $60,000, indicating stronger economic conditions.
________________________________________
Relationship Between Income & Hardship
A Seaborn Jointplot (scatterplot + histograms) revealed a strong, negative correlation between per capita income and the Hardship Index:
•	Low-income areas ($10K–$20K) often face hardship scores above 80, reflecting severe economic difficulty.
•	Middle-income areas ($30K–$40K) see a steep decline in hardship, suggesting improved living conditions.
•	High-income areas (above $50K) approach hardship scores near zero, indicating minimal economic strain.
Statistical analysis confirmed this: r = -0.849, p < 0.001. This is a very strong, statistically significant negative correlation, meaning higher income is strongly associated with reduced hardship.
________________________________________
Tools & Technologies Used
•	Python (Pandas, Seaborn, Matplotlib) – for data analysis and visualization
•	SQL – for database queries and insight extraction
•	SQLite – for structured data storage and retrieval
•	Jupyter Notebook – for interactive analysis and presentation
________________________________________
Conclusion
Economic well-being in Chicago’s communities is closely tied to income levels. Higher per capita income is strongly linked to reduced socioeconomic hardship, making it a critical factor in public policy and community development strategies.
