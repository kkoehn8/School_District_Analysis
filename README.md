# School_District_Analysis

## Project Overview
We were tasked with cleaning and analysing student and school data. The data was for 15 High Schools and included student names, grades, math and reading scores and schools types, size and budget. The first step in the project was to clean any the data provided, mainly removing prefixes and suffixes that high school students should not have then running some summary statistics. After completing the initial analysis we were told that there may have been some academic dishonesty among the ninth graders at Thomas. The second part of the project was to rerun the summary statistics after removing students were who suspected of academic dishonesty.


## Data and Software
The analysis was conducted using the following files:
 - students_complete.csv
 - schools_complete.csv
 - PyCitySchools_Chalenge_starter_code,ipnub

The software used was:
 - Python 3.7.6
 - JupyterLab 3.3.2
 
## Results
The original analysis was conducted using all students in all grades, however for the new analysis the math and reading scores for the ninth grade students at Thomas High School were replaced with NaN (not a number) and the analysis was completed again.

How is the district summary affected?
The analysis at the district level showed little change, however the following changes were noted:
 - Percent Passing Math: 75% (original), 74.8% (new)
 - Percent Passing Reading: 86% (original), 85.7% (new)
 - Percent Overall Passing: 65% (original), 64.9% (new)

The school summary showed a dramatic difference for Thomas High School after the scores from the ninth graders were removed. The image below is from the original analysis

![orig_school_summary](https://github.com/kkoehn8/School_District_Analysis/blob/main/Images/orig_SchoolSummary.PNG)

The image below is from the new analysis. 
![new_school_summary](https://github.com/kkoehn8/School_District_Analysis/blob/main/Images/new_SchoolSummary.PNG)

As seen above there's a dramatic different in Percent Passing Math, Percent Passing Reading and Overall Passing Percent once the ninth grade students scores were removed.

This results in Thomas High School jumping from a 65% Overall Passing to a 90% Overall Passing and moving it from one of the lower performing schools to one of the higher performing schools in comparison to the other schools in our analysis.

After replacing the ninth grade scores we can see the following:

 - The output for our scores by grade now show the ninth grade at Thomas is classified as nan (not a number).  
![orig_math](https://github.com/kkoehn8/School_District_Analysis/blob/main/Images/Orig_MathByGrade.PNG)
![new_math](https://github.com/kkoehn8/School_District_Analysis/blob/main/Images/New_MathByGrade.PNG)

 - We see the exact same thing when we look at the reading scores 

 - We don't see a difference in the scores by school spending as can be seen below
 
![orig_score_spending](https://github.com/kkoehn8/School_District_Analysis/blob/main/Images/Orig_ScoreBySpending.PNG)
![new_score_spending](https://github.com/kkoehn8/School_District_Analysis/blob/main/Images/New_ScoreBySpending.PNG)
 
 - We don't see a difference in the scores by school size after removing the ninth graders from Thomas High School

 - We don't see a difference in the scores by school type
 
## Results
After removing the the ninth grade students from Thomas High School we can notice a difference when reviewing the school level analysis however that difference it less noticeable at the district level. 

The math, reading and overall passing percentage for Thomas High School increases dramatically when compared to other schools and results in Thomas High School becomming a top performing school. At the district level, the changes in the Math, reading and overall passing percentages have a minimal effect on the overall summary but there are slight changes. However, when reviewing other analysis at the District level there appears to be no change. There could be two reasons for this, first the rounding of the data, if we were to show the data to two decimal places we may notice a difference at the District level. The second consideration is that while we notice a difference at the school level once the data is aggregated to the District level the removal from the analysis of the Thomas High School ninth graders is not an important a factor due to the number of students. 










