# Data documentation
## Objectives
- Notes
- Differentiate lab notebooks, codebooks, and readme files
- tech is changing quickly, e.g. DNA sequencing, and new analyses coming quickly, good documentation is important

## Introduction
Plan management -> **Collect and store**  -> Assure quality -> **Analyze and present** -> **Share and preserve**

In this module, we'll focus on documenting important parts of your workflow to help you later write your thesis or dissertation, and to also make sure you can share your data later.

## What to document
Data Documentation
Why document data?

Clear and detailed documentation is essential for data to be understood, interpreted, and used. Data documentation describes the content, formats, and internal relationships of your data in detail and will enable other researchers to find, use and properly cite your data.

Begin to document your data at the very beginning of your research project and continue throughout the project. Doing so will make the process much easier. If you have to construct the documentation at the end of the project, the process will be painful and important details will have been lost or forgotten. Don't wait to document your data!

Professor John MacInnes, University of Edinburgh, speaks to documenting data when analyzing it [youtube](https://www.youtube.com/watch?v=EIZsxT-fIiQ)

What to document?

Research Project Documentation

Rationale and context for data collection
Data collection methods
Structure and organization of data files
Data sources used (see citing data)
Data validation and quality assurance
Transformations of data from the raw data through analysis
Information on confidentiality, access & use conditions
Dataset documentation

Variable names and descriptions
Explanation of codes and classification schemes used
Algorithms used to transform data (may include computer code)
File format and software (including version) used

From: DMPTool "Data Management General Guidance" [website](https://dmptool.org/dm_guidance)



"You may be on intimate terms with your dataset while you are collecting and analysing it, but remembering that the variable "sglmemgp" means single member of group, or the exact procedure you used to transform or derive particular variables, could potentially become difficult months or years later." 

Project level: what the study set out to do, how it contributes new knowledge to the field, what the research questions/hypotheses were, what methodologies were used, what sampling frames were used, what instruments and measures were used, etc. A complete academic thesis normally contains this information in detail, but a published article may not. If a dataset is shared, a detailed technical report will need to be included for the user to understand how the data were collected and processed. You should also provide a sample bibliographic citation to indicate how you would like secondary users of your data to cite it in any publications, etc.

File or database level: how all the files (or tables in a database) that make up the dataset relate to each other; what format they are in; whether they supercede or are superceded by previous files. A readme.txt file is the classic way of accounting for all the files and folders in a project.

Variable or item level: the key to understanding research results is knowing exactly how an object of analysis came about. Not just, for example, a variable name at the top of a spreadsheet file, but the full label explaining the meaning of that variable in terms of how it was operationalised.

From: MANTRA "Documentation, metadata, citation" [module](http://mantra.edina.ac.uk/documentation_metadata_citation/)






Maintining documentation as you go along will save you having to try and think back about your procedures, ad hoc decisions you had to make while gathering your data, and the processing you did to transform and analyze raw data. Key elements to keep track of include:

Maintain dataset provenance
- Where did the data come from? Did you collect it, or did you get your data form another source?
- 



Document transformations
Beware of accidental duplication

Review metadata for compatibility of context, methods, and meaning
For what purpose was the data collected?
How was the data collected?
Is it sensible to combine these datasets?


Ensure compatibility
Convert to common units
Choose appropriate numeric precision
Evaluate and standardize missing value codes

Document all assumptions
What assumptions underlie the original datasets?
What assumptions did you make in combining the datasets?


Recognize that you are creating a new dataset
Revisit the data life cycle to ensure the new dataset is properly documented, validated, and preserved

Use reproducible workflows
Enable transparency and reproducibility in the integration process
Ensure others understand and can evaluate your decision making process.
Automate the integration as much as possible
Especially when integrating many datasets or large datasets


## Tools for documentation

laboratory notebooks & experimental protocols

questionnaires, codebooks, data dictionaries

software syntax and output files

information about equipment settings & instrument calibration

database schema

methodology reports

provenance information about sources of derived or digitised data

From: MANTRA "Documentation, metadata, citation" [module](http://mantra.edina.ac.uk/documentation_metadata_citation/)

## Lab notebooks
Why?
For laboratory researchers, laboratory notebooks are crucial components of data management. 

They can play an important role in supporting claims relating to intellectual property developed by University researchers, and even defending claims of scientific fraud. 

In less extreme circumstances, they demonstrate adherence to standards of good practice, academic and ethical integrity, and compliance with contractual provisions permitting sponsors to audit work carried out in pursuit of sponsored-research. 

Therefore, thorough and effective management of laboratory data and the routine documentation of all lab procedures is a highly important responsibility for all laboratory researchers.
From: MANTRA "Documentation, metadata, citation" [module](http://mantra.edina.ac.uk/documentation_metadata_citation/)

- To provide yourself with a record of how your data were collected, organized and processed. Yes, you will forget if you don’t write it down.
- To provide yourself with a central & physical location for protocols, results, and general happenings.
- To encourage a thoughtful process. The act of writing things out forces you to explore and clarify ideas.
- To enable continuity in the face of unexpected events.
- To establish a legal and scientific provenance (historical record) of your work

How? 
Analog

- A notebook
	 - stitched binding that lays flat when open
	 - larger size is generally better
	 - better quality paper is worth it
	 - pre-numbered pages are also worth it. 

-  are hugely variable and often discipline-specific. Do your homework if you want to go that route.

Digital

- Electronic notebooks (ELNs)
- Computer and Mobile Software
	- Evernote
- Computer files in a directory

What?

- Date each entry
	- Include the year
- Include the full names and contact information for all collaborators
	- Identify who did what in your notes
- Take notes on meetings and discussions about the experimental or research goals
	- Write the names of people who assisted you, for future acknowledgement.
- Provide justifications for method, source of data (how did they generate the data?).
- Protocols for experiments or for acquiring data (if using 2ndary data). 
	- Tape in printed versions.
- Capture field, laboratory, or interview conditions.
	- Use military time, or AM/PM
	- Provide full details on experimental/research organisms/subjects.
	- If performing lab experiments w/reagents, list details like manufacturer, batch, etc.
	- Record equipment details. 
- Images can help with documentation: 
	- Take photos or make quick drawings set-ups, locations, etc.
- Annotate all calculations
- If data are logged or added on a computer, record file names of data
	- Include where they are stored and backed up
- Describe the locations of all physical materials: data binders, seeds, samples, etc..
- If helpful to see them on paper, print and attached graphs, data sheets, photographs, etc.
	- Use glue to cleanly and permanently attach all edges
- Detail your mistakes.
- At the conclusion of your experiment, write or print out a full directory of all electronic files that relate to your experiment.
- Typically, a phycial laboratory notebook stays in the laboratory where the experiments were conducted.

### Analog to digital transfer
scanning and OCR

- ScannerPro
- Evernote
- NVAlt

## README files
## Codebooks

## References
- DataONE. "Data entry and manipulation" [modules](https://www.dataone.org/education-modules)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Purrington, C.B. Maintaining a laboratory notebook http://colinpurrington.com/tips/academic/labnotebooks.