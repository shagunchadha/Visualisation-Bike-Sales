Bike Sales - Data Cleaning & Analysis (Excel)
Project Overview
This project involves cleaning and analysing a real-world dataset of global bike sales using Microsoft Excel.
The dataset was sourced from Kaggle, inspired by Alex The Analyst's data analysis tutorial series.
Dataset

File: bike_sales.xlsx
Source: Kaggle - Bike Sales Dataset
Tool Used: Microsoft Excel

Project Structure
Bike-Sales-Excel-Project/
├── README.md
├── Bikes_Sales.xlsx

Part 1 - Data Cleaning
Steps Performed:

Created Working Sheet

Duplicated raw data into a working sheet to preserve the original


Removed Duplicates

Found and removed 26 duplicate rows via Data → Remove Duplicates


Standardised Data

Marital Status: M → Married, S → Single
Gender: M → Male, F → Female
Used Find & Replace with Search by Column to avoid overwriting values in other columns


Formatted Currency

Reduced decimal places on Income column for cleaner readability


Created Age Brackets Column

Added new column using nested IF formula:

excel   =IF(L2>54,"Old",IF(L2>=31,"Middle Age",IF(L2<31,"Adolescent","Invalid")))

Adolescent = Under 31
Middle Age = 31–54
Old = 55 and above


Part 2 - Pivot Tables & Dashboard
Pivot Tables Created:

Avg Income by Gender — Average income split by gender and bike purchase (Yes/No)
Customer Commute — Count of purchases by commute distance
Customer Age Bracket — Count of purchases by age group

Dashboard:

Moved all charts to a dedicated Dashboard sheet
Added Slicers for: Marital Status, Region, Education
Slicers connected to all pivot tables for cross-filtering