# Executive Summary

This analysis of employee attrition has highlighted several key factors that drive turnover and provided actionable steps to help reduce it. The data shows that employee satisfaction, compensation, workload, and work-life balance are major contributors to whether employees stay or leave. Here are the main points to focus on:

1. **Satisfaction is key**: Employees with low job or environmental satisfaction are far more likely to quit. Improving job satisfaction and creating a better work environment are essential to keeping people around.
2. **Overtime leads to burnout**: Employees who regularly work overtime are much more likely to leave. Reducing overtime or offering better support for employees who work extra hours is crucial.
3. **Pay matters**: The lowest-paid employees show the highest attrition rates. Addressing pay gaps, especially for lower-income workers, can have a big impact on retention.
4. **Travel and long commutes hurt retention**: Frequent travel and long commutes make employees more likely to leave. Offering more flexibility, like remote work options, can help reduce this risk.
5. **Younger and newer employees are at risk**: Employees early in their careers or with fewer years at the company are more likely to leave, especially within the first few years. Focusing on better onboarding and clear career growth can help keep them engaged.
6. **Training is important**: Employees who don’t receive training are more likely to leave. Regular training and development programs are a great way to increase engagement and retention.
7. **Frequent job changers**: Employees who’ve worked for many companies are more likely to leave again. Giving these employees a clear path for long-term growth can help them stay longer.
8. **Stock options can help, but balance is key**: Employees without stock options are more likely to leave, but offering too many doesn’t necessarily help. Stock options should be part of a balanced retention strategy.

By focusing on these factors, companies can take meaningful steps to improve employee retention and reduce turnover.
# What's driving employee attrition and can we predict it?

In today's business world, keeping top talent is a critical challenge. Employee turnover can be costly, not just in terms of recruitment and training but also in lost productivity and team disruption. This report dives into the [IBM HR Analytics Employee Attrition & Performance dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)to explore what factors might be driving employees to leave the company.

We'll be focusing on key areas such as overtime, travel, job satisfaction, and other factors that could be contributing to employee attrition. By breaking down these factors and analyzing the attrition rates tied to each one, we aim to uncover patterns that can help us understand why people are leaving. The goal is not just to look at the data, but also to predict future attrition by developing a model that can help the company take proactive steps to retain their employees.
## Analyzing all the factors
### Personal and Education Factors
![[Personal and Education.png]]

When it comes to personal and education factors, there wasn't much difference in attrition cases between genders, so that's not a major driver here. However, the type of degree and employee has might play a role, though this could be more about the department they end up working in rather than the degree itself causing the higher attrition rates, which we will dig into later in the report. As for education levels, which are ranked from 1 to 5 (with 1 being less than a college degree and 5 being a doctorate), the attrition rates for levels 1 through 4 are similar, but those with doctorates (5) had a much lower attrition rate. It might indicate that those with doctorates are more invested with their careers, and less likely to jump ship.

Interestingly, relationship status seemed to matter, single employees and those with the lowest relationship satisfaction scores show much higher attrition rates. This can mean that personal dissatisfaction can spill into their work life. Also, maybe single employees are less tied down by obligations, making them easier to leave.
### Travel and Commutes
![[Travel.png]]

Business travel seems to play a significant role in employee attrition. Employees who don't travel have the lowest attrition rates, while those who travel occasionally ('Rarely_Travel') show a much higher attrition rate. The real standout is those who travel frequently, in which makes up almost a fourth of all employees that leave the company. It's pretty clear that frequent travel is a major factor in pushing people out the door. Even those that travel occasionally have a noticeable higher attrition, but it's the frequent travelers that are at risk. This suggests that the stress or disruption of travel, whether from work-life balance issues or just the fatigue of constant movements, plays a big role in employee attrition.

As for distance from home, the data is split into five quantiles, and there's a steady increase in employee attrition as employees live further from the workplace. Those in the bottom fifth (closest to work) are the least likely to leave, while those in the top fifth (furthest from work) have the highest attrition rates. The increase in attrition with distance from home shows that a long commute should not be underestimated, as it too can affect work life balance by acting as a time drain.
### Department and Job Roles
![[Department and Job Roles.png]]

Looking at the data by department, Research & Development (R&D) has the lowest attrition rates, while HR and Sales departments have much higher turnover. This pattern carries through to specific job roles—sales representatives stand out with an almost 40% attrition rate, making them the most likely to leave. Close behind are employees in human resources and laboratory assistants, with research scientists and sales executives rounding out the top spots for higher attrition.

Job involvement and job level also play a big part here. Employees at the lower end of both tend to leave at higher rates compared to those with higher involvement or at a more senior job level. Interestingly, despite R&D having a lower overall attrition rate as a department, lab assistants and research scientists still face higher attrition than their department's average, likely due to their lower job involvement or level compared to others in the department.
### Age and Experience
![[Age and Experience.png]]

When it comes to age, there’s a clear pattern, the younger an employee is, the more likely they are to leave. It seems like the younger workforce is more restless or looking for better opportunities. Looking at experience, the number of other companies an employee has worked for also impacts attrition. Those who’ve worked for 5-9 companies are much more likely to leave, but there’s an odd spike for employees who’ve only worked for one other company as well. Meanwhile, those with 0 or 3-4 other companies under their belt have lower attrition rates.

Total working years and years at the company tell a similar story: the less time you’ve been working (either in total or at the current company), the more likely you are to leave. Around 35% of employees who’ve only been at the company for a year or less have already left, and 23% of those who’ve been there 2-4 years followed suit. This pattern also shows up in years in the current role, shorter tenure equals higher attrition.

Even though years since the last promotion doesn’t have a huge impact, there’s a minor trend where employees who’ve been stuck in their role for too long are more likely to quit. Interestingly, years with the current manager also makes a difference, over 30% of employees who’ve been with their manager for less than a year leave, but after two years, that number drops significantly.

Lastly, training and work-life balance play roles too. Employees who received no training are more likely to leave compared to those who did, and those with poor work-life balance (rated the lowest) have an attrition rate of over 30%.
### Income
![[Income.png]]

People always look to earn the most money, and the pattern shows here with the lowest income quantile show an attrition rate of over 30%, while it drops by half in the second and continues to lower, though less dramatically as income increases.

But salary hikes seem to not be the solution, as they don't have much of an impact. There is a slight reduction in attrition when moving from the first to the second quantile and then third, but beyond that the effect is non-existent. While low pay is a big factor, it seems that salary hikes are not much of a factor, meaning job growth and satisfaction might carry more weight in the long run.

Stock option levels show that employees without any stock options are more likely to leave compared those with levels 1-3. However, stock option level 3 has a higher attrition rate than 1-2, meaning more stock options don't always guarantee retention.
### Satisfaction
![[Satisfaction.png]]
Both environmental and job satisfaction plays a role in employee attrition. Employees who report the lowest satisfaction levels are more likely to leave compared to those who are more satisfied with their job and work environment. It’s clear that dissatisfaction, either professionally or personally (relationship satisfaction), in any form, is a indicator of potential turnover.

Overtime is another major factor. Employees who are regularly working overtime are three times more likely to leave, with an attrition rate of around 30%, compared to just 10% for those who don’t work overtime. Clearly, the extra hours are taking their toll.
## Modelling the data to predict attrition.

### Dashboard Overview

We created a HR dashboard, using PowerBI to help give us an overview of the company.

![[Department Dashboard.png]]

The dashboard gives us a snapshot of the current workforce with key statistics, such as current employees, attrition rate, and the number of employees who have quit, or who are at risk. It also displays the average satisfaction levels.

![[At Risk Dashboard.png]]

The At Risk Employees section digs deeper into each individual employee data, including satisfaction, job role, income, overtime, and other relevant factors. In this example, we have an at risk employee that show low satisfaction across the board, which can signal HR to intervene try to prevent the employee from leaving.
### Model Performance and Interpretation

The model, using XGBoost, we built to predict employee attrition has an AUCPR score of 0.5, which is higher than the actual attrition rate of 16%, showing that the model performs better than random guessing. While the model is quite accurate overall, especially in predicting those who will stay (93%), it's less reliable when it comes to predicting those who will leave. Specifically, it has a precision of 0.53 and a recall of 0.51 for those employees, meaning it can catch about half of them but also flags some false positives.

However, given that this dataset is a static snapshot in time, it's useful to think those false positives, employees predicted to leave, but didn't, as being "at risk" of leaving. These employees share characteristics with those who did leave, so while they haven't exited the company yet, they might still be prone to attrition in the near future. This interpretation gives the model a more practical value, allowing it to flag employees who might need addition support or intervention to stay.

One challenge that remains is the false negatives—employees who ended up leaving but weren’t predicted by the model. Given that this is a static dataset, it’s understandable that certain subtle or evolving factors that lead to attrition weren’t fully captured. In this case, some employees may have left for reasons that weren’t as easily detectable by the data we had available.

For future research, improving the model’s ability to capture these false negatives would likely involve incorporating additional data or refining how existing data is used. For instance, adding time-based data could give a better picture of trends leading up to attrition, allowing the model to detect gradual dissatisfaction or other warning signs. Including more qualitative factors, like employee feedback or exit interview data, could also help refine predictions.

## Conclusion

In summary, there are clear patterns in what drives employee attrition, and understanding these can help companies take proactive steps to keep their talent. Employees who are dissatisfied with their job or work environment, work too much overtime, or earn lower incomes are much more likely to leave. Younger employees, those with less time at the company, and frequent travelers or long commuters are also more prone to turnover. On the flip side, providing training, fair compensation, and stock options can help improve retention.

While not every factor can be controlled, focusing on improving job satisfaction, reducing excessive overtime, and offering support to newer or lower-income employees can make a big difference. Ultimately, it’s about finding ways to keep employees engaged, satisfied, and feeling like they’re valued and have room to grow within the company.
# Methodology

The project uses [IBM HR Analytics Employee Attrition & Performance](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset) downloaded from kaggle. The dashboard, all code used to create the visualizations, and model is located at my [github](https://github.com/RHardiyanto1) to view or download. 

The data was cleaned, to make sure there were no duplicates, null values. Some columns were removed, such as 'EmployeeCount', 'Over18', 'StandardHours', as all values are the same across all employees.

In prepping the data for modelling, the non-numeric values for some columns were encoded into ordered numbers, or turned into dummy variables. We then created a correlation matrix and found multicollinearity between several features, because of this, we skipped using logistic regression and moved to use more tree-based algorithms which can handle this issue better.

Since the data is unbalanced, we tried to balance it by using oversampling and undersampling algorithms, but results showed no improvements on the model. We also used a grid search to fine the optimal tuning for our models. Since XGBoost outperformed random forest in our testing, we chose the first to act as our final model.

Since the data is static in time, with attrition known, for the purposes of the project, we ran the entire dataset into the model to 'predict' employee attrition, and labeled those false positives as 'at risk.'