# HR Employee Attrition Analysis

## Project Overview
This Project provides insights into employee attrition trends, key influencing factors, and potential strategies for retention. The analysis focuses on various employee attributes such as age, department, job role, years at the company, and more.

## Problem Statement
Employee attrition poses significant challenges to organizational productivity and financial stability. To develop effective retention strategies, it's crucial to understand the underlying factors contributing to employee turnover. 

**This analysis seeks to address the following critical questions**:

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
The dataset used in this project mirrors real-world HR records, collected from various organizational sources. It includes employee demographics, job roles, tenure, performance metrics, and exit interview details.
To ensure data privacy, personally identifiable information (PII) was removed or anonymized. AI-based techniques were applied to regenerate realistic values for removed data points, maintaining authentic attrition patterns for meaningful analysis.

## Data Structure  
The data contains the following columns: EmployeeNumber, Attrition, Age, Gender, Department, JobRole, JobLevel, MonthlyIncome, YearsAtCompany, YearsInCurrentRole, JobSatisfaction, WorkLifeBalance, OverTime, BusinessTravel, DistanceFromHome, EnvironmentSatisfaction, PerformanceRating, PercentSalaryHike, TrainingTimesLastYear, Education, EducationField, MaritalStatus.

## Data Analysis Process

**Data Cleaning & Transformation**
Conducted using Power Query, the process involved: formatting fields (e.g., income ranges), handling missing values, grouping job levels, standardizing ratings (e.g., environment satisfaction, job level), and applying binning and segmentation for clearer analysis.

**Exploratory Data Analysis (EDA)**

Explored attrition trends in relation to key variables: job role, monthly income, department, job level, environment satisfaction, and marital status.
Tool Used: Power BI

 **DAX Calculations** 
 
Data Analysis Expressions (DAX) was used to create custom measures and KPIs, including:
- Attrition rate calculations
- Segmentation by job level and income bracket

**Attrition Rate%** = 
  DIVIDE(
      CALCULATE(
          COUNT('WA_Fn-UseC_-HR-Employee-Attrition'[EmployeeNumber]),
          'WA_Fn-UseC_-HR-Employee-Attrition'[Attrition] = "Yes"
      ),
      COUNT('WA_Fn-UseC_-HR-Employee-Attrition'[EmployeeNumber])
  )
  
**Data Visualization**

Utilized Power BI to create compelling visuals and interactive reports to effectively communicate key insights. The visualizations included bar charts, column charts, matrix tables, donut charts, and funnel charts. Tenure-based trends and filters allowed for deeper insights into various performance metrics.

**HR Employee Attrition Analysis Dashboards Showing Insights**

![image](https://github.com/user-attachments/assets/71c3c752-332f-45b1-a033-8985aa3bde9e)
![image](https://github.com/user-attachments/assets/1b7b4246-3006-4074-9af3-3e0988996a6f)
![image](https://github.com/user-attachments/assets/7941dafb-8302-45c0-a556-5cb2045b11e5)

 ## Executive Summary
Findings suggest that attrition rates are higher among employees with lower salaries, entry-level positions, and those in sales and HR roles. Employees experiencing long commutes, frequent business travel, poor work-life balance, and limited training opportunities are more likely to leave. Additionally, high attrition is linked to low job satisfaction, inadequate recognition, and insufficient career growth opportunities. Employees with higher education and job satisfaction tend to stay longer, while those with poor work environments or lacking career advancement are more likely to exit.

## **Insights Deep Dive**

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

1. **Increase Salaries for Mid-Level Employees**: Consider offering competitive salaries for employees earning between $1k - $5k, as they have the highest attrition rate. A salary increase for this group, especially in mid-level roles, could reduce turnover.

2. **Enhance Career Growth Opportunities**: Focus on providing more development and career advancement opportunities for entry-level and mid-level employees to improve retention. Clear career paths can motivate employees to stay long-term.

3. **Provide Incentives for Sales Roles**: Since sales roles have the highest attrition, consider introducing better incentives, support, and manageable performance targets to reduce job pressure and retain top talent.

4. **Improve Work Culture and Incentives in High-Turnover Departments**: Departments like Sales and HR experience high turnover. Implement initiatives such as team-building activities, better incentives, and employee engagement programs to create a more positive and supportive work environment.

5. **Improve Job Satisfaction**: Address factors contributing to low job satisfaction, such as workload, management support, and work-life balance. Conduct regular satisfaction surveys to identify areas for improvement.

6. **Support Single Employees**: As single employees have the highest attrition rate, consider offering additional support like career counseling, networking opportunities, and more flexible work arrangements to cater to their needs.

7. **Address Burnout and Retirement Concerns for Senior Employees**: For employees with 10-20 years of experience, consider offering retirement planning programs, career coaching, or roles with less pressure to retain them longer.

8. **Enhance Recognition and Reward Programs**: High-performing employees are leaving at the same rate as others. Strengthen employee recognition programs, introduce regular feedback loops, and provide clear pathways for promotions and rewards to ensure their efforts are appreciated.

9. **Offer Flexible Work Options**: For employees living 21-30 miles away or those experiencing long commutes, consider providing remote work options or flexible hours to improve retention.

10. **Implement Work-Life Balance Initiatives**: Employees with poor work-life balance experience high attrition. Introduce flexible hours, wellness programs, and other initiatives that promote a healthier work-life balance.

11. **Limit Overtime and Ensure Workload Management**: Since employees working overtime are more likely to leave, reduce excessive work hours and ensure a balanced workload to prevent burnout and improve job satisfaction.

12. **Reduce Frequent Business Travel**: Frequent business travel is associated with high attrition. Explore options to reduce travel frequency or provide greater support for employees who travel regularly to mitigate burnout.

13. **Increase Training and Development Opportunities**: Employees with low training levels are more likely to leave. Invest in training and upskilling programs to equip employees with the tools and knowledge they need to advance in their careers.

14. **Encourage Higher Education and Professional Development**: Employees with higher education tend to stay longer. Support educational development programs and provide incentives for employees to pursue higher qualifications or certifications.

15. **Consider Gender-Specific Needs in Retention Strategies**: Since male employees have a slightly higher attrition rate, consider tailoring retention strategies to address gender-specific challenges or preferences in job roles and career growth.

16. **Timing of Salary Hikes**: Ensure salary hikes are provided in a timely manner and are competitive with industry standards. Delayed salary increases may not significantly improve retention if granted too late.

17. **Address High Attrition in HR and Technical Roles**: HR professionals and those in technical fields, such as engineering or IT, experience higher attrition. Investigate stress levels, job market demand, and external opportunities in these roles to create better retention strategies.

18. **Improve Job Satisfaction to Lower Attrition**: Address the factors contributing to poor job satisfaction, especially for those with low satisfaction, to reduce attrition. Offering growth opportunities, better communication, and a supportive work environment could be key to improving retention.

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



