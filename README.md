# Challenge_04_PythonPdJN_PyCitySchools
This is the challenge

# PyCitySchools with Pandas

## Overview of Project
Based on the data provided by the school board, there was evidence of certain academic dishonesty in the Thomas High School 9th grade students, since there is no knowledge of the full extent, there must be a complete analysis for all schools while there is a need to remove the 9th graders from Thomas High School (THS).

### This project includes:
- The district summary
- The school summary
- The top 5 and bottom 5 performing schools, based on the overall passing rate
- The average math score for each grade level from each school
- The average reading score for each grade level from each school
- The scores by school spending per student, by school size, and by school type

### Purpose
Remove 9th graders from Thomas High School and adjust the measures in order to visualize the data without the information that can be from thesource of the possible academic dishonesty. This will make the calculations as fast as possible while working in an enviornment that will help visualize the results the code gets.

## Analysis and Challenges
To make this challenge, there is a need to know the code that is going to help in the cleaning of the information. In this case, is also important the use of numpy with the .nan in order to produce NaN values. Also "loc", "isnull", "notnull" will be needed to produce and seach for NaN values. For the other part of the challenge is important to consider the proper way to write dataframes and series in order to get the information needed.

## Analysis of Outcomes Based on Clean Data
Before cleaning (as shown in the image below), it can be observed that Thomas High School percentage for reading and math were low but after the cleaning, those values increased.

#### Before
![Before cleaning](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/beforecleaning_02.PNG)

#### After
![After cleaning](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/summary_per_school.PNG)

Since it was asked to remove the 9th graders scores from Thomas High School and make a new analysis with the clean data, first, it was needed to make sure the information that was asked to be changed into NaN was really converted. 

![Show the NaN](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/9th_gradersNaNTHS.PNG)

### The district summary

In the district summary for all 15 schools, it is shown the total students, the total budget for all schools, the average math and reading score, and also the passing percentage for those topics and the overall passing of all students. As shown in the image below, in this case it can be seen that the total number of schools that are considered are 15, and in those schools the sum of the number of the students is 39,170, and given the different amount each student have to pay depending on the school, the total budget for all the schools is $24,649,428.00, there must be said that that total is not for each school, but for all of them. The average math score of all is 78.9, while the reading score average is 81.9. The passing percentage counting all the students, is as follows: for math is 74.8% of the students passed; in the case of reading the 85.7% passed. An overall passing for students that passed both topics is 64.9%. 

![District summary](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/district_summary_01.PNG)

### The school summary
Observing the school summary, Bailey High School has the highest number of students and due to the per student budget it has, is the one with the highest school budget, getting an amount of $3,128,928.00. The one with the less students is Holden High School and it has the budget of $248,087.00. The most expensive one is Huang High school, since that school per student budget is $655.00; and the least expensive one is Wilson High School, since it's per school budget is $578.00.

Pena High School is the one with the best average math score of 83.839917 while Huang High School has a math average socre of 76.629414, making it the lowest. In the reading average score, the lead is Pena High School with 84.044699, and the last place is Rodriguez High School with an average of 80.744686.

The highest percentage of students who passed math is 94.6% in Pena High School an the lowest passing math percentage is 65.7% that corresponds to Huang High School. The school with the highest percentage of students that passed reading is Griffin High Shcool with a 97.1% while the lowest is 80.2% that corresponds to Rodriguez High School. The highest percentage of students that passed both math and reading is 91.3% and is from Cabrera High School, the lowest is 53.0% from Rodriguez High School.

With the cleaned data that was made, it can be seen that Thomas High School would had been the lowest percentage in passing reading percentage only.

![School summary](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/summary_per_school.PNG)

### The top 5 and bottom 5 performing schools, based on the overall passing rate
The top five performing schools based on overall passing rate are:
- **1st place:** Cabrera High School
- **2nd place:** Thomas High School
- **3rd place:** Griffin High School
- **4th place:** Wilson High School
- **5th place:** Pena High School

![top 5](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/Top%20Five.PNG)

The bottom five performing schools based on overall passing rate are:
- **1st last place:** Rodriguez High School
- **2nd last place:** Figueroa High School
- **3rd last place:** Huang High School
- **4th last place:** Hernandez High School
- **5th last place:** Johnson High School

![bottom five](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/bottom_five.PNG)

*The bottom five are in order of worst to better percentage*

### The average math score for each grade level from each school
**As shown in the image, since Thomas High School 9th graders math score average has been removed, it will not participate in the 9th grader's evaluation.**

The highest average in math scores goes as follows:
- 9th Grade: Holden High School with 83.8
- 10th Grade: Griffin High School with 84.2
- 11th Grade: Holden High School with 85.0
- 12th Grade: Pena High School with 84.1

The lowest average in math scores goes as follows:
- 9th Grade: Figueroa High School with 76.4
- 10th Grade: Figueroa High School with 76.5
- 11th Grade: Huang and Rodriguez High School with 76.4
- 12th Grade: Ford High School with 76.2


![math average score per grade](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/average_math_per_grade.PNG)

### The average reading score for each grade level from each school
**As shown in the image, since Thomas High School 9th graders reading score average has been removed, it will not participate in the 9th grader's evaluation.**

The highest average in reading scores goes as follows:
- 9th Grade: Shelton High School with 84.1
- 10th Grade: Cabrera and Thomas High School with 84.3
- 11th Grade: Shelton High School with 84.4
- 12th Grade: Holden High School with 84.7

The lowest average in reading scores goes as follows:
- 9th Grade: Ford High School with 80.6
- 10th Grade: Rodriguez High School with 80.6
- 11th Grade: Ford High School with 80.4
- 12th Grade: Huang High School with 80.3

![reading average score per grade](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/average_reading_per_grade.PNG)

### The scores by school spending per student, by school size, and by school type
In the spending ranges per student, the best averages and passing percentage was from the ones that had and spending range from $0 to $584, while the worst averages and passing percentages was from the range of $645 to $675.

![scores by school](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/spending_per_student.PNG)

As shown in the image below, the small school size got a better average in math score and average reading; the medium size got a better math passing percentage, passing reading percentage and overall passing. The lowest average and passing percentages were from the larger size schools.

![scores by size](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/size_cal.PNG)

The school have two types in this case, which is Charter and District. Observing the data, the best results are for the schools that are for the Charter Type of school, while the District Type Schools are lower in the results. In the Math score average, the charter type got 83.5 points, white the district type got 77.0 points. Getting to the Reading score average, the charter obtained 83.9 points while the distric was near with 81.0 points. The math passing percentage in the charter wa 84%, while the district got only 67%. The passing reading percentage in the charter was 97% and in the district was 81%. The overall passing percentage of both reading and math was 90% for charter and 54% for district.

![scores by type](https://github.com/LennethNova/Challenge_04_PythonPdJN_PyCitySchools/blob/main/Resources/school_type.PNG)

### Challenges and Difficulties Encountered
One of the first difficulties encountered during the developement of this code, was from understanding the different variables and data frames, not only for the way they work, but for what they are referring to, what they do and what information was stored in them.


## Results
### Changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs:
- After the scores for the 9th grade changed to NaN, some Thomas High School values changed such as percentages for passing percentage for math, reading and students that passed both.

- That change with NaN also made possible for Thomas High School to make it into the Top 5 performing schools based on the overall passing.

- It also impacted in the bin results due to the change in the passing percentages.

- It helped to improve the school position, but it did not impact on some values since it was not the highest in some points, nor the lowest, except that Thomas High School would had been the lowest percentage in passing reading percentage.
