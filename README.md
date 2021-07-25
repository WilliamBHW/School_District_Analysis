# School_District_Analysis
## Overview
This project is aimed to display the following metrecies:
- Top 5 and bottom 5 performing schools, based on the overall passing rate
- The average math score received by students in each grade level at each school
- The average reading score received by students in each grade level at each school
- School performance based on the budget per student
- School performance based on the school size
- School performance based on the type of school

## Background
> The school board has notified Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked you to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once you’ve replaced the math and reading scores, Maria would like you to repeat the school district analysis that you did in this module and write up a report to describe how these changes affected the overall analysis.

## Results
The school summary is affected, setting Thomas High School (THS) grades for 9th grade students are set to NaN will affect the columns math, reading, and overall passing percentages in the future summarzation.
<br>
![image of change](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/9th_grade_NaN.png)
<br>

The district summary is affected in columns math, reading, and overall in the percentage pasing. (The change is small considering its population, one school's change will affect the whole in decimals)
<br>
###### Before
![](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/District_Summary(Before).png)
<br>
###### After
![](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/District_Summary(After).png)
<br>

Thomas High Schools performance is significantly dropped in overall passing rate in both reading and math, which will allow other high schools percentage replacing the original position (likely to move upward). Thomas High School's overall pass rate position will significantly drop (originally at 2nd place).
<br>
###### Post Replacement
![image of change](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/NaN_Affect.png)
###### Pre Replacement
![image_before_change](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/THS_placing_before_change.png)
<br>
Comparing the picture above, the percentages in math, reading and overall all reduced to below 70% (originally above 90%). This may change the standing or the reviews of the school from "Good" to "Not So Good". Images below are modifications that consider 10-12th students grade at THS which remained their position at 2nd place. The position will drastically change from Top 5 to Bottom 5 if 9th grade students are considered.
<br>
#### Top 5 Schools Based on Overall Passing Percentage
![](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/Top5.png)
<br>
#### Bottom 5 Schools Based on Overall Passing Percentage
![](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/Bottom5.png)
<br>

###### Modified THS Data
![](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/Modified_THS.png)
<br>

Replacing 9th grade will reduce the results in the following criteria:
- reduce in student counts 
  - since all 9th grades are removed, the population of THS will drop from 1635 to 1174 ![](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/THS_Count.png)

- raise in per student spending
  - population remove affect `budget/population where population decreased but budget remains the same`
  - originally at range $630-644, removing 9th greade population will increase the amount to $645-675 range ![](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/by_spending.png)

- pull down the average score by school size
  - drop in all passing percentages
  - percentages will decrease if no fix are applied 
  - THS population remains in the same range (Medium) since its from 1635 to 1174 ![](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/by_size.png)
- score by school type
  - Thomas High School is in the "CHARTER" type
  - removing THS 9th grade scores reduces all passing percentages
  - ##### Before
    ![](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/by_type(before).png)
  - ##### After
    ![](https://github.com/WilliamBHW/School_District_Analysis/blob/main/Resources/by_type(after).png)
<br>

## Summary
Overall, changing THS's 9th grade to NaN will drastically affect the school's passing rate in math, reading and both. THS's placement will be dropped and per student capita will increase as the 9th graders are not considered. Population wise, changes in THS will not have significant affect in the district since the population is large which consist of 15 schools. Other schools placement may increase due to ther THS change.
