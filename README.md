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
The district summary is affected, setting Thomas High School math grade for 9th grade students are set to NaN will affect the columns math, reading, and overall.
<br>
![image of change]()
<br>

The school summary is affected in columns math, reading, and overall in the percentage pasing.
<br>
![image of change]()
<br>

Thomas High Schools performance is significantly dropped in overall passing rate in both reading and math, which will allow other high schools percentage replacing the original position (likely to move upward). Thomas High School's overall pass rate position will significantly drop (originally at 2nd place).
<br>
![image_before_change]()
![image_after_change]()
<br>

Replacing 9tth grade will reduce the results in the following criteria:
- reduce in student counts (since all 9th grades are removed)
- raise in per student spending (population remove afect budget/population where population decreased but budget remains the same)
- pull down the average score by school size (drop in math, reading and overall percentage)
- score by school type
