# School_District_Analysis

## Overview of the school district analysis.
  The school board has notified Maria and her supervisor that there is some evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders. Maria asked us to replace the math and reading scores for Thomas High School with NaNs (Not-A-Number) while keeping the rest of the data intact. Maria asked to repeat the school district analysis and write up a report to describe how these changes affected the overall analysis following the change in scores for Thomas High School. This analysis will be done in different scopes, focusing on factors such as school spending, school size, and school type. This analysis is done using Python in Jupyter notebook.

## Results: Using bulleted lists and images of DataFrames as support, address the following questions.
- How is the district summary affected?
    - The district summary is minimally affected by the change in data. Average math score decreased by 0.1 points, the average reading score remained unchanged, the % Passing math decreased by 0.2%, the % passing reading decreased by 0.3% and the % Overall Passing decreased by 0.1%. All of the changes above were less than 1% indicating the change in data was minimal following the omission of the suspicious scores.
  
  ![District Summary](https://user-images.githubusercontent.com/64291905/142790070-a8eb8174-7e89-457b-8876-0e5975d2ae7d.PNG)

- How is the school summary affected?
    - The school summary is affected pretty significantly with the omission of THS' 9th grade class. Passing Math % decreased from 93% to 66% and Passing Reading % decreased from 97% to 69% resulting in a new Overall Passing % of 65% from 91%. This is a pretty drastic change with around a 25% swing seen after omission of the 9th grade class. None of the other school's individual scores had changed because that data was not touched. 

![School Summary 2](https://user-images.githubusercontent.com/64291905/142790155-5da5d7f7-fdd8-487f-89ed-a5b626978dab.PNG)

![School Summary](https://user-images.githubusercontent.com/64291905/142790081-b0a27ba8-af70-45c1-9a0d-3cc6abcb1907.PNG)

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
    - Before the results were changed, THS was ranked #2 in the schools based on overall percentage, but after the change it fell to #8. All schools that were 3-8 moved up 1 spot respectively, while Thomas had fallen significantly.
  ![Bottom 5 Schools](https://user-images.githubusercontent.com/64291905/142800003-c42f02f4-287b-4ffa-ba38-9f12782b9a28.PNG)

- How does replacing the ninth-grade scores affect the following:
    - Math and reading scores by grade were not affected in any schools except for THS because that was the only data that was altered. THS only had changes in the 9th grade section as that was the data that was changed. At THS, 9th grade math changed from 83.6% to NaN, and 9th grade reading changed from 83.7% to NaN. 

![Math and Reading Scores by Grade](https://user-images.githubusercontent.com/64291905/142790107-e25c78f9-02df-4e06-9e81-6b70a97ff3e4.PNG)

  - Scores by school spending
    - THS was within the $630-$644 range, so the differences caused by the altered data fell within this range only. Passing Math % fell to 67% from 73%, Passing Reading % fell to 77% from 84%, and Overall % Passing fell to 56% from 63%.
![Scores by School Spending](https://user-images.githubusercontent.com/64291905/142799979-8d4e1b0f-1b9b-4b55-b059-3714823fe013.PNG)

  - Scores by school size
    - THS fell within the Medium(1000-2000) school size, so only this bin was affected as THS was the only school with data that was changed. The % Passing Math fell to 88% from 94%, the % Passing Reading fell to 91% form 97%, and the % Overall Passing fell to 85% from 91%.

 ![Scores by School Size](https://user-images.githubusercontent.com/64291905/142799987-d3c8623c-6a8d-46aa-aa76-f7d1e9ce3585.PNG)

  - Scores by school type
    - THS was classified under "Charter School", so only this category was affected by the changes in data. % Passing math fell to 90% from 94%, % Passing Reading fell to 93% from 97%, and % Overall Passing fell to 87% from 90%.

 ![Scores by School Type](https://user-images.githubusercontent.com/64291905/142799992-927b4e6a-9566-4b93-b1df-4af16eff1719.PNG)

## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
  1. The largest change was within the results of THS itself. Dropping each of the metrics by around 25% indicates the school is performing far worse than it was originally thought to be. This could result in changes to funding, as well as indicating the need for a document integrity initiative.
  2. Going hand in hand with the above point is the ranking of THS in the district as a whole. Dropping 6 spots is significant when there are only 15 schools in total. Thats a movement that is equivalent to almost half of all schools in the district. The school may be viewed in a lower light with the lower ranking, resulting in decreased funding.
  3. THS fell within one of the larger 2 spending ranges per student, and both of these higher ranges actually have lower Overall % Passing. This is an interesting thing to note because even though the school is contributing more to their students in terms of monetary value, they are falling short in testing. This could indicate that there needs to be more quality time among faculty and students, rather than continuing to spend higher dollar amounts on things that aren't bearing fruition for testing results.
  4. With the changes to the data, schools with a size of "small" actually ended up being in the #1 spot in terms of testing %s. This might indicate that there is a benefit to being in a smaller school, potentially because the faculty to student ratio is smaller allowing for more 1:1 time encouraging better grasp of the material. Correlation doesn't indicate causation, but it may be something worth looking into. 
