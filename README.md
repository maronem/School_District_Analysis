# PyCitySchools Challenge

## Overview
The purpose of this analysis was to use a clean a dataset of reading and math scores of 9th-12th graders from selected High Schools 
and assess the impact of school attended, grade, school spending, school size, and school type on passing percentage. This analysis 
was completed using the Pandas software library and Jupyter Notebook. Math and reading scores from 9th graders at Thomas High School
(THS) were replaced with "NaN" using the np.nan function. 

## Results

### Effect on the District Summary
Removing THS 9th grader scores effected the school district grade summary by:
* Decreasing the average math score from 79 to 78.9, decreasing the percentage of students passing math from 75 to 74.8%, decreasing the 
percentage of students passing reading from 86 to 85.7%, and decreasing the overall passing percentage from 65 to 64.9%.
* Had no effect on the placement of THS at 2nd among the 15 schools in the district in terms of overall passing percentage. While the
overall passing percentage was decreased from 90.6% to 90.5% this did not affect the standings.

**District summary with THS 9th Graders**

![district_summary_pre](https://user-images.githubusercontent.com/108199140/181410318-3416269c-3052-459e-8e17-ee9c44ae5c92.PNG)

**District summary without THS 9th Graders**

![district_summary_post](https://user-images.githubusercontent.com/108199140/181410322-4913ba03-4eb8-4a4c-b856-27ec83ac430e.PNG)

**Top 5 Schools with THS 9th graders**

![top_5_pre](https://user-images.githubusercontent.com/108199140/181413761-b108bbff-becc-44cd-9448-33676c30c73f.PNG)

**Top 5 Schools without THS 9th graders**

![top_5_post](https://user-images.githubusercontent.com/108199140/181413804-8b41314e-324e-4f95-aa21-0ebff69e11ab.PNG)

### Effect on the School Summary
By replacing the scores of 9th graders from Thomas High School, the school summary was affected by:
* An increase in the average math score for the school from 66.9% to 93.2%.
* An increase in the average math score for the school from 69.7$ to 90.7%.

**With 9th Graders**

![per_school_pre](https://user-images.githubusercontent.com/108199140/181399553-1fa049cb-8950-40ea-b4c7-160f51256526.PNG)

**Without 9th Graders**

![per_school_post](https://user-images.githubusercontent.com/108199140/181399559-f8ea5c98-31c4-4aae-8778-dca90470f2c5.PNG)


### Effect of replacing ninth-grade scores on math & reading scores by grade:
Replacing the scores of 9th graders from Thomas High School, math and reading scores were effected in each grade by:

* All 9th grade scores for students at Thomas High School (THS) were replaced by NaN using the function np.nan (A1 = With 9th graders math,
A2 = Without 9th graders math, B1 = With 9th graders reading, B2 = Without 9th graders reading). 
* No changes were seen in any grade for either reading or math as this only removed grades for 9th graders at THS

**A1)** ![per_grade_math_pre](https://user-images.githubusercontent.com/108199140/181400649-300990f9-91f8-4fa0-afe5-5c92289a7fcf.PNG) **A2)** ![per_grade_math_post](https://user-images.githubusercontent.com/108199140/181400654-0eef6975-6176-4b3a-baee-951311b17052.PNG)


**B1)** ![per_grade_reading_pre](https://user-images.githubusercontent.com/108199140/181400672-f3cd3728-8ce5-4630-a843-5a29cbae8c95.PNG) **B2)** ![per_grade_reading_post](https://user-images.githubusercontent.com/108199140/181400679-5383beaa-cee3-4191-a7ff-ab658a5f06f5.PNG)


### Effect of replacing ninth-grade scores on math & reading scores by school spending:
By replacing the scores of 9th graders from Thomas High School:
* There was no change to the trend that schools which spend a lower cost per student had the highest average scores in both reading and math, higher passing percenteages, an doverall passing percentage. 
* It is noted that while the analysis bins were created differently pre and post removal of the students, the general trends still stand. 


**Math scores per capita with THS 9th graders**

![per_capita_pre](https://user-images.githubusercontent.com/108199140/181404705-1c4b69e2-142e-4582-b8cc-37db113f29c9.PNG)

**Reading scores per capita without THS 9th graders**

![per_capita_post](https://user-images.githubusercontent.com/108199140/181404710-92e52721-5e68-4b5d-a3a3-4cfe35949d20.PNG)


### Effect of replacing ninth-grade scores on math & reading scores by school size:
By replacing the scores of 9th graders from Thomas High School:
* The percentage of students passing reading for medium sized schools decreased from 97% to 95%, this suggests 9th graders from THS were
performing strongly in percentage of students passing reading.
* This also shows that THS is a medium sized school (1000-1999 students), which was also validated in the analysis and shown in section figure A3.


**A1) Scores by school type with THS 9th graders**

![by_size_pre](https://user-images.githubusercontent.com/108199140/181405927-3302cbef-443d-4e76-9d04-32432cb0fccb.PNG)

**A2) Scores by school type without THS 9th graders**

![per_size_post](https://user-images.githubusercontent.com/108199140/181405935-b1835980-5c28-4f96-ae6a-1b7612f34569.PNG)

**A3) School size for THS**

![THS_size](https://user-images.githubusercontent.com/108199140/181407001-18787c11-5cb1-40b1-82f1-dd1dd7862ef4.PNG)

### Effect of replacing ninth-grade scores on math & reading scores by school type:
By replacing the scores of 9th graders from Thomas High School:
* The percentage of students passing reading in Charter type schools was decreased from 97% to 96%, which is consistent in showing a high percentage
of THS 9th graders passing reading.
* This also shows that THS is a charter type school which is also shown in section figure A3.

**Scores by school type with THS 9th graders**

![by_type_pre](https://user-images.githubusercontent.com/108199140/181407149-fb667760-6e45-41a9-bd66-d147f2ec226a.PNG)

**Scores by school type with THS 9th graders**

![by_type_post](https://user-images.githubusercontent.com/108199140/181407163-f888cdf5-3160-48d4-86ab-ee56a498e27d.PNG)

**THS is a Charter type school**

![THS_size](https://user-images.githubusercontent.com/108199140/181407579-a0d93a86-6ad0-4132-bf28-82ad2731a0a8.PNG)

# Summary
Replacing the math and reading scores for 461 THS 9th graders did not alter data strongly, while percentages were slightly different there was no
difference in the outcome of the data. Math and reading scores by grade were unaffected, except for 9th grade scores as these were replaced with NaN. 
Scores by school spending were unchanged with schools with lower per capita spending having higher passing percentages and scores for both math and 
reading. The percentage of students passing reading for medium sized schools decreased form 97% to 95%, moving medium sized schools into second behind small sized schools (<1000 students) for the highest percentage of students passing reading. Lastly, replacing THS 9th grader scores with "NaN" decreased the percentage of students at Charter schools passing reading from 97% to 96% but this did not change that Charter schools perform better in all categories compared to District schools. 
