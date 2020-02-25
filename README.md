# analysis-of-baltimore-city-government-salary

An analysis of Baltimore City employee salary data, specifically the police department 

This analysis used data from the [Open Baltimore](https://data.baltimorecity.gov/City-Government/Baltimore-City-Employee-Salaries-FY2018/biyh-j8tc)

The two questions that this analysis looked at were:
1. What is the impact of job tenure on gross salary for the police department?
2. What is the impact of job tenure and gross salary on the amount of overtime pay in the police department? 

## Analysis Steps for Question 1: 
1. The data was filtered to include only people who have job titles with the word 'Police' 
2. The date of hire data was changed to the accepted Excel date format
3. The tenure for each employee was then calculated and graphed against that employee's gross salary 
4. The equation for the linear regression was then displayed on the graph.

![alt text](https://github.com/yangnoah/analysis-of-baltimore-city-government-salary/blob/master/Graph.JPG)

This analysis shows that there is a linear relationship between how long a person is employed by the police department and what their gross salary is. The R-squared value is 0.39 which means the data is a good fit. The longer one is employed by the police department, the more money they make. This makes sense because annual raises accumulate over time and increase one's salary. For someone with prvious policing experience who is seeking employment in the police department, it would make sense for them to use the linear regression model to esimate how much salary they should ask for. 

## Analysis Steps for Question 2:
1. Data was copied over from Question 1
2. Overtime pay was calculated by subtracting the annual salary from the gross pay 
3. ToolPak was then used with overtime pay on the y-axis and the gross salary and the job tenure on the x-axis 

The regressions statistics show an R squared value of 84% which means 84% of the variations in overtime pay can be explained by job tenure and the gross salary of a position. The two coefficients are:

Job Tenure: -2.67
Gross Annual Pay: 0.81

The -2.67 coefficient for job tenure suggests that the longer one is employed with the police department, the amount of overtime they are paid is lower. This is likely due to overtime being paid more to hourly workers than higher level managers who are likely paid a fixed amount. 

The 0.81 coefficient for gross annual pay suggests that the more one is paid, the amount of overtime they are paid is higher. This is because those who have a high annual pay also have a high hourly pay rate. So for the same amount of overtime hours they will have a higher amount of overtime pay. 

The city should use this model to aid in budgeting for overtime for the police department. Every year, this model can be used at the start of the year to determine approximately how much overtime the department will pay depending on the tenure and gross pay of the current staff. 





