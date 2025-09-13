# ETL-Logistic-Regression
Description extract, transform and load data 
# This is the project for enrollies of Hr Analytics:
## This is a company which is active in Big Data and Data Science wants to hire data scientists among people who successfully pass some courses which conduct by the company.Many people signup for their training. Company wants to know which of these candidates are really wants to work for the company after training or looking for a new employment because it helps to reduce the cost and time as well as the quality of training or planning the courses and categorization of candidates.
# Adding data enrollies
## Data source
This company have many data source with different types like google sheet, excel, csv, html, tml, etc. And for each type of data, there are many kind of ways to extract data. 

1/ For data enrollies:
This data is a link google sheet so that I have to use pandas to import data.
The details code is attached in the attachment. After extract, the data needed to be checked, explore to find it is a normal data or not.
<img width="654" height="697" alt="image" src="https://github.com/user-attachments/assets/0bc1d445-447c-4e52-b0b5-58e2932ef522" />

2/ For data enrollies' education and enrollies' working experience
This data is a file excel and csv so in colab, the data need to upload in it.
The result after upload
Enrollies' education: 
<img width="999" height="698" alt="image" src="https://github.com/user-attachments/assets/5d953da3-891e-48a9-9ca9-8292fc9c85cb" />
Enrollies' working experience:
<img width="1132" height="680" alt="image" src="https://github.com/user-attachments/assets/b3f849a5-f343-4790-a0cd-44e35cc6ace0" />

3/ For training hours and employment data
For this type, I need to install pymysql and create_engine to access the database
Result after import data:
Training_hours:
<img width="556" height="576" alt="image" src="https://github.com/user-attachments/assets/2ea1cf96-cad8-4a76-80f9-431db3f589ba" />
Employment:
<img width="519" height="579" alt="image" src="https://github.com/user-attachments/assets/025fcf68-325a-4061-b59c-7d82ac501bba" />

4/ For city development index data
The code should be use: 
tables = pd.read_html('link')
Result after import:
<img width="453" height="324" alt="image" src="https://github.com/user-attachments/assets/3c867250-fd9a-46cb-aa62-1c16139625ac" />

## ETL data
After import data, there are some database have missing value and some types of some collumns is not right and need to excecute and repair.
Some database need to transform data like enrollies, enrollies' education and enrollies' working experience. 
I need to change type object into suitable type like string, category, etc. Moreover, the database is missing value so I need to create new categories unknown and add in Na value. Finalize, I excecute standarlize value to make the data standard and easy to use.
All of code which transformed data in this link: https://colab.research.google.com/drive/1KKIQHymW9KTj4ZTdFBIcbuqs3xMseCBb?authuser=0#scrollTo=AlonNbv93Olu
