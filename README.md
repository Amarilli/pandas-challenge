# Pandas Challenge

**Summary of the analysis**

In this assignment, I created and manipulated Pandas DataFrames to examine school and standardized test data. 
The first task was to analyze the district-wide standardized test results (math and reading scores) to showcase trends in school performance.
I built a high-level snapshot of the district's key metric in a DataFrame that includes:

* Total number of unique schools
* Total students
* Total budget
* Average math score
* Average reading score
* The percentage of students who passed math
* The percentage of students who passed reading
* The rate of students who passed math and reading

Then, I created a new DataFrame for the above calculations called `district_summary`.
At this point, I created another DataFrame that summarized crucial metrics about each school, including:

* School name
* School type
* Total students
* Total school budget
* Per student budget
* Average math score
* Average reading score
* The percentage of students who passed math
* The percentage of students who passed reading
* The rate of students who passed math and reading. 

I recapped the results in `per_school_summary`.
Also, in `top_school`, I displayed the top 5 schools where students passed math and reading.
In `bottom_school`, I displayed the lowest-performing school.
Then, I calculated the average math and reading score for students of each grade level (from 9th to 12th grade).
Also, to individuate a possible trend, I created a table that broke down school performance based on average spending ranges per student. I displayed the result in `spending_summary`, which included:

* Average math score
* Average reading score
* The percentage of students who passed math
* The percentage of students who passed reading
* The rate of students who passed both math and reading
 
Besides, in `size_summary`, I showed school performance based on school size (small, medium, or large).
Lastly, in `type_summary`, I displayed performance based on the school type. 

**Results:**

One of the first things to notice is that the five highest-performing schools are Charters, while the five lowest-performing schools are district type.
The school budget for the top schools is around 1 million dollars, with a max of  $1,319,574 for Wilson High School and a min of $585,858 for Pena High School. Wilson High School is the largest Charter school of the sample analysis (2283 students), while Pena is one of the smallest (962 students).

The budget for the lowest-performing schools is higher, with a max of $3,094,650 for Johnson High School and a min of $ 1,884,411 for Figueroa High School. However, the number of students in these schools is higher: Johnson has 4,761 students, and Figueroa has 2,949 students. 

If we examine the budget Charter and District invest per student, it is noticeable that they all spend around $600 per learner (from a max of $655 for Huang High School to a minimum of $578 for Wilson High School).
Therefore, the budget per student is *not* a factor that influences the student's success in passing math and reading standardized tests. 

The `size_summary` shows that small schools (with less than 1000 students) and medium-sized schools (between 1000 and 2000 students) have high rates of success in both math and reading (89.883853% and 90.621535%). On the contrary, large schools, with more than 2000 students, reach only 58.286003% in both subjects: the difference is due to the low rate of students passing math (only 69.963361% while the reading rate is 82.766634%).

In `type_summary`, it is visible that Charter schools have better results, both in math and reading scores(83.473852%, 83.896421%) and in passing both subjects( 90.432244%).
The overall passing rate for the district is just 53.672208% due to the low percentage of passing math (66.548453%). 

In ***conclusion***, school size is the best indicator to predict success in reading and math tests. Small and medium size schools perform better, and generally, Charter schools achieve more satisfactory results. Except for Wilson High School and its 2283 students, all charter schools have less than 2000 students, so they are considered medium or small. 

For a deeper analysis, it would be interesting to know the student-teacher ratio of the schools in this analysis. If the smaller schools have a higher proportion of teachers per student, we can deduce that more than the budget, to be successful in passing reading and math tests, it is essential to have more teachers per student. In particular, more math teachers, since math is the subject with a lower percentage of success.
