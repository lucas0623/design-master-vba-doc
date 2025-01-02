---
title: Customizing Summary Sheet
draft: false
---

## 1	Introduction
A *Summary Sheet* is mainly used by 2 processes:
- When extract result from the imported data. See [[../05 - Extract Frame Force/Extract Frame Force to Summary Table]].
- When transferring the data to design spreadsheet. See [[../07 - Summary To Design/Transferring Data From Summary to Design Worksheet]].
Hence, understanding the behaviour of these 2 processes will help you understanding how to building up the *Summary Sheet*. Also, it is important to understanding the [[../01 - Introduction/05 Tag System|Tag System]] that is used to locate the data for all processes in the add-in.
## 2	Structure of Summary Sheet
- 'rRow' tag.
- 'targetWS' tag.
- System tag for Data Extraction Process.
- Any other customized tags for Summary to Design Process.
![[../../../Z_System/Attachment/Pasted image 20250102134643.png]]
## 3	Custom Tag
The tags in Summary Sheet can be grouped into 3 categories:

1.    System Tag (Necessary). These tags must be present in a summary sheet for data extraction and ‘Transfer Data to Design Worksheet’, which are listed below:

a.    rRow. Must be at the first column of the sheet. Apply for all operation.


b.    targetWS. Necessary for ‘Put Data to Design Worksheet’ operation. Must be located at the first row of the Summary sheet.

2.    System Tag (Optional). These tags are used in ‘Extract Force’ Operations. User may keep/remove these tags according his/her needs.

3.    User Defined Tag (Optional). These tags are used in ‘Put Data to Design Worksheet’, which are most likely the design input of Design Spreadsheet. The tag shall match with the registered tag in ‘WsData’.

User may view the condition & name of these tag in **Design Master>View tag ….**.

Error may occur if there are tag’s name changed/ tag deleted, or they are not in the first row/first column of the sheet.

Hence, there are 2 points we can notice:
- Insert/ moving column of a worksheet would not affect the macro functionality in principle.
- 