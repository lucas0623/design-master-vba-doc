---
draft: false
---
## 1	Export Data from GSA
1. In the explorer tab, Go to `Output`,  click any output view. A output window will pop up. 
2. Then, right click on the window, and choose `Output Setting`. ![[Pasted image 20241230133901.png]]
3. In the `Output Setting Wizard`, check the following tables:
	- Nodes - Nodes
	- Nodes - Supports
	- Elements - Elements
	- Beam and Spring Element Results - Beam and Spring Forces and Moments.
4. Check `Output Table` option. Uncheck `Output Summary` option.
5. Go to `Further Option`, check `Fully populate fields`
6. Input your own case list/ node list and elements list. However, **remember to include all the nodes that connected to your element. The node list is hence recommended to always set as 'All'**![[{71F17577-D6C3-4495-A6C8-72555E59C199}.png]]
7. Click `OK` and the output table will be rendered. Then click `Output>Export Output (CSV or TSV file)`. Save the csv table that contains the selected output data in your designated location.
8. You can save the output view by `right click > save output view`, so that you can directly call out the same output for export directly without navigating through all settings.
## 2	Import Data to Workbook
1. Go to the workbook, `Design Master Tab > Import Data > Import GSA Output (Existing Data will be DELETED)`. A file selection box will pop up. Select the .csv data file you saved previously.
2. When success, a message box will pop up notifying you about the operation completed.![[{49D1FAE2-2963-4AE7-818E-41712617A563}.png]]
## 3	Viewing Import Data
The imported data are stored in the `Data_Joint, Data_Frame and Data_FrameForce` sheets. These sheets are hidden by default, and can be unhide by `right click at the sheet tab > unhide`
## 4	Q&A
- What version of GSA does it support?
	- The import functions currently work for both GSA 10.1 and 10.2. Update of the add-in might be required in the future if the data format in GSA is changed.
- Difference between `Import GSA Output (Existing Data will be DELETED)` and `Import GSA Data`.
	- The `Import GSA Output` option will NOT delete the existing data in the workbook. The imported data will be added to the workbook. **It is assumed that there is no frame name/ joint name conflict between the original data in the workbook, and the imported data, or otherwise error or unpredictable result may occur**
	- Hence, in most of the situation, `Import GSA Output (Existing Data will be DELETED)` is recommended.