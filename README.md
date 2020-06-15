# School_District_Analysis

## Challenge overview

### Background

The grades of the ninth graders at Thomas High School have been changed. While administrators do not know the full extent of this academic dishonesty, they want to uphold the standards of state testing and have turned to you for help.

After assessing the situation with the school superintendent and Maria, you decide the best approach is to:

- Replace the ninth-grade math and reading scores from Thomas High School.
- Keep all other data associated with the ninth-grade students and Thomas High School intact.

### Objectives
The goals of this challenge are for you to:
- Filter DataFrames using logical operators.
- Replace the incorrect values with NaN.
- Explain how your PyCitySchools analysis changes after you handle the incorrect data. 

### Analysis Results

461 students have been impacted by the data alteration:
- On the 39,170 total students, they represent only 1.2% of them: thus, the impact on the results should be limited for overall recap
- On the opposite, these students represent 28.2% on the total students of Thomas High School (total: 1,635): it might be a larger impact for School summary


#### District Summary 
##### Without data alteration
![Images/District_Summary_wa.png](Images/District_Summary_wa.png)

##### With data alteration
![Images/District_Summary.png](Images/District_Summary.png)

##### Conclusion
Averages and passing percentages have very slightly dropped because of data alteration.
This small changes are due to the low percentage of population affected by the modification.

---
#### School Summary 
##### Without data alteration
![Images/School_Summary_wa.png](Images/School_Summary_wa.png)

##### With data alteration
![Images/School_Summary.png](Images/School_Summary.png)

##### Conclusion
Only Thomas High School data changed.
For this high school, averages did not vary a lot: the averages of the "erased" grades of the 461 students are the same as the others students. 
9th grade have the same level in math and reading as the other grades.

Thomas High School percentages dropped a lot because of the data alteration. As grades have been set to "NaN", averages computed (using the mean() method) did not took into account these "erased" data. On the opposite, passing percentages took into account these data because we divided the number of grades above 70 by the total number of students without excluding the 461 students of the 9th grade.
This could flaw the result for this high school and its interpretation if we do not remember/precise this fact.

---
#### Top 5 School Summary 
##### Without data alteration
![Images/School_Summary_Top_5_wa.png](Images/School_Summary_Top_5_wa.png)

##### With data alteration
![Images/School_Summary_Top_5_wa.png](Images/School_Summary_Top_5.png)

##### Conclusion
As mentioned in the **School Summary** above, as overall passing percentage dropped a lot, Thomas High School has been kicked out of the top 5 to the advantage of Shelton High School (the above charts are sorted descending on this criteria).

---
#### Bottom 5 School Summary 
##### Without data alteration
![Images/School_Summary_Bottom_5_wa.png](Images/School_Summary_Bottom_5_wa.png)

##### With data alteration
![Images/School_Summary_Bottom_5.png](Images/School_Summary_Bottom_5.png)

##### Conclusion
Even if Thomas High School overall passing percentage dropped a lot, they did not drop enough to join the bottom 5 schools (the above charts are sorted ascending on this criteria). The bottom positions did not change.

---
#### Math Score by Grades
##### Without data alteration
![Images/School_Summary_Math_Score_by_Grade_wa.png](Images/School_Summary_Math_Score_by_Grade_wa.png)

##### With data alteration
![Images/School_Summary_Math_Score_by_Grade.png](Images/School_Summary_Math_Score_by_Grade.png)

##### Conclusion
The data did not change except for Thomas High School for which they are not available for 9th grade.

---
#### Reading Score by Grades
##### Without data alteration
![Images/School_Summary_Reading_Score_by_Grade_wa.png](Images/School_Summary_Reading_Score_by_Grade_wa.png)

##### With data alteration
![Images/School_Summary_Reading_Score_by_Grade.png](Images/School_Summary_Reading_Score_by_Grade.png)

##### Conclusion
As for Math score, the data did not change except for Thomas High School for which they are not available for 9th grade.

---
#### Score by School Spending
##### Without data alteration
![Images/Score_by_School_Spending_wa.png](Images/Score_by_School_Spending_wa.png)

##### With data alteration
![Images/Score_by_School_Spending.png](Images/Score_by_School_Spending.png)

##### Conclusion
Thomas High School has a spending by student equal to $638. The bin "$630-644" is thereby the only affected. 
As mentioned above and as Thomas High School 9th have similar averages as the other grades of this school, the averages are not impacted.
Only passing percentage changed because of the fact detailed on **School Summary**.

---
#### Score by School Size
##### Without data alteration
![Images/Score_by_School_Size_wa.png](Images/Score_by_School_Size_wa.png)

##### With data alteration
![Images/Score_by_School_Size.png](Images/Score_by_School_Size.png)

##### Conclusion
Thomas High School has 1,635 students. The bin "Medium (1000-2000)" is thereby the only affected.
Same remarks as the ones made in the **Score by School Spending**.

---
#### Score by School Type
##### Without data alteration
![Images/Score_by_School_Type_wa.png](Images/Score_by_School_Type_wa.png)

##### With data alteration
![Images/Score_by_School_Type.png](Images/Score_by_School_Type.png)

##### Conclusion
Thomas High School is a charter School. Thus, only the "Charter" is affected.
Same remarks as the ones made in the **Score by School Spending**.

---
