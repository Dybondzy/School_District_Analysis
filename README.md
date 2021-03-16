# Module 4 Challenge
#
## Purpose
The school board has notified Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked you to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once you’ve replaced the math and reading scores, Maria would like you to repeat the school district analysis that you did in this module and write up a report to describe how these changes affected the overall analysis.


## Overview

This new assignment consists of two technical analysis deliverables and a written report to present your results. You will submit the following:

Deliverable 1: Replace ninth-grade reading and math scores
Deliverable 2: Repeat the school district analysis
Deliverable 3: A written report for the school district analysis (README.md)


Make a copy of your PyCitySchools.ipynb file and rename it PyCitySchools_Challenge_testing.ipynb.

Download the PyCitySchools_Challenge_starter_code.ipynb file, copy the code, and paste it at the top of your PyCitySchools_Challenge_testing.ipynb file.

You’ll use this file to test your code as you work through the challenge.
Once your code is working, you'll make a copy of the PyCitySchools_Challenge_testing.ipynb file and rename it PyCitySchools_Challenge.ipynb.

When you're ready to submit, be sure to check that all DataFrames created for Deliverables 1 and 2 are visible in your outputs. Do not include any unnecessary print statements in your code.


### Deliverable 1

Deliverable 1: Replace Ninth-Grade Reading and Math Scores (50 points)
Deliverable 1 Instructions
Using the Pandas loc method with conditional statements and comparison and logical operators, select the ninth-grade reading and math scores for Thomas High School. Then, use the Pandas NumPy module to change the reading and math scores to NaN.

Use the code snippet provided in Step 1 to import the NumPy module: import numpy as np.

Use the code snippet provided in Step 2 for the Pandas loc method.

To select all the ninth-grade reading scores at Thomas High School, use the following steps to write code inside the brackets of the loc method:

a) Add an opening parenthesis, then use a comparison operator to retrieve all the rows with Thomas High School from the "school_name" column of the student_data_df, then close the parenthesis.

b) Add a logical operator then another opening parenthesis, then use a comparison operator to retrieve all the rows with ninth grade from the "grade" column of the student_data_df, then close the parenthesis.

c) To change the reading scores only, add a comma after the last closing parenthesis then add the "reading_score" column.

d) Outside of the closing brackets of the loc method, set the ninth-grade reading scores from Thomas High School equal to np.nan.

### Deliverable 2

Deliverable 2: Repeat the School District Analysis (25 points)
Deliverable 2 Instructions
Repeat the school district analysis you did in this module, and recreate the following metrics:

The district summary
The school summary
The top 5 and bottom 5 performing schools, based on the overall passing rate
The average math score for each grade level from each school
The average reading score for each grade level from each school
The scores by school spending per student, by school size, and by school type
In Steps 1-4, you’ll update the district summary. For this task, you’ll recalculate the total student count by subtracting the number of ninth-grade students in Thomas High School from the total student count, then you'll recalculate the passing math and passing reading percentages, and the overall passing percentage with the recalculated total student count.

In Steps 5-14, you’ll execute the code from this module that creates and formats the School Summary DataFrame, then update the school summary using the 10th-12th graders from Thomas High School as follows:

First, you’ll calculate the number of 10th-12th graders in Thomas High School.
Create three new DataFrames for the 10th-12th graders from Thomas High School: students who passed math, students who passed reading, and students who passed both math and reading.
Using these DataFrames, you'll recalculate the percentage of students who passed math, passed reading, and passed both math and reading for Thomas High School only.
Finally, you'll replace the % Passing Math, % Passing Reading, and % Overall Passing scores in the current School Summary DataFrame with the new passing percentages for Thomas High School.


### Deliverable 3
