# MIS-311: Introduction to Business Analytics
Individual Assignment 1 - Personal Portfolio

Nguyen Mong Trinh - 2332300163

## 1. Data Overview 
The name of dataset is *06_Student_Performance*. 
- In this dataset, I use analytical tool that is Excel to conduct my analysis. 
- This dataset has 202 students to show their performance in education.
- It has totally 8 columns:
  
       + Gender: 0 and 1
  
       + Race_ethnicity: Group A, Group B, Group C, Group D, Group E
  
       + Parental_level_of_education: The educational background of the student's family.
  
       + Math_score: Student score in math
  
       + Reading_score: Student score in reading
  
       + Writing_score: Student score in writing 
  
       + Total_score: The sum of 3 scores 
  
       + Average_score: The mean of 3 scores

- The purpose of this dataset is to show the performance of students in 3 subjects: math, reading, writing. Besides that, it also show factors which are affect student's academic performance.
  
  ## 2. Data Cleaning
 The cleaning dataset is the dataset doesn't have missing value, duplicate rows
 #### Firstly, checking the missing values 
 `Method`
 
- Choosing the whole dataset by using Crtl + A, then pressing Crtl + G. Click to Special... -> Blanks -> OK (ThomasCoget, 2025)
- Missing values appear in the variable of parental_level_of_education and average_score.

`How to process`

     + In "parental_level_of_education". There are 3 missing values. Missing parental education values were replaced with "Unknown" to ensure integrity of data
     
     + In "average_score". There are 4 missing values. Because this is the average of 3 score that is math_score, reading_score, writing_score, so in Excel using the fuction `=AVERAGE(D2:F2)` to calucate again the average_score (AlexJerabek, 2024).
Then, checking the dataset again to make sure that no empty cells are missed. 

`Result`

<img width="1920" height="1080" alt="missing_value" src="https://github.com/user-attachments/assets/6133ffdd-125d-40eb-b33f-70684b59b6bb" />


#### Secondly, checking duplicated rows
`Method`

- In excel: Data-> Remove duplicate (AlexJerabek, 2024).
  
`Result`

- Identify and remove 3 duplicated rows
<img width="1920" height="1080" alt="duplicate" src="https://github.com/user-attachments/assets/38e4ffe1-a3ce-47ee-8251-6d93e11c2442" />

=> After cleaning, the data has 199 students and 8 fields.

## 3. Descriptive Statistics 
Data -> Data Analysis -> Descriptive Statistic -> Range is from math_score column to average_score column -> OK (“Cách Sử Dụng Tính Năng Thống Kê Mô Tả (Descriptive Statistics) Trong Excel,” 2025). 
- The descriptive statistic show the measures of central tendency (the mean, median, and mode), whereas measures of variability ( standard deviation, variance, minimum and maximum values, kurtosis, and skewness) (Hayes, 2024). 
<img width="1171" height="363" alt="image" src="https://github.com/user-attachments/assets/8c1c3e72-09ff-4a0e-837e-c1df9874fc6e" />



- Two visualisation to present the descriptive statistics.
<img width="696" height="501" alt="image" src="https://github.com/user-attachments/assets/405631b7-a4de-4586-86e4-b753cd64111c" />



<img width="801" height="485" alt="image" src="https://github.com/user-attachments/assets/89445979-9855-41cd-957d-34dd531a4ea0" />



**Insight 1**: 
Students whose parents have bachelor's degree, master's degree tend to achieve higher average scores at about 73.03 and 72.27 respectively, while students whose  parents completed high school, some high school has lower average score just around 62.29, 60.46 repectively. This shows that parental education plays an important role in students' learning. This is because, the parents will provide more support and guidance at home. Based on the statistics, the school can help student whose parents have limited access to higher education by tutoring, academic support programs.

**Insight 2**: The histogram shows that the average scores of most students are concentrated in the middle range. Only a small percentage of students are in very low or very high scores. This indicates that overall academic results are quite balanced.

**The dataset after cleaning**: [Cleaned Data](https://github.com/chinn1207/MIS-311/raw/refs/heads/main/06_Student%20Perfomance.xlsx)

## 4. Reference
AlexJerabek. (2024). AVERAGE function | Microsoft Support. Microsoft.Com. https://support.microsoft.com/en-us/excel/functions/average-function

AlexJerabek. (2024). Find and remove duplicates | Microsoft Support. Microsoft.Com. https://support.microsoft.com/en-us/excel/find-and-remove-duplicates

Cách sử dụng tính năng Thống kê mô tả (Descriptive Statistics) trong Excel. (2025). In UniTrain. https://unitrain.edu.vn/cach-su-dung-tinh-nang-thong-ke-mo-ta-descriptive-statistics-trong-excel/

Hayes, A. (2024). Descriptive statistics: Definition, overview, types, example. In Investopedia. https://www.investopedia.com/terms/d/descriptive_statistics.asp 

ThomasCoget. (2025). How to Handle Missing Data in Excel A Practical Guide. In Getelyxai.com. ElyxAI. https://getelyxai.com/en/blog/how-to-handle-missing-data 
