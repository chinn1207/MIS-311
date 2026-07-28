# MIS-311
Introduction to Business Analytics
## 1. Data Overview 
The name of dataset is *06_Student_Performance*. 
- This dataset has 202 students to show their performance in education.
- It has totally 8 rows:
  
       + Gender: 0 and 1
  
       + Race_ethnicity: Group A, Group B, Group C, Group D, Group E
  
       + Parental_level_of_education: The educational background of the student's family.
  
       + Math_score
  
       + Reading_score
  
       + Writing_score
  
       + Total_score
  
       + Average_score

- The purpose of this dataset is to show the performance of students in 3 subjects: math, reading, writing. Besides that, it also show factors which are affect student's academic performance.
  
  ## 2. Data Cleaning
 The cleaning dataset is the dataset doesn't have missing value, duplicate 
 #### Firstly, checking the missing value 
- Choosing the whole dataset by using Crtl + A, then pressing Crtl + G. Click to Special... -> Blanks -> OK
- Missing values appear in the variable of parental_level_of_education and average_score

`How to process`
- In "parental_level_of_education". There are 3 missing values
- In "average_score". There are 4 missing values. Because this is the average of 3 score that is math_score, reading_score, writing_score, so in Excel using the fuction `=AVERAGE(D2:F2)` to calucate again the average_score
- After deal with missing value, checking the dataset again to make sure that no empty cells are missed. The result is: 
<img width="1920" height="1080" alt="missing_value" src="https://github.com/user-attachments/assets/6133ffdd-125d-40eb-b33f-70684b59b6bb" />


#### Secondly, checking duplicated rows
<img width="1920" height="1080" alt="duplicate" src="https://github.com/user-attachments/assets/38e4ffe1-a3ce-47ee-8251-6d93e11c2442" />



