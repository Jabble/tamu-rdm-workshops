# File organization
## Objectives
- Recognize the purpose of file naming conventions.
- Explain the components of sensible file names.
- Compare and critique file naming conventions.

## Introduction
Plan management -> **Collect and store**  -> Assure quality -> Analyze and present -> Share and preserve

In this module, we'll look at organizing data with accessibility in mind. The goal is for you to be aware of organizational strategies that can help you focus on working with your data, rather than trying to find files. 

Professor Jeff Haywood at the University of Edinburgh on the importance of good file management [youtube](https://www.youtube.com/watch?v=i2jcOJOFUZg)

### Exercise: Current practices?
*Pair and share activity*
Do you already have your own way of naming files?
Does your research lab or group already have a file naming convention?
Does it have an organizational strucutre for folders?
What's in a name?
Describe?

## Naming conventions
Without structured information, our lives would be much poorer.  Naming files and directories sensible things is good for you and for your computers. So, we're going to talk about what are "sensible" names. 

First, I need to note. There's one necessary condition for a naming convention to succeed, and for an organized scheme to develop. 

**Be consistent.** 

Choose a naming convention and ensure that the rules are followed systematically by always including the **same information** in the **same order**. This is one of those things to think about a little in advance, set (make a habit), and more or less forget.

Have conventions for your:

1. Directory structure
2. Folder names
3. File names

## What's in a name?
Let's start at the low level. What ought to go into a file name? "sensible things." Well, these will depend on your project and expected use. 

Generally, descriptive information that will help you identify the content you seek when browsing, sorting, and/or searching, especially in the case when additional context is lost or missing.

When constructing files, the following components are "sensible things." Use them alone or in a combination that suits your needs.

|informational component | possible use | tip |
|----------|----------|----------|
|names | creator, project, team, named data| Keep it relevant and simple|
|sequential numbering | Run of experiment, version number |Include leading zeros|
|dates and times| year month and day created, range of years indicating a period for the data|Use [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format for dates to retain the order |
|unique identifier | subject id, project number, grant number| |
|experimental condition |lab instrument, solvent, temperature, etc.| |

### Tips for choosing and ordering components into names
What order should this information take? 

The order of these elements is primarily useful for browsing and sorting files on your computer. Especially is you want to have an overview of the files or directories.




### file order and sorting

Order the components of a name to organize your file by:

Date
Type
Subject
Sequential number (forced order)

Naming files by chronology - if using a date, use the format Year-Month-Day: YYYY-MM-DD or YYYY-MM or YYYY-YYYY. This will maintain chronological order of your files.
2006-03-24_Attachment
24 March 2006 Attachment
240306attch

Descriptive file naming Keep file names short and relevant - using sufficient characters to capture enough descriptive information
labtox_recent_110810_old version.sps
2010-08-11_bioassay_toxicity_V1.sps
FFTX_3776438656.sps

### Directory structure
Consider the organisation that will result from naming your files and folders a particular way and the scalability
e.g. project with names of regions like ILSSI for directories

I'll share my directory structure and file naming schemes I use with you. What's the problem with them? Do you see any?

Do not use generic file names that may conflict when moved from one location to another. 
Ensure filenames are independent of location and if you work on more than one computer ensure that your files are synchronised. 
Transportable rather than too context specific

[screenshot](../images/20170726-124454-screenshot.png)

[screenshot](../images/20170726-125025-screenshot.png)

### Tips when putting name components together
The way you put the components together is particularly useful for search. and cross-platform integration.

- Keep names under 32 characters
- Include relevant information for identification
- Include the same informational components
- Retain the order of components
- Avoid special characters ( & * % $ £ ] { ! @)
	- These are often used for specific tasks in different operating systems
- Use '-' or '_' instead of ' '
	- Like special characters, these are parsed differently on different systems.
- limit '.' to one before the file extension 

Do not assume that the software application or instrument uses case dependency when naming or renaming files within the aforementioned utility - assume that TANGO, Tango and tango are the same, even thought some file systems may consider them as different.

Where possible, use file extensions (often defaults) to accurately reflect the software environment in which the file was created and the physical format of the file. Eg use .por for SPSS portable files, .xls or .xlsx for Excel files, .ssd or .sas7bdat as appropriate for SAS files, .txt for text files, etc Exercise 
let's practice. Good practices for naming files, especially files associated with a research project are below.

Organising data with Professor Richard Rodger from University of Edinburgh [youtube](https://www.youtube.com/watch?v=RhxVmYtKqIY)

###




### Folder and file naming conventions
There are also a number of common elements that should be considered when developing a file naming strategy, including:


File names should outlast the file creator who originally named the file.

Consider how scalable your file naming policy needs to be e.g. if you want to include the project number, don't limit your project number to two digits, or you can only have ninety nine projects.

File and folder naming conventions are key to maintaining well-organised electronic directory and drive structures.

A filename is the chief identifier for a research data file. In most cases the policy for naming a file is left to individuals or to groups of individuals. 

There are a number of easy-to-follow rules that should be followed when naming data files:

Keep file names short and relevant - generally about 25 characters is a sufficient length to capture enough descriptive information for naming a data file

Do not use special characters in a filename such as : as 



The filename should include as much descriptive information that will assist identification independent of where it is stored.

If including dates, format them consistently.

.




- MANTRA "Organizaing data" [module](http://mantra.edina.ac.uk/organisingdata/)








### Strategies and trade-offs


## Exercise


generate potential file names for your data & document your strategy 
share your strategy with a partner & hear what they came up with
volunteer to share your idea with the class

## Set, forget... repeat
Okay, you might not get it right the first time. 

### Batch renaming
Although all operating systems have in-built tools for managing files, there are software tools that can organise research data files and folders in a consistent and automated way through batch renaming (also known as mass file renaming, bulk renaming). Batch renaming software exists for most operating systems.

There are many situations in which batch renaming may be useful, such as:

where images from digital cameras are automatically assigned base filenames consisting of sequential numbers

where proprietary software or instrumentation generate crude, default or multiple filenames

where files are transferred from a system that supports spaces and/or non-English characters in filenames to one that doesn't (or vice versa). Batch renaming software can be used to substitute such characters with acceptable ones.

Examples of bulk renaming tools include:


Windows:
Ant Renamer (www.antp.be/software/renamer)

RenameIT (sourceforge.net/prpjects/renameit)

Bulk Rename Utility (www.bulkrenameutility.co.uk/)

Mac:
Renamer 5 (for Mac) (renamer.com/)

Name Changer (mrrsoftware.com/namechanger/)

Linux:
GNOME Commander (www.nongnu.org/gcmd/)

GPRename (http://gprename.sourceforge.net/)

Unix:
The use of the grep command to search for regular expressions

- MANTRA "Organizaing data" [module](http://mantra.edina.ac.uk/organisingdata/)

File Renaming

Tools to help you:

Bulk Rename Utility (Windows; free)
Renamer (Mac; free trial)
PSRenamer (Linux, Mac, Windows; free)
File Naming Conventions for Specific Disciplines

Many disciplines have recommendations, for example:

DOE's Atmospheric Radiation Measurement (ARM) program

From: DMPTool "Data Management General Guidance" [website](https://dmptool.org/dm_guidance)




Basic Directory and File Naming Conventions

Research data files and folders need to be labelled and organised in a systematic way so that they are both identifiable and accessible for current and future users. The benefits of consistent data file labelling are:

- Data files are distinguishable from each other within their containing folder

- Data file naming prevents confusion when multiple people are working on shared files

- Data files are easier to locate and browse

- Data files can be retrieved not only by the creator but by other users

- Data files can be sorted in logical sequence

- Data files are not accidentally overwritten or deleted

- Different versions of data files can be identified

- If data files are moved to another storage platform their names will retain useful context 


There are three main criteria to consider regarding the naming and labelling of research data files, namely:

Organisation - important for future access and retrieval, and needs to take into account the file naming constraints of the system where the file is located

Context - this could include content specific or descriptive information, independent of where the data are stored

Consistency - choose a naming convention and ensure that the rules are followed systematically by always including the same information (such as date and time) in the same order (e.g. YYYYMMDD)

- MANTRA "Organizaing data" [module](http://mantra.edina.ac.uk/organisingdata/)

These are rough guidelines to follow to help manage your data files in case you don't already have your own internal conventions. When organizing files, the top-level directory/folder should include:

Project title
Unique identifier (Guidance on persistent external identifiers is available)
Date (yyyy or yyyy.mm.dd)
The sub-directory structure should have clear, documented naming conventions. Separate files or directories could apply, for example, to each run of an experiment, each version of a dataset, and/or each person in the group.

Reserve the 3-letter file extension for the file format, such as .txt, .pdf, or .csv.
Identify the activity or project in the file name.
Identify separate versions of files and datasets using file or directory naming conventions. It can quickly become difficult to identify the 'correct' version of a file.
Record all changes to a file no matter how small. Discard obsolete versions after making backups.

From: DMPTool "Data Management General Guidance" [website](https://dmptool.org/dm_guidance)

## Conclusion
The goal of having folder and file naming conventions is primarily for easy identification (through search and browse) and sorting. This way you can quickly navigate to the right place and identify the file or files you need at a glance.

Remember, you can use other means to save more information about your files and the data within them. We discussed this in more depth in the "Data Documentation" portion. This can be done inside the file itself or in a seperate Notebooks and README file that describe your file naming convention and file organization.

## References
- Library Carpentry. [lesson](https://data-lessons.github.io/library-data-intro/03-foundations/)
- MANTRA "Organizaing data" [module](http://mantra.edina.ac.uk/organisingdata/)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Spolsky, Joel. 2003. "The Absolute Minimum Every Software Developer Absolutely, Positively Must Know About Unicode and Character Sets (No Excuses!)"[blog](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)
- MIT Libraries [website](http://libraries.mit.edu/data-management/store/organize/)
- Meghan Frazer 2013 "An eleveator pitch for file naming conventions" [article](http://acrl.ala.org/techconnect/post/an-elevator-pitch-for-file-naming-conventions)

File management. Cornell Research Data Management Service Group. http://data.research.cornell.edu/content/file-management

## Materials