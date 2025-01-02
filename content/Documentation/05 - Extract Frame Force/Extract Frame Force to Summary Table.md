---
draft: false
---
After data is imported to the workbook, you may extract frame force data with `Design Master Tab > Extract Frame Force to Summary Table > by Correspondence Cases`. A userform will appear which give you a selection of option to process and extract data as per your need. The choice of options will be saved and loaded in the next time automatically for certain summary sheet.
![[../../../quartz/Z_System/Attachment/{4A018596-A4C9-427F-BB88-9E23F5B07744}.png]]
## 1	Description of Each Parameter
Filters - to filter certain properties
- Section Filter
- Member Filter
- Load Combination Filter
- Position Filter

Grouping Output Data
- By section or Member
- Each load combination or not
- Each position or not

Correspondence Cases Control
- Correspondence case - To locate frame forces using certain extreme value, and return the frame forces at the position of a frame under certain load combination that the extreme value located.
- Create permutation from envelope load combinations - for envelop load combinations, the frame forces are output as a Max and a Min value. when this option is checked, both Max and Min value will be taken into account, and create permutations of frame forces if not considering the absolute maximum value.

## 2	Code Logic
The code logic can the simplified in the following steps:
1. Read all imported frame forces data
2. Apply section, member and load combination filters
3. Group frame forces by  
	1. 'Group output by member/ section' option
	2. 'Output result separately for each load combination' option
	3. 'Output result separately for each position' option
4. For each group of frame forces, extract the frame forces by:
	1. For each selected correspondence cases
		1. Find the extreme value of the case.
		2. Create permutation(s) according to user option (apply when envelop load combination that have 2 frame forces data for an frame element at certain location). Suggest to uncheck this option only when you want to plot graph (e.g. BMD) or the load combinations are not envelope load combination.
		3. Is consider absolute maximum - for envelope load combination, the direction of the forces and moments may not be important in design (e.g. shear force, moment for symmetric section). In such cases, checking the box(es) so that the Add-in will consider the absolute maximum of the checked forces/moments. For unchecked forces/moments, permutations will be created to ensure all possibilities.
## 3	Suggest Extraction Setting
Below are some suggested frame extraction setting under different situations for reference.
- Steel Member Design (Preliminary) 
	- By section
	- ![[../../../quartz/Z_System/Attachment/{5E318AF5-F723-4B6B-9C4A-CA3728FEBD0A}.png]]
- Steel Member Design (Detail) - Design for each element at all positions.
	- By Member (WITHOUT identified member using `process model data`). ![[../../../quartz/Z_System/Attachment/{B171415B-D729-4EEA-9D63-CE6255451401} 1.png]]
- Pile Design - 
	- By Member (WITHOUT identified member using `process model data`) 
	- Design for each pile ![[../../../quartz/Z_System/Attachment/{BE281E6C-27C8-4A35-98AF-BAD95995E1D8}.png]]
- RC Beam Design
	- Calculation at each position
	- Direction of moment is important.
	- By member (with identified member) ![[../../../quartz/Z_System/Attachment/{AFC36256-3CBC-4895-8672-5F077792B6CE}.png]]
- Plotting BMD Diagram
	- extract Max and Min value seperately
	- Can be multiple load combinations if only plotting for BMD
	- Uncheck 'create permutation'
	- By Member (with Identified member) ![[../../../quartz/Z_System/Attachment/{FDEE6449-1728-403F-93C4-CC6E8A2608C3}.png]]