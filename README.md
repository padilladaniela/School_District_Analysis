# School_District_Analysis
 Using Python to analyze school district data.
 
## Overview of the school district analysis
The purpose of this analysis was to help Maria identify whether academic dishonesty happened for the Thormas High School math and reading grades. Maria asked us to replace all the math and reading scores for THS to NaNs while leaving the rest of the data untouched. Once we replaced the scores, we re-ran the analysis to provide infromation on how the NaNs affected the data.

## Results

- The district summary is effected by us removing the ninth grade scores. We removed 461 students out of 39,170 students. The scores before and after the update greatly differentiate.

![district_summary](https://github.com/padilladaniela/School_District_Analysis/blob/main/school_district_summary.png)

- The school summary is affected as well. The percentages changed from our initial scores to the updated.

![school_summary](https://github.com/padilladaniela/School_District_Analysis/blob/main/School_summary.png)

- Prior to replacing the ninth grader's math and reading scores for THS, the school was doing relatevely low with as 65% overall passing percentage. After our changes, their overall passing percentange increaded to 91%.

*Step 3. Refactor the code in Step 2 to replace the math scores with NaN.**

-*student_data_df.loc[(student_data_df["school_name"] == "Thomas High School") & (student_data_df["grade"] == "9th"), ["reading_score"]] = np.nan*

-*student_data_df.loc[(student_data_df["school_name"] == "Thomas High School") & (student_data_df["grade"] == "9th"), ["math_score"]] = np.nan*

- How does replacing the ninth-grade scores affect the following:

- Math and reading scores by grade

![math and reading scores by grade](https://github.com/padilladaniela/School_District_Analysis/blob/main/reading_scores_per_grade.png)

- Scores by school spending

![school_spending](https://github.com/padilladaniela/School_District_Analysis/blob/main/before_after_spending.png)

- Scores by school size)

![school_size](https://github.com/padilladaniela/School_District_Analysis/blob/main/before_after_school_size.png)

- Scores by school type

![Before_reading](https://github.com/padilladaniela/School_District_Analysis/blob/main/before_school_type.png)

![Updated_Reading](https://github.com/padilladaniela/School_District_Analysis/blob/main/updated_school_type.png)


## Summary

The four major changes in the updated school analysis:
- The differences in all of our DataFrames was minimal.
- We were able to identify differences in the actual data and how much it affected the overall results.
- By removing the ninth grade math and reading, we are able to show Maria how this data changes. The distrcit summary was affected the most from our changes.
- After removing the NaNs, we were able to learn how to refactor data to pull information as wanted using pandas and numpy. Maria can possibly use this code and rerun with any scores she would like to remove or update.

