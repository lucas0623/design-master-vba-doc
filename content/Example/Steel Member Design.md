---
draft: true
---
## 1	Introduction
This tutorial will go through all steps for using Design Master in steel member design, including: -
- Exporting SAP2000 data; 
- Setting up the Design Master workbook; 
- Registering *Design Spreadsheets*; 
- Setting up the *Summary Sheet* from scratch.
- Extracting force data to *Summary Sheet*
- Carry out design calculation and report preparation
## 2	Setting Up the Workbook

### 2.1	From Scratch
The Design Master Add-in requires a number of worksheets to store structural analysis model data and system data. In this section, the process of how to set up the workbook from a new blank workbook.
#### 2.1.1	Setting up the Workbook From a New Workbook
1. Create a new excel workbook.
2. Go to `Design Master` tab, click `Set Up Workbook`.
3. Message box 'Initialization Complete' will pop up and some sheets are added to the workbook. It is noticed that some of the worksheets are hidden in view by default. The detail for each System Worksheet refers [[Design Master - Data Sheet]]![[../../Z_System/Attachment/{1CC5BEFA-8A25-4290-A024-04951A0453D9}.png]]
#### 2.1.2	Register Design Worksheet Input and Output
1. The macro needs to know the input and output address of each design spreadsheet so that it can carry out automated task, i.e., transferring data
#### 2.1.3	Setting up the Summary Worksheet

### 2.2	From Existing Workbook
## 3	Design Process
### 3.1	Exporting Model Data   (from SAP2000)
![[../../Z_System/Attachment/{59EE7CF8-2B16-42A2-A438-03863D5942F0}.png]]
1. Select the elements and nodes that you would like to carry out design checking.![[../../Z_System/Attachment/{41A958AB-3513-4EBB-9466-BE988BA02A13}.png]]
2. Select the following tables. ![[../../Z_System/Attachment/{FB8DDA32-669C-4967-9725-10A593125D0F}.png]]
3. Save all data in an excel .xlsx file.
### 3.2	Import Data to Workbook

### 3.3	Extract Data to Summary
### 3.4	Transfer Data to Summary to Worksheet
#### 3.4.1	Viewing Result of particular worksheet
#### 3.4.2	Export PDF files
#### 3.4.3	Reviewing the Log File
#### 3.4.4	Preparing Report
