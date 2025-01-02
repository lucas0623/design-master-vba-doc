---
title: Tag System
draft: false
---
## 1	Locating Data with Tags
In order to provide flexibility and allow customization for different projects/ different design situations/ design of different types of structure, all tables in the Summary Sheet and the Data Sheets are located using the *tag system*. These tags are located in the first row and the first column of the sheets, which each tag represents one type of data/property. The macro will find these tag to locate the data in the worksheets.

For example, in the `Data_joint` sheet, there is a tag ‘rRow’ in the first column. This represents the header row of a table. The first row of data will be rRow + 1, which is row 3 in this example. There are also some tags in the first row of the sheet, which are ‘ID’, ‘x’, ‘y’, ‘z’ and ‘isRestraint’.
![[../../../Z_System/Attachment/Pasted image 20241231101312.png]]
## 2	System Tag
There are 2 different types of tag used in the add-in. The first one is called *system tag*. This is a specified string that is read by the add-in for locating certain data in the worksheet.  These tags are usually saved in the 1st row and 1st column of the worksheet. 

In the above figure, there are *system tag* 'ID', 'x', 'y', 'z' and 'isRestraint' at the 1st row of the worksheet `Data_Joint`. Take 'x' as an example. The add-in will try to look for the string 'x' in the 1st row of the `Data_joint` sheet to locate the x-coordinate of joints. These string cannot be amended unless the source code is changed. 

**It is noticed that all system tags are necessary except  for those in the summary sheet.** Read [[../02 - Setting Up the Workbook/Customizing Summary Sheet]] for more details about optional system tag.
