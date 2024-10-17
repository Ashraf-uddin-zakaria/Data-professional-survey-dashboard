
# Data professional survey 

### Dashboard Link : https://app.powerbi.com/groups/me/reports/5301f993-227e-43b0-8cad-75dcd07fe678/47e3e33ca26850d9b248?experience=power-bi

## Problem Statement

This dashboard helps the company understand their employee better. It helps the company to know if their employee are satisfied with their policies. Through different ratings, they get to know their improvement area, & thus they can improve their services by identifying these area.



### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : Removed some columns like 'Browser', 'OS' which only caontains Null values.

![Null column removed](https://github.com/user-attachments/assets/6a68993d-d0ad-4ef7-a015-abd961a1d600)
- Step 5 : Data cleaning: Noticed there are many subcategories under 'Other' options; added all the subcategories in one option, 'Other'.

![Other Issues](https://github.com/user-attachments/assets/d6de7e70-fb89-4e29-b8b9-2aa820ab0f2a)

added all the subcategories in one option, 'Other'.

![Other 2](https://github.com/user-attachments/assets/eae70c6f-803e-4f09-a829-1406abd995a4)

- Step 6 : Salary was range data and was in text format, e.g., 150k-200k, therefore calculated average data for salary column (Average_salary)
![Salary](https://github.com/user-attachments/assets/dde255dc-f36b-46d1-9724-889cf6be20c3)

for creating new column following DAX expression was written:

= Table.AddColumn(#"Changed Type7", "Average_salary", each ([#"Q3 - Current Yearly Salary (in USD).1"]+[#"Q3 - Current Yearly Salary (in USD).2"])/2)

![Average salary](https://github.com/user-attachments/assets/88e124c7-bce0-457f-bfc0-3caacc3d8087)

- Step 7 : Card visual was used to represent number of people participate in the survey and average age

![Card visual1](https://github.com/user-attachments/assets/9be41cc0-e311-4591-bb9e-8ee3927fdfd3)

- Step 8 : A stacked bar chart was added to show the average wage per job title for survey respondents.

![Job title salary](https://github.com/user-attachments/assets/9c696c9e-3e7e-45ab-b529-be5c471afc13)

- Step 9 : Donut chart used to represent the count of gender
![Gender](https://github.com/user-attachments/assets/7a9ca71d-fa7d-4614-b327-3d0247b191db)

- Step 10 : Stacked column chart representing the favorite programming languages of data professionals

![Fvr language](https://github.com/user-attachments/assets/f70818a6-2361-4a48-a7c2-ba9a242f5fe6)

- Step 11 : Gauge chart showing how much happy and satisfied employees are with management, their work-life balance, and salary 

![Gauge](https://github.com/user-attachments/assets/8b16aa97-f316-4e4d-9b84-ce3bb224d2d1)


 
 - Step 12 : The report was then published to Power BI Service.
 
 

# Snapshot of Dashboard (Power BI Service)

![PowerBIapp](https://github.com/user-attachments/assets/814af2ef-0e46-44ae-a246-62b28c8e1c53)

 
 # Report Snapshot (Power BI DESKTOP)

 
![PB DEsktop](https://github.com/user-attachments/assets/7d64faa6-8a4b-4dc6-8dd5-22ccac3995aa)



