# School_District_Analysis
 Using Python to analyze school district data.
 
## Overview of the school district analysis
The purpose of this analysis was to help Maria identify whether academic dishonesty happened for the Thormas High School math and reading grades. Maria asked us to replace all the math and reading scores for THS to NaNs while leaving the rest of the data untouched. Once we replaced the scores, we re-ran the analysis to provide infromation on how the NaNs affected the data.

## Results

- How is the district summary affected?
- The district summary is very efected by us removing the ninth grade scores. We removed 461 students out of 39,170 students.

- How is the school summary affected?
- The school summary is also not very affected by the changes.

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- Prior to replacing the ninth grader's math and reading scores for THS, the school was doing relatevely low with as 65% overall passing percentage. After our changes, their overall passing percentange increaded to 91%.

#*Step 3. Refactor the code in Step 2 to replace the math scores with NaN.**

-*student_data_df.loc[(student_data_df["school_name"] == "Thomas High School") & (student_data_df["grade"] == "9th"), ["reading_score"]] = np.nan*

-*student_data_df.loc[(student_data_df["school_name"] == "Thomas High School") & (student_data_df["grade"] == "9th"), ["math_score"]] = np.nan*

- How does replacing the ninth-grade scores affect the following:
- Math and reading scores by grade
- Scores by school spending
- Scores by school size
- Scores by school type



## Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

The four major changes in the updated school analysis 
