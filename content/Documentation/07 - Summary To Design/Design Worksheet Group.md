---
draft: false
---
## 1	Usage
*Design Worksheet Group* provides more advanced control on transferring data from *Summary Sheet* to *Design Worksheet*. **The *Design Worksheet* must be defined in `WSData` before it is used in the *Design Worksheet Group*.** See [[Setting Up Design Worksheet Input and Output]]. There are mainly 3 usages for *Design Worksheet Group*:-
- When multiple design worksheets are required in a calculation, e.g. connection design that required welding checking, baseplate checking and bolt checking. 
- To define the tag relationship between the *tags* in *Design Worksheet* input/output and the *tags* in *Summary Sheet*, e.g. when a design worksheet force input using 'Fx', 'Fy', 'Fz' as tags but the frame forces tags are 'P', 'V2' and 'V3' as default according to element local axis. User may want to map the forces to the design worksheet per their need.
- Allow default input value. When this option is used, the value specified in the *Summary Sheet* will be ignored.

Below shows an example of the *Design Worksheet Group* 'D44'.
![[../../../quartz/Z_System/Attachment/Pasted image 20250102102149.png]]