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

