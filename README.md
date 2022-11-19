# An Exploration of Education…By the Numbers
-----------------------------------------------------------------------------------------------------------------------------------------------------------
![giphy](https://user-images.githubusercontent.com/115101031/202830993-5df3e097-e1ec-483a-a52b-70b00c2adfc0.gif)

##Background

When considering the quality of education and outcomes for success there are a number of variables that can be explored as contributing factors. School size, and as a result class size is one of the small number of variables thought to influence student learning.  Another is school budget, which can influence decisions on pupil/teacher ratios in classes.  Additionally, as charter school enrollments grow, school districts may struggle with the redirection of funding which impact the availability of resources and learning in the classroom.

The question remains if these factors play out in the numbers.  For example, does competition between charter and district schools spur traditional public schools and districts to improve—for the benefit of all?

Sources:

https://www.brookings.edu/research/class-size-what-research-says-and-what-it-means-for-state-policy/
https://www.brookings.edu/blog/brown-center-chalkboard/2019/06/07/charter-schools-good-or-bad-for-students-in-district-schools/ 
https://schoolturnaround.org/factors-that-affect-student-achievement/ 


##Using Pandas to Boost Data Analysis

Pandas will provide a powerful framework for our analysis and has several functions for cleaning, analyzing, and manipulating data, which will help extract valuable insights about our data set. Because of its flexibility and simpler syntax, it is now widely used for data analysis.

Information speaks volumes. Data analysis will provide a snapshot of what students know, what they should know, and what may be needed to help them fulfill their potential. With appropriate analysis and interpretation of data, the school board, schools, and educators can make informed decisions that positively affect student outcomes, and equally important, data and analytics also play a vital role in addressing inequalities in education.

In this task, student performance in math and reading was measured by:
•	District
•	School
•	Overall performance (both highest and lowest)
•	Grade level
•	School budget and spending
•	School size
•	School type (District versus Charter)

Sources:
https://towardsdatascience.com/boost-your-data-analysis-with-pandas-69c4be5d73bb
https://sedl.org/pubs/sedl-letter/v22n02/using-data.html 


##Technical Observations

Educator's and school districts have long collected and used a wide variety of data, including examining standardized test scores to measure district-wide achievement. Tools like Pandas has greatly increased the opportunities to use data and analytics. Using Pandas to take on this challenge gave me a front-row seat to why it is the most popular tool among data scientists.

Pandas makes it simple to do many of the time consuming, repetitive tasks associated with working with data, including:
* Data cleansing
* Data fill
* Data normalization
* Merges and joins
* Data visualization
* Statistical analysis
* Data inspection
* Loading and saving data

Our data set included a range of data points, including:
* School informaiton for the district - schools, student population size, type of school, school budget
* Student information: names, gender, grade, home school, math scores, reading scores 


##Observations on the Results

* District Summary: Includes a total of 15 schools and 39,170 students. As a district, students perform better in reading than in math.  It is also clear that there are schools that underperform overall, weighting the overall percentage passing to 65%.
<img width="909" alt="District Summary" src="https://user-images.githubusercontent.com/115101031/202832825-6f51f961-b6e0-4c66-ad60-7fc8d5b99ca4.png">

* School Summary: The largest schools were District schools, had the largest budgets, and spend the most per student.  Charter schools by comparison are smaller and generally have smaller budgets.  District schools represented the lowest performing schools across math, reading, and overall scores.  The top 5 performing schools were all Charter schools, while District schools populated all positions in the bottom 5 schools.  A conclusion might be drawn that smaller schools have smaller class sizes and therefore more individual attention for each students.  Budget did not seem to be a contributing factor, as bigger schools, with bigger budgets seem to lag in student performance.

<img width="994" alt="Top Performing Schools" src="https://user-images.githubusercontent.com/115101031/202833629-c44aa74d-2da2-4fcc-bb6a-3ad7c3401798.png">

<img width="993" alt="Bottom Performing Schools" src="https://user-images.githubusercontent.com/115101031/202833640-a553a992-4395-4cc7-9794-9922d6053725.png">

* Scores by Grade: Across each school, there was consistency with math and reading scores from grade to grade.  Students performed better in reading than in math.  The results provided insight as to prioritizing curricular resources and effort on improving math skills across the grades, whether a revision of the curriculum, or additional teaching support to improve foundational capacity. 

<img width="316" alt="Math Scores by Grade" src="https://user-images.githubusercontent.com/115101031/202834651-e7471b3f-aef5-445d-ab64-833fe71e2cb6.png">

<img width="316" alt="Reading Scores by Grade" src="https://user-images.githubusercontent.com/115101031/202833784-ee952751-6025-49e2-823a-f8263b3c415a.png">

* Scores by Spending: School budgets did not seem to be an indicator of student performance.  Schools that spent more per student had the lowest scores.  It provides insight to take a closer look at how the budget is being allocated.  How are schools with smaller budgets using their resources effectively, and how can that inform policies and practices across the district.

<img width="807" alt="Scores by Spending" src="https://user-images.githubusercontent.com/115101031/202834003-1c33cd9e-ab2a-4a06-9a6b-1b4b7f1a5fa8.png">
                                                                                                                                                     
* Scores by Size: Overall, schools with less than 2000 students performed better than larger schools.  It could be hypothesized that smaller schools would have smaller classes, and therefore, more individual attention to students.  Clearly, class size has an impact on student performance.
                                                                                                                                                         <img width="833" alt="Scores by Size" src="https://user-images.githubusercontent.com/115101031/202834080-095177b6-d890-4d89-baa1-323818361443.png">
                                                                                                                           
* Scores by Type: There was a significant difference between District and Charter schools in terms of student performance in all categories.  Charter schools are publicly-funded, tuition-free schools, but they differ from traditional public schools in key ways. First, charters have more flexibility. Rather than being part of a public school district, which dictates curriculum and standards in all schools, charters operate autonomously through individual agreements, or charters, with state or local governments that dictate rules and performance standards. Given the ability to operate through these agreements, individual charter schools can tailor their curriculum, academic focus, discipline policy and other matters generally decided at the school district or state board level. In return for that flexibility, charter schools are supposed to be more accountable to parents and the state or local governments that authorize them. (Source: https://www.usnews.com/education/k12/articles/understanding-charter-schools-vs-public-schools). This offers an interesting prospect of growing the number of charter schools in the district.  Given their smaller operating budgets and tailored curriculum, this would equalize and improve opportunities for more of the communities families.

<img width="803" alt="Scores by Type" src="https://user-images.githubusercontent.com/115101031/202834300-d4f7f393-cc65-49d7-963c-db63524f22c7.png">
                                                                                                                  
##Next Steps

Clearly, there is much more that we can learn from the data.  When considering the quality of education and outcomes for success there are a number of additonal variables that can be explored, including enhancing the visualization of the data broadening the data set to compare district data with other district, state date and national results; exploring soci-economic and racialized impacts on performance (as a byproduct of school and resources), and examining trends over time by school and student.

