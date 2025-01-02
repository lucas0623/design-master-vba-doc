---
draft: false
---
## 1	Export Data from SAP2000
1. In SAP2000, select the elements **and nodes** that you would like too design
2. `Display > Show Table` or use hot key `Ctrl + T` 
3. Check the following tables:
	- Connectivity Data - Joints Coordinates
	- Object Connectivity - Frame
	- Object Connectivity - Link (optional)
	- Joint Restraint Assignments
	- Frame Section Assignments
	- Frame Local Axes Assignments (optional)
	- Link Property Assignments (optional)
	- Link Local Axes Assignments (optional)
	- Element Forces - Frame
	- Element Forces - Links (optional)
	![[../../../Z_System/Attachment/{435FDD20-9E1E-44F9-8EE2-C91A1F5828E3} 1.png]]
4. Select load combinations and cases.
5. 6. Consider `Save Named Set` to avoid navigating the selection next time. 
6. Click `OK` and the output table will be rendered. Then click `File > Export All Tables > To Excel`. Save the excel table that contains the selected output data in your designated location.![[../../../Z_System/Attachment/{BE6EB5C5-881A-4E69-9C6E-2B784BD1C03E}.png]]
## 2	Import Data to Workbook
1. Go to the workbook, `Design Master Tab > Import Data > Import SAP2000 Output (Existing Data will be DELETED)`. A file selection box will pop up. Select the .xlsx data file you saved previously. This option will cleared all previously imported data and import the data from the selected file. 
2. When success, a message box will pop up notifying you about the operation completed.![[../../../Z_System/Attachment/{49D1FAE2-2963-4AE7-818E-41712617A563}.png]]
## 3	Viewing Import Data
The imported data are stored in the `Data_Joint, Data_Frame and Data_FrameForce` sheets. These sheets are hidden by default, and can be unhide by `right click at the sheet tab > unhide`
## 4	Q&A
-  What is the difference between `Import SAP2000 Output (Existing Data will be DELETED)`and `Import SAP2000 Data`?
	- The `Import SAP2000 Data` option will NOT delete the existing data in the workbook. The imported data will be added to the workbook. **It is assumed that there is no frame name/ joint name conflict between the original data in the workbook, and the imported data, or otherwise error or unpredictable result may occur**
	- Hence, in most of the situation, `Import SAP2000 Output (Existing Data will be DELETED)` is recommended.
