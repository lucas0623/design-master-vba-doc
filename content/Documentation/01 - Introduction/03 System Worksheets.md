---
title: System Worksheets
draft: false
---
The workbook contains the following components:
1. **Data Sheets**. These sheets contain all imported data and processed data. They are named in ‘Data_xxx’ and are hidden by default. In general, the user does not need to unhide these sheets throughout the process unless he/she wants to view these source data.  Sheets include:
	- `Data_Joint` - contains data for imported joint coordinates
	- `Data_JointConn` - contains data for a joint connectivity. It is used for connection mapping.
	- `Data_Frame` - contains frame connectivity data
	- `Data_FrameForce` - contains frame force data
	- `Data_MemberList` - contains member data. 
	- `Data_System` - contains all data used in the add-in

 2. `WSData`. This is a data sheet that contains the input and output location data of a design worksheet. In other words, user may register his/her own Design Worksheet through filling in the input/output location data to this ‘WsData’ sheet.
 3. `DesignWsGroupData`. This is a data sheet to define a design worksheet group. See [[../07 - Summary To Design/Design Worksheet Group]] for more information.
 4. `Define_ConnectionType`. For connection design only. This is used to define the connection types and control the force extraction behaviour for connection design. User may omit this sheet for other design.
 5. **Summary sheets.** They are named in ‘Summary_xxx’. These sheets serve as the link between the imported data from the structural analysis model and the design worksheet. The data in this sheet is located and managed by the ‘Tag System’. There can be any number of Summary sheet in a Workbook. Most of the operations (Extract forces and transfer data to Design Worksheet) are related to the summary sheets.
 6. **Design Worksheet –** this refers to any typical design worksheet we used in our daily design work. The template DM Workbook does not contain any design worksheet. The user shall import their own design worksheet according to their need.

The below figure outlined the data flow of the add-in, and how the data are processed and handled by the macro in different worksheets.
![[../../../quartz/Z_System/Attachment/{2B4544C3-45D9-49E2-A1B2-8F35A05D9092}.png]]
![[../../../quartz/Z_System/Attachment/Pasted image 20241230110707.png]]