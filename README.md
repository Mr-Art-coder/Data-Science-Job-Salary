# INTRODUCTION
Data-related jobs have been a crucial part of the labor market. This research focuses on identifying the wage range within each of the positions in data science, the highest paid role, and the salary trend over time. These roles include data scientists, data analysts, data engineers, and others.

----

# DATA SOURCE
The Pomerol website provided the dataset, which is the entry for the September data challenge. To get the dataset, click [here](https://pomerolpartners.com/dataset_challenge/september-2022/).

----

# DATA WRANGLING
## COLUMN REMOVAL
Using the power query in Power BI, this dataset was transformed. The dataset was retrieved as a CSV file with 11 columns, including the following: work year, level of experience, employment type, job title, salary, salary currency, salary in USD, remote ratio, firm size, location, and employee residence.
First, the salary and salary currency columns were eliminated since they were unnecessary. The salary may be expressed in USD because it is the most widely used currency, and the currency can be readily established by the country of work.

----

## ABBREVIATION
The columns were renamed for visibility and easy comprehension. Company location and employee residence fields were abbreviated using country code, i.e., NG stands for Nigeria, but not everybody can understand this scenario, so the fields were changed to the full country using the “Replace” method.

The fields in company size were also abbreviated, L, S, and M, and the fields were replaced with the full meaning where L stands for Large, S for Small, and M for medium.

The fields in Experience level were also abbreviated, MI, SE, EN, and EX. These four abbreviations were changed to full for easy understanding, MI changed to Mid-level, SE to Senior Level, EN to Entry Level, and EX changed to Expert.

Employment type column was not excluded, it also contained abbreviation, CT, FL, FT, and PT. these abbreviations were changed so that CT changed to Contract, FL to Freelance, FT to Full time while PT change to Part time.

Lastly, remote ratio column came in numbers, 0,50 and 100. After reading the description of the dataset on the source site, 0 was changed to “Not Remote”, 50 was changed to “Partial Remote” while 100 was changed to “Fully Remote”.

----

## ADDED COLUMN
As stated earlier, the dataset contained 11 columns, 2 were removed which reduced the columns to 10. To determine if employee secure work in his/her residence or outside his/her residence, new column was added. This column was added using “Conditional Statement (if, then, else), if the employee works in his/her place of residence, the column should return “TRUE” else it should return “FALSE”. This was written using employee residence and company location columns. (if [Employee Residence] = [Company location] then “TRUE” else “FALSE”).

----
# VISUALIZATION

7 charts were used to visualize the analysis, card, line chart, slicers, donut chart, stacked column chart, stacked bar chart, and table.

## Cards
![Cards](https://github.com/Mr-Art-coder/Data-Science-Job-Salary/blob/main/Charts/Cards.JPG)

Four cards were used to visualize the total salary in USSD, total company locations, number of people employed, and total number of job title/ roles.

## Line
![Line](https://github.com/Mr-Art-coder/Data-Science-Job-Salary/blob/main/Charts/line.JPG)

This chart was used to visualize the salary scale per year

## Slicers
![Slicer](https://github.com/Mr-Art-coder/Data-Science-Job-Salary/blob/main/Charts/slicer.JPG)

6 slicers were used to filter by company size, job type, job title, company location, experience level, and year.

## Donut Chart
![Donut](https://github.com/Mr-Art-coder/Data-Science-Job-Salary/blob/main/Charts/Donut%20Chart.JPG)

This chart was used to visualize the percentage of employees who work in their residence and those who work outside their residence

## Stacked Column Chart
![Column](https://github.com/Mr-Art-coder/Data-Science-Job-Salary/blob/main/Charts/Stacked%20Column.JPG)
![Columnline](https://github.com/Mr-Art-coder/Data-Science-Job-Salary/blob/main/Charts/line%20and%20stacked%20column.JPG)

2 Stacked column chart was used to visualize the remote ratio scale by employment and the number of employments and salary by company size.

## Stacked Bar Chart
![Bar](https://github.com/Mr-Art-coder/Data-Science-Job-Salary/blob/main/Charts/Stacked%20bar%20chart.JPG)

This chart was used to visualize the number of employments by experience level, to determine the changes.

## Table
![Table](https://github.com/Mr-Art-coder/Data-Science-Job-Salary/blob/main/Charts/Table.JPG)
This was used to determine the salary scale by job title.

----

# INSIGHT

•	Salary scale trends upward by year
•	Data scientists earn more in 2020 and 2021 than other data-related job titles.
•	Data Engineer is earning more in 2022
•	Fully remote ratio trends upward by year
•	92% of employee work in their residence
•	Medium size companies hire and pay more.

----

# DASHBOARD
![DASHBOARD](https://github.com/Mr-Art-coder/Data-Science-Job-Salary/blob/main/Charts/Dashboard.png)

----
# ACCOUNT

Follow on [Twitter](https://twitter.com/AdegunleRT
Let us connect on [LinkedIn](https://www.linkedin.com/in/adegunleraphael
