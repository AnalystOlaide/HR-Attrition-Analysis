# HR Attrition Analysis

## Project Overview
This Power BI dashboard provides insights into employee attrition trends, key influencing factors, and potential strategies for retention. The analysis focuses on various employee attributes such as age, department, job role, years at the company, and more.

## Problem Statement
Employee attrition can significantly impact an organization’s productivity and costs. Understanding the key factors driving employee turnover is essential for improving retention strategies and workforce stability.
🧩 Problem Statement
Employee attrition poses significant challenges to organizational productivity and financial stability. To develop effective retention strategies, it's crucial to understand the underlying factors contributing to employee turnover. This analysis seeks to address the following critical questions:

Which job roles and departments exhibit the highest attrition rates?

How does compensation influence employee attrition?

What is the relationship between job level and attrition?

How do work-life balance and overtime impact attrition?

What role does job satisfaction play in employee turnover?

Are certain demographic groups more prone to attrition?

Does the distance from the workplace affect attrition rates?

How does the frequency of business travel relate to attrition?

What is the impact of training and development opportunities on attrition?

How does performance recognition influence employee retention?

## Data Source
The data used in this project comes from ChatGPT.

## Methodology
- **Tool Used**: Power BI
- **Data Preparation**: Cleaning and transforming raw HR data using Power Query
- **Analysis Techniques**: Data visualization, trend analysis, segmentation, and DAX calculations
- **Key Metrics**: Attrition rate, department-wise turnover, job role analysis, tenure-based trends

## Power BI Skills Applied
- **Power Query**: Used for data cleaning and transformation.
- **DAX Formula for Attrition Rate%**:
  ```DAX
  Attrition Rate% = 
  DIVIDE(
      CALCULATE(
          COUNT('WA_Fn-UseC_-HR-Employee-Attrition'[EmployeeNumber]),
          'WA_Fn-UseC_-HR-Employee-Attrition'[Attrition] = "Yes"
      ),
      COUNT('WA_Fn-UseC_-HR-Employee-Attrition'[EmployeeNumber])
  )
  ```
- **Data Visualization**: Created interactive reports to display insights effectively.

## Key Insights
![image](https://github.com/user-attachments/assets/e3ba721f-0c08-4457-aeee-b8c80e4543bb)
![image](https://github.com/user-attachments/assets/c9edfc24-35c7-44d9-8a52-c54522677f0b)
![image](https://github.com/user-attachments/assets/845d0d49-76b0-48e2-9f04-ec232e96eddc)

### 1. Monthly Income vs. Attrition
- Employees earning $1k - $5k have the highest attrition rate (21.76%).
- Attrition decreases as salary increases, with employees earning $15k - $20k having the lowest attrition rate (3.76%).
**Key Insight**: Higher salaries may help reduce employee turnover.

### 2. Attrition Rate by Job Level
- Entry-level employees have the highest attrition rate (49.24%).
- Mid-level employees have an attrition rate of 31.06%.
- Senior-level employees experience attrition (19.71%).
**Key Insight**: More career growth opportunities for entry and mid-level employees could help improve retention.

### 3. Job Roles with the Highest Attrition
- Sales Representatives have the highest attrition (39.76%).
- Laboratory Technicians (23.94%) and Human Resources (23.08%) follow.
- Research Directors and Manufacturing Directors have much lower attrition.
**Key Insight**: Sales roles experience the highest turnover, possibly due to job pressure or lack of incentives.

### 4. Attrition by Department
- Sales department has the highest attrition (20.63%).
- Human Resources follows at 19.05%.
- Research & Development has lower attrition (13.84%).
**Key Insight**: Departments with high attrition may require improved work culture or better incentives.

### 5. Work Environment Satisfaction vs. Attrition
- Employees with poor satisfaction account for 38% of attrition.
- Employees with excellent satisfaction account for only 20%.
**Key Insight**: Improving workplace satisfaction can help retain employees.

### 6. Marital Status and Attrition
- Single employees have the highest attrition rate (25.53%).
- Married employees (12.48%) and divorced employees (10.09%) follow.
**Key Insight**: Single employees may be more likely to switch jobs for better opportunities.

### 7. Attrition Rate by Years at Company
- Employees with 31-40 years have the highest attrition rate (50.7%).
- Employees with 10-20 years have an attrition rate of 33.08%.
**Key Insight**: Senior employees may leave due to retirement, burnout, or lack of progression.

### 8. Attrition Rate by Performance Rating
- High-performing employees are leaving at nearly the same rate as others.
**Key Insight**: Recognition and rewards need improvement.

### 9. Attrition Rate by Distance from Workplace
- Employees living 21-30 miles away have the highest attrition rate (22.06%).
**Key Insight**: Remote work options could help improve retention.

### 10. Attrition Rate by Work-Life Balance
- Employees with poor work-life balance have the highest attrition (31.25%).
**Key Insight**: Flexible work arrangements can improve retention.

### 11. Attrition Rate by Overtime
- Employees who work overtime have a 30.53% attrition rate.
**Key Insight**: Reducing excessive work hours can improve retention.

### 12. Attrition by Business Travel
- Employees who travel frequently have the highest attrition rate (52.04%).
**Key Insight**: Frequent business travel may lead to burnout.

### 13. Attrition by Training Level
- Employees with low training levels have the highest attrition rate (38.47%).
**Key Insight**: Lack of training leads to high turnover; upskilling is crucial.

### 14. Attrition by Education Level
- Employees with a high school diploma have the highest attrition (18.24%).
**Key Insight**: Higher education may correlate with job stability.

### 15. Attrition by Gender
- Males (17.01%) have a slightly higher attrition rate than females (14.80%).
**Key Insight**: Industry trends and job roles may influence gender-based attrition.

### 16. Attrition by Salary Hike Percentage
- Employees receiving a 21-25% salary hike have the highest attrition (17.54%).
**Key Insight**: Salary hikes may not always improve retention if granted too late.

### 17. Attrition by Education Field
- Human Resources has the highest attrition rate (25.93%), followed by Technical Degrees (24.24%) and Marketing (22.01%).
- Medical (13.58%) and Other fields (13.41%) have the lowest attrition rates.
**Key Insight**: HR professionals and those with technical backgrounds are leaving at higher rates, possibly due to stress, job market demand, or better external opportunities.

### 18. Attrition Rate by Job Satisfaction
- Employees with poor job satisfaction have the highest attrition rate (22.84%).
- Employees with fair (16.43%) and good (16.52%) satisfaction have similar attrition rates.
- Employees with excellent satisfaction have the lowest attrition rate (11.33%).
**Key Insight**: Job satisfaction significantly impacts employee retention. Companies should focus on improving work culture, career development, and employee engagement.

## Recommendations
1. **Offer competitive salaries** to reduce attrition among lower-income employees.
2. **Enhance career growth opportunities** for entry and mid-level employees.
3. **Improve job satisfaction** by fostering a supportive work culture and clear career progression.
4. **Implement flexible work policies** such as remote work options.
5. **Reduce excessive overtime** and provide fair compensation.
6. **Improve training programs** to enhance employee engagement and skill development.
7. **Limit frequent business travel** to prevent burnout.
8. **Recognize and reward high performers** to ensure retention of top talent.
9. **Offer better incentives** for high-attrition job roles like Sales and HR.

## Conclusion
Employee attrition is influenced by multiple factors, including salary, job satisfaction, work-life balance, career growth, and work conditions. This Power BI analysis has identified key drivers of attrition and provided data-driven recommendations. Implementing these strategies will help organizations build a more stable and satisfied workforce.



## How to Use This Project
1. **Download the Power BI file** from this repository.
2. **Load the dataset** (or use the provided sample data).
3. **Explore the interactive dashboard** to gain insights into employee attrition.
4. **Modify the visuals** as needed to tailor insights for your organization.

## Technologies Used
- **Power BI** (Data visualization and dashboard creation)
- **Power Query** (Data cleaning and transformation)
- **DAX** (Data analysis and calculations)

## Author
[Yusuf Olaide] - Data Analyst

## License
This project is open-source and free to use 

