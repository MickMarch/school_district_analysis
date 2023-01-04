# School District Analysis

## Overview of Project

### Purpose

The purpose of this project was to use Jupyter Notebook to analyze a student dataset from a school district.

# Summary

## Data Types

The raw data has the following columns:

- student_id 
  - Type: Integer
- student_name
  - Type: Object
- grade
  - Type: Object
- school_name
  - Type: Object
- reading_score
  - Type: Float
- math_score
  - Type: Float
- school_type
  - Type: Object
- school_budget
  - Type: Integer

## Data Cleanup / Adjustments

It would be worth noting the following items had to be cleaned up, so as to pass along to whomever can improve the data entry methods for this dataset:

- 1968 Reading Scores were NaN, and the entries affected were removed.
- 982 Math Scores were NaN, and the entries affected were removed.
- After the above cleanup, 1836 entries were found to be duplicates and were removed.
- The "grade" column entries had the "th" removed from the data, then the value was converted from "Object" to "Integer".

## Data Analysis

- Math Scores:
  - The average **Math Score** for students was 64.7%
  - **Grade 9 students** in **Charter schools** had the highest average Math Score, at 70%
  - **Grade 11 students** in **Public schools** had the lowest average Math Score, at 59.0%
- The lowest Reading Score entry for the students was 10.5%
- **Charter schools** average school budget was $872,625.66
- **Public schools** average school budget was $911,195.56
- Montgomery High School had the highest student count of 2038. *(Counted using only complete entries after data cleanup)*
- Chang High School had the lowest student count of 171. *(Counted using only complete entries after data cleanup)*


# Bonus: Additional Analysis

## Average Reading Scores by School Type and Grade

By grouping the data by school type and then grade, we were able to determine the average reading scores from that grouping.

![school_type_grade_avg_reading](/resources/school_type_grade_avg_reading.png)

## Budgets Per School

It was worth taking a look at the different school budgets, sorted by school type and then school budget (descending).

![school_budgets_sorted](/resources/school_budgets_sorted.png)