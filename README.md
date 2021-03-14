# School_District_Analysis1
Anaconda Python Software

Here is the list of deliverables for the analysis of the school district: 

A high-level snapshot of the district's key metrics, presented in a table format
An overview of the key metrics for each school, presented in a table format
Tables presenting each of the following metrics:
Top 5 and bottom 5 performing schools, based on the overall passing rate
The average math score received by students in each grade level at each school
The average reading score received by students in each grade level at each school
School performance based on the budget per student
School performance based on the school size 
School performance based on the type of school

The school district summary will be a high-level snapshot of the district's key metrics:

Total number of students
Total number of schools
Total budget
Average math score
Average reading score
Percentage of students who passed math
Percentage of students who passed reading
Overall passing percentage


To get the percentage of students who passed math and reading, we will write code to:

Determine the passing grade.
Get the number of students who passed math and reading in separate DataFrames.
Calculate the number of students who passed math and reading.
Calculate the percentage of students who passed math and reading.
To get the overall passing percentage, we will write code to:

Get the number of students who passed both math and reading in a DataFrame.
Calculate the number of students who passed both math and reading.
Calculate the percentage of students who passed both math and reading.


Total number of schools in the column "Total Schools"
Total number of students in the column "Total Students"
Total budget in the column "Total Budget"
Average reading score in the column "Average Reading Score"
Average math score in the column "Average Math Score"
Percentage of students passing reading in the column "% Passing Reading"
Percentage of students passing math in the column "% Passing Math"
Overall passing percentage in the column "% Overall Passing"

Debug and fix errors faster.
Make your code more readable.
Reuse code by importing functions into other algorithms.
Speed up programming development. Multiple team members can work on separate functions of a complex algorithm to speed up the development of the project.
A hallmark of professional programmers is that they can take long blocks of code and write smaller pieces of that code as functions.

There are four basic parts to a function:

The name, which is what we call the function
The parameters, which are values we send to the function
The code block, which are the statements under the function that perform the task
The return value, which is what the function gives back, or "returns," to use when the task is complete


The name cannot be a Python keyword.
The name cannot contain spaces.
The first character of the name must be an uppercase or lowercase letter or an underscore.
After the first character, you can use uppercase and lowercase letters, digits 0 through 9, or an underscore.

We added two values to the passing_math_percent function: pass_math_count and student_count.
We added return in front of the calculation for the passing percentage.

In this code, there is a list of grades formatted to two decimal places. To format these grades to the nearest whole number percent, we will do the following:

Iterate through the grades.
Pass the grade variable inside the format() function.
Specify the format for the grade variable we would like by using {:.0f}.
In this format, the gradevariable is referenced in front of the colon, so there is no need to add the grade variable.
After the colon, the .0f means to format the grade with no decimal place, where the "period" is for the decimal place, the "0" is for "no" decimal place, and the "f" means floating-point decimal. If we wanted to format to one decimal place, we would use 1 instead of 0, and 2 for two decimal places, and so on.


The order of the columns in the district_summary_df DataFrame should be as follows:

Total Schools
Total Students
Total Budget
Average Math Score
Average Reading Score
% Passing Math
% Passing Reading
% Overall Passing

This next project requires you to get the following key metrics for each school and place them in a school summary DataFrame. As a reminder, here are the key metrics you're working with: 

School name
School type
Total students
Total school budget
Per student budget
Average math score
Average reading score
% passing math
% passing reading
% overall passing

Now that we have performed all the calculations needed for the school summary, we can add the following values to a new DataFrame named per_school_summary_df. The data and columns of the DataFrame will be:

Type of school in the "School Type" column
Total students per school in the "Total Students" column
Total budget per school in the "Total School Budget" column
Total budget per student for each school in the "Per Student Budget" column
Average math score for each school in the "Average Math Score" column
Average reading score for each school in the "Average Reading Score" column
Percentage of students passing math for each school in the "% Passing Math" column
Percentage of students passing reading for each school in the "% Passing Reading" column
Overall passing percentage for each school in the "% Overall Passing" column


In the per_school_summary_df DataFrame, we will format the Total School Budget and Per Student Budget columns to include:

A U.S. dollar sign 
Two decimal places
A thousands separator


If the columns were not ordered correctly, put them in the following order:

School Type
Total Students
Total School Budget
Per Student Budget
Average Math Score
Average Reading Score
% Passing Math
% Passing Reading
% Overall Passing

Looking at the per_school_counts Series, we can see that the highest student population is 4,976. Therefore, the upper edge will be 5,000. Because we have only three bins—small, medium, and large—here's how we can group the school sizes:

"Small" schools have fewer than 1,000 students
"Medium" schools have 1,000–1,999 students
"Large" schools have 2,000–5,000 students


