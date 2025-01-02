---
draft: false
---
## 1	Code Logic
1. Read all data in the summary table
2. Read all data in `WSData` and `DesignWsGroupData`
3. Locate the column with `targetWS` input, and loop for each row selected.
	1. If the specified name in the `targetWS` column of the row matched any *Design Worksheet Group* specified in `DesignWsGroupData`, the data of the row will be transferred and calculated based on the specified *Design Worksheet Group*. 
	2. If the specified name in the `targetWS` column of the row matched any *Design Worksheet* specified in `WSData`, the data of the row will be transferred and calculated based on the specified *Design Worksheet*.
### 1.1	Data Transferring Process Based on *Design Worksheet* in `WSData`
The data transferring process is summarized below:
1. For each *Design Worksheet* Input
	1. Matching the Input tag to the first row of  the *Summary Sheet*
	2. Transfer the data to the design worksheet 
2. Calculate the sheet.
3. Return data from the *Design Worksheet* to *Summary Sheet*. Similar logic to the input.
![[Pasted image 20250102104721.png]]
### 1.2	Data Transferring Process Based on *Design Worksheet Group* in `DesignWsGroupData`
The data transferring process in *Design Worksheet Group* is similar to *Design Worksheet*. The process is summarized below:
1. For each *Design Worksheet* in *Design Worksheet Group* 
	1. For each input in the *Design Worksheet*
		1. For default input = true --> input specified default input value to the cell.
		2. For default input = false 
			1. Matching the Input tag to the first row of  the *Summary Sheet* according to the input in `DesignWsGroupData`
			2. Transfer the data to the design worksheet 
	2. Calculate the sheet.
	3. Return data from the *Design Worksheet* to *Summary Sheet*. Similar logic to the input.
**It is noted that only 1 design worksheet will be updated in a single calculation (instead of calculation of whole workbook). If your design worksheet requires input from other worksheet, please be careful and check if the worksheet's calculation is performed correctly.**
## 2	Limitation of Design Worksheet
1. Cannot deal with the design worksheet that is powered by excel macro. It is suggested to use excel lambda function instead, which should be able to complete most of the engineering calculation.
2. The design worksheet shall be a single worksheet. It is suggested to avoid worksheet input referencing the calculation of other worksheet (but look up of static data from other worksheet is ok, e.g. look up properties from steel section table).
## 3	Review Matched Tag in Summary Sheet
You can use `Design Master Tab > View Tag of Design Worksheets` to check if the tags in the *Summary Sheet* matched the *Design Worksheet* Input and Output
![[{C8CB3610-6F34-4324-97F3-2723D677DA75}.png]]