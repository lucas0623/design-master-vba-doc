---
title: Overview
draft: true
---

## 1	Release
v4.1.4
- Update frame force extraction logic and performance
	- position filter added
	- option for each position
	- option for create permutation or not
- Remove the 2 extract frame force methods
	- Extract frame force by position of member
	- All forces along member
- remove the feature 'Import Design Worksheet'
v4.1.3
- Improved performance of initialization of Summary to Design.
- Fixed the bug in initialization of userform for Extract Frame Force
v4.1.2
- Fixed the issue of SummaryToiDesign crashing when Design worksheets name specified in 'DesignWsGroupData' does not exist
- Added 'Application.FormatStaleValue=False' in SummaryToDesign
- Added module to review speed of design worksheet
- Added timer for summary to design
v4.1.1
- Fixed the issue of setting up workbook
- Add support of import GSA v10.2 result
- ExtractFrameCo: Now can apply position filter (End I only, End J Only, Both Ends Only or No Filter)
- 
v4.1.0 
- Added description in log file.
- Added support for design worksheet group
- Added verification of cell address of design input/output in 'WSData'
- Fixed the issue when the output cell is in Error.

v4.0.3 
- Fix the bug when the first row in WSData used 'merge cell'
- Support import and force extraction for Link Element
- Rewrite the function 'FindLastNonEmptyColumn'.
- Fixed the bug when the last column in a datasheet is empty.
- Fixed the bug that appears when the matched joint in the connection type is empty.
v4.0.2
- TransferDataFromSummary
	- Added verification of target WS. Warning will be logged if there is missing worksheet in 'WSData'
v4.0.1
- Fixed incorrect version
- Now will check and initialize the 'system' sheet automatically for all macros.
- SummaryToDesign now can work without the full setup of workbook
- Handle the error appears when the log file did not close properly.
- Fixed bug for displaying log file.
- Fixed bug for importing datafile from SAP2000
- Fixed bug for extracting correspondence load cases in SAP
- CreateNewSummary: now added 'rRow' tag
- Resolve the bug when initializing the userform of ForceExtraction - load last saved data inappropriately
- Resolve the bug of wrong initilization of userform of ConnForceExtraction
v4.0.0
- Beta version. First release as an addin in .xlam format.




