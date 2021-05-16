# School District Analysis with Jupyter 

## Overview of Election Analysis
The purpose of this analysis was to amalgamate and analyze standardized test data from a school district. By using Pthyon (particularly pandas) within a Jupyter noteboook, we are able to manipulate and synthesize vast amounts of student data, which we can use to gain new insights related to student performance in the district. Ultimately this will help the school board make strategic decisions at the school and district level. 

However, with evidence of academic misconduct at Thomas High School, our intial results needed to be revised. 

## Results 
It appears the students_complete.csv that was used to conduct our intial findings contained evidence of academic dishonesty. Specifically, the math and reading grades of Thomas High school ninth grades appear to have been altered. This affects our analysis in a number of ways. If these dubious grades remain in our data set, all of our grade averages at the school and district level will be skewed. 

Looking at the original school district summary vs. the corrected district summary, we don't see a huge change in the overall data. The school district is so large that removing Thomas High School 9th graders from the data (461 observations) is not enough to drastically shift the overall averages. The total number of students only decreased 1.2%, with all of the passing percentges for Math, Reading, and Overall decreased by less than 1%. 

The summary by school vs. the correctted version is not much different. The change at Thomas High school does not affect the details or outcomes of other schools. For Thomas High School, once the 9th graders where excluded from the average calculations, the % passing grades for Reading, Math, and Overall shifted down by less than 1%. It appears, despite the academic dishonesty, that the THS 9th graders collectively were not outliers in the data, so they did not influence the mean to a large degree when they were included in the data. In fact, Thomas High School is still in the top 5 performing schools even after excluding  the 9th grade scores. 

For the Math and reading scores by grade table, only affected data point is the Thomas high school 9th grade value, with displays "nan". This change had no real affect on the scores by school spending, scores by school size, and scores by school type tables, as the removal of 461 obversations was not enough to shift the averages of the bucket thoas high school was placed in. As a side note: The "scores by school spending" table is somewhat paradoxically inverted. The schools with the highest spending per student had the worst student outcomes. 

## Summary 
To conclude, the removal of the THS 9th graders from the data did not drastically affect the overall results of the school district. Since only 461 observations were removed from a data set of 38,709 observations, the averages for the district as a whole, as well as the collected groups by school size, school spending, and school type, where largely unaffected by the change. However, Thomas High School's specific test results did see a slight change. THS average student test performance for reading, math, and overall did shift downward slightly with the removal of their 9th grade class from the data set. 
