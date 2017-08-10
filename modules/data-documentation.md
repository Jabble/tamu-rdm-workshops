# Data documentation
## Objectives
- Identify relevant project-level and data-level documentation.
- Recognize the purpose of documentation tools such as lab notebooks, codebooks, and readme files.

## Introduction
Plan management -> **Collect and store**  -> Assure quality -> Analyze and present -> Share and preserve

In this module, we'll focus on documenting important parts of your workflow to help you share information about your project with your advisor, write your thesis or dissertation, and to ensure your data are useful later.

## Why document 
"You may be on intimate terms with your dataset while you are collecting and analysing it, but remembering that the variable "sglmemgp" means single member of group, or the exact procedure you used to transform or derive particular variables, could potentially become difficult months or years later." 

Clear and detailed documentation is essential for data to be understood, interpreted, and used. Documenting your data from the beginning of research projects, will make your research career easier.

It will enable:

- You to get a mess of details out of your head, so that you can focus on doing your work and avoid forgetting important considerations.
- You can reproduce and improve workflows in the future.
- Other researchers, including your collaborators, can find the right data and use them properly.

## What to document
Documentation can be used to describe your research projects at different levels. High-level documentation explains your research goals and the progress of your project. Low-level documentation explains the details of the data, how it has been collected, stored, and changed over time.

Project documentation explains:

- Rationale and context for data collection
- Research questions/hypotheses
- Data sources, collection methodology, protocols
- Data validation and quality assurance actions
- Transformation of raw or derived data for integration or analysis
- Data confidentiality, access, and use conditions

Dataset documentation explains:

- Variable names and descriptions
- Codes and classification schemes
- Algorithms used to transform data 
- Structure and organization of files
- Relationship among data files or tables in a database schema
	- Version information
- File formats and software used

## Video: documenting data during secondary analysis
Professor John MacInnes, University of Edinburgh, speaks to the value of documention during data analysis [youtube](https://www.youtube.com/watch?v=EIZsxT-fIiQ)

## How to document
- Laboratory notebooks
- Codebooks and data dictionaries
- README and log files

### Exercise
- Have you used one of these forms or documentation?
	- If so, can you describe it, what did it contain?
	- If not, choose one of the above. What information do you think it should include?

### Notebooks and note files
For projects including observational and experimental data sources, lab and field notebooks are crucial components of data management. However, notebooks are also helpful to save project-level documentation when working with data from other sources.

- Provide a central and physical location for protocols, results, and happenings. You have one place to go.
- Encourage a thoughtful process. The act of writing forces you to explore and clarify ideas.
- Enable continuity in the face of unexpected events or time passing. Yes, you will forget if you don’t write it down.
- Provide a record of how your data were collected, organized, and processed. Establishing a legal and scientific provenance (historical record) of your work.

Physical notebook (analog)
**Bring a good example**

- stitched binding that lays flat when open
- larger size is generally better
- better quality paper and pre-numbered pages are worth it

Digital notes

- Electronic notebooks (ELNs)
- Computer and Mobile Software
	- Evernote
- Text files saved in a directory

Good practices: 

- Date each entry
	- Include the year
- List the full names and contact information for all collaborators
	- Identify who did what
- Take notes on meetings and discussions about the research
	- Write the names of people who assisted you for future acknowledgement
- Provide justifications for the method and data source(s)
	- Details about where and who derived or digitized data come from
- Include protocols for experiments or data acquisition
- Capture conditions in the field, laboratory, or interview 
	- Include the time, using military time or include AM/PM
	- Note details on experimental/research organisms/subjects
	- List details like manufacturer, batch, etc. for purchased material
	- Record equipment details such as settings and instrument calibration
- Note mistakes in detail and what needed to be fixed
- Use images to simplify documentation
	- Take photos or make quick drawings of set-ups, locations, etc.
- Annotate all calculations and include units
- If data are logged or added on a computer, record file names of data
	- Include where they are stored and backed up
- Describe the locations of physical materials: data binders, seeds, samples, etc.

### Tools for analog to digital transfer
- ScannerPro: scanning and OCR
- Evernote: Photos and notes

### README and log files

Coopted for data management from software code. Readme files can serve a similar purpose as notebooks, but are primarily aimed at an external audience and your future-self rather than ongoing note-taking. 

They may be less concerned with project-level documentation and more with the documenting the dataset and data element level. 

A readme.txt file is the classic way of accounting for all the files and folders in a project. Common in software. Logs can be used to automatically report actions taken by a software.

Recommended content
Recommended minimum content for data re-use is in bold.

General information

Provide a title for the dataset
Name/institution/address/email information for
Principal investigator (or person responsible for collecting the data)
Associate or co-investigators
Contact person for questions
Date of data collection (can be a single date, or a range)
Information about geographic location of data collection
Keywords used to describe the data topic
Language information
Information about funding sources that supported the collection of the data
Data and file overview

For each filename, a short description of what data it contains
Format of the file if not obvious from the file name
If the data set includes multiple files that relate to one another, the relationship between the files or a description of the file structure that holds them (possible terminology might include "dataset" or "study" or "data package")
Date that the file was created
Date(s) that the file(s) was updated (versioned) and the nature of the update(s), if applicable
Information about related data collected but that is not in the described dataset
Sharing and access information

Licenses or restrictions placed on the data
Links to publications that cite or use the data
Links to other publicly accessible locations of the data
Recommended citation for the data
Methodological information

Description of methods for data collection or generation (include links or references to publications or other documentation containing experimental design or protocols used)
Description of methods used for data processing (describe how the data were generated from the raw or collected data)
Any instrument-specific information needed to understand or interpret the data
Standards and calibration information, if appropriate
Describe any quality-assurance procedures performed on the data
Definitions of codes or symbols used to note or characterize low quality/questionable/outliers that people should be aware of
People involved with sample collection, processing, analysis and/or submission
Data-specific information

*Repeat this section as needed for each dataset (or file, as appropriate)*

Count of number of variables, and number of cases or rows
Variable list, including full names and definitions (spell out abbreviated words) of column headings for tabular data
Units of measurement
Definitions for codes or symbols used to record missing data
Specialized formats or other abbreviations used

- Cornell University, Research Data Management Services Group. "Guide to writing "readme" style metadata" [webpage](https://data.research.cornell.edu/content/readme)

I strongly recommend that you use a README.txt file at the top level of your project folder to explain the purpose of the project, the relevant summary and contact details, and general organization of your files. This is equivalent to using the first page of your laboratory notebook to give a general description of your project.

Top-level and low level readmes

- Data Ab Initio. [blog](http://dataabinitio.com/?p=378)


### Codebooks

So what is a data dictionary? A data dictionary is something that describes the data in a dataset. Generally, a data dictionary includes an overall description of the data along with more detailed descriptions of each variable, such as:

Variable name
Variable meaning
Variable units
Variable format
Variable coding values and meanings
Known issues with the data (systematic errors, missing values, etc.)
Relationship to other variables
Null value indicator and missing value codes
Anything else someone needs to know to better understand the data
This list represents the types of things you would want to know when faced with an unknown dataset. Not only is such information incredibly useful if you’re sharing a dataset, but it’s also useful if you plan to reuse a dataset in the future or you are working with a very large dataset. Basically, if there’s a chance you won’t remember the details or never knew them in the first place, a data dictionary is needed.


Can be contained in a readme doc, a seperate file, or as  part of a data spreadsheet. seperate thing.
Use example from blog
- Data Ab Initio. [blog](http://dataabinitio.com/?p=454)


A codebook is similar to a readme file, and describes the contents, structure, and layout of a data collection. A well-documented codebook "contains information intended to be complete and self-explanatory for each variable in a data file.
Creating a codebook [PDF](http://ccjr.csusb.edu/docs/researchmanualdocs/creatingacodebook.pdf)
From: [website](http://www.icpsr.umich.edu/icpsrweb/NAHDAP/support/faqs/2006/01/what-is-codebook)

## References
- DataONE. "Data entry and manipulation" [modules](https://www.dataone.org/education-modules)
- DMPTool. "Data Management General Guidance" [website](https://dmptool.org/dm_guidance)
- MANTRA. "Documentation, metadata, citation" [module](http://mantra.edina.ac.uk/documentation_metadata_citation/)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Purrington, C.B. Maintaining a laboratory notebook http://colinpurrington.com/tips/academic/labnotebooks.