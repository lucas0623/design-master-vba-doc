---
title: Overview of Design Master Excel Add-in
---
## 1	Introduction
This excel add-in addressed the issue by streamlining the daily design process with calculation using user's excel spreadsheets. It offers tools to expedite data processing, transitioning seamlessly from structural analysis results to the preparation of design reports. This enhanced process is divided into three main functions:- 
1. **Importing structural analysis result data** from structural analysis software (SAP2000 and GSA);
2. **Extracting relevant design data** from the imported information based on user specifications;
3. **Performing bulk design calculations using your own spreadsheets** and exporting the results in PDF format. 

![[Z_System/Attachment/Pasted image 20250102141621.png]]


## 2	Feature
- **Versatile Tool for Diverse Applications.** This add-in is designed to automate repetitive calculations and support the design of a broad spectrum of structural elements across various structural analysis software platforms.

- **Comprehensive Force Extraction Methods.** Users can extract forces using multiple methods tailored to the specific requirements of different projects and structural elements.

- **Simple Automation Setup**. Easily configure the automation process with your own design spreadsheets and summary tables in just a few minutes. 

- **User-Friendly Interface**. All macros are triggered by buttons on the ribbon and Userform is provided to meet your needs without requiring any coding expertise.

- **High performance**. Capable of completing up to 50 calculations per second, ensuring rapid results.  

- **Open sourced**. The add-in's code is open for review, allowing anyone to examine the macro's underlying logic.

## 3	Application Areas
- Steel member and connection design
- Extract useful loading from models
- RC design
- Whenever repetitive calculation is required.

## 4	Advantages of Using the Add-in
- **Time Saving in Design**. Allowing for quick and comprehensive design process. 
- **Streamlined team workflow**. Enable the entire team to adopt the same tool for a wide range of design tasks, reducing the time required for training and familiarization of new tools.
- **Spreadsheet Reusability**. Utilize template spreadsheets within the workbook to simplify updates and maintenance.

## 5	To Start With...
- Go to [[Documentation/01 - Introduction/Installation|Installation]] to check out how to install the add-in.
- [[Documentation/01 - Introduction/Overview of Data Flow|Overview of Data Flow]] gives an overview of how data is transferred and processed with the add-in from structural analysis result to design report preparations.
- Check out a tutorial in [[Example/Steel Member Design (GSA)|Steel Member Design (GSA)]] to understand the workflow.
- Read [[Documentation/02 - Setting Up the Workbook/Setting up the Workbook|Setting up the Workbook]] to understand more about how to create your own worksheet for design automation.
- [[Documentation/03 - Import Data/Import Data from SAP2000|Import Data from SAP2000]] or [[Documentation/03 - Import Data/Import Data from GSA|Import Data from GSA]] to learn about how to import structural analysis data to the workbook.
- [[Documentation/05 - Extract Frame Force/Extract Frame Force to Summary Table|Extract Frame Force to Summary Table]] to learn more about how to extract useful data to your summary sheet after importing data into the workbook.
- [[Documentation/07 - Summary To Design/Transferring Data From Summary to Design Worksheet|Transferring Data From Summary to Design Worksheet]] to learn about how to do bulk design automatically using your own design spreadsheet with the add-in.