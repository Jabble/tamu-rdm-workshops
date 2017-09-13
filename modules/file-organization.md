# File organization
## Objectives
- Recognize the purpose of file naming conventions.
- Explain the components of sensible file names.
- Compare and critique file naming conventions.

## Introduction
In this module, we'll look at organizing data files with accessibility in mind. The goal is for you to be aware of strategies that can help you focus on working with your data, rather than trying to find files. 

Professor Jeff Haywood at the University of Edinburgh on the importance of good file management [youtube](https://www.youtube.com/watch?v=i2jcOJOFUZg)

## Exercise: Your current practices
*Pair and share activity*
Do you or your research group already have a particular way of naming files? 
Can you describe what goes into a file name?
Does you have a method for organizing your computer folders/directories?

*Share, did you learn something from your partner. What is something you didn't know?*

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
Let's start at the low level. What ought to go into a file name? Earlier, I said "sensible things." These things will depend on your project and expected use. 

Generally, descriptive information that will help you identify the content you seek when browsing, sorting, and/or searching, especially in the case when additional context is lost or missing.

When constructing files, the following components are "sensible things." Use them alone or in a combination that suits your needs.

|Informational component | Possible use | Tip |
|----------|----------|----------|
|Names or acronyms | creator, project, team, named data| Keep it relevant and simple|
|Sequential numbering | Run of experiment, version number |Include leading zeros|
|Dates and times| date of creation, date range of experiment|Use YYYY-MM-DD([ISO 8601](https://en.wikipedia.org/wiki/ISO_8601))format|
|Unique identifier | subject id, project number, grant number| Keep it relevant and simple|
|Research condition |lab instrument, solvent, temperature, spatial coordinates, etc.| Keep it relevant and simple|
|Type or keyword| denote type of content within a file|Work from a standard list|

## Arranging components into names
We'll discuss tips for choosing and arranging components into names. The choice of components and their arrangement will affect how files are ordered and sorted on your computer, and the directory structure.

### File order and sorting
The order of these elements is primarily useful for browsing and sorting files on your computer. Especially if you want to have an overview.

Date - chronological order
	20170809
	2017-08-09
Type - categorical order
	table
	photo
	graph
Name or initials - order by creator
	dabrowski
	ajd
Sequential number - order by experimental run
	01
	001
Extension - keep last
	.csv
	.png
	.pdf
*create examples of manipulating order, include file extensions CSV and PNG*

Note: Each strategy has trade-offs

### Directory structure
Consider the organisation that will result from naming your files and folders a particular way
e.g. project with names of regions like ILSSI for directories

Type of analysis 
Country
Region
Data files

Country
Region
Type of analysis  
Data files

Remember to thnk in terms of scalability. What happens when you have more data for a particular region? What happens when you add a new region? What's most likely?

The sub-directory structure should have clear, documented naming conventions. Separate files or directories could apply, for example, to each run of an experiment, each version of a dataset, and/or each person in the group.

## Exercise: Critique me!
I'll share my directory structure and file naming schemes I use with you. What's the problem with them? Do you see any?

[screenshot](../images/20170726-124454-screenshot.png)

[screenshot](../images/20170726-125025-screenshot.png)

What do you notice? 
what components to I include?
I use all lowercase, and '_' and '-' for different purposes.
I use generic file names that may conflict when moved from one location to another.
I'm inconsistent use YYYYMMDD as a sequence, but not always
I use different naming in different directories

Consider how scalable your file naming policy needs to be e.g. if you want to include the project number, don't limit your project number to two digits, or you can only have ninety nine projects.

## Putting components together
The way you put the components together is important for cross-platform integration and useful for search.

- Keep names under 32 characters
- Include relevant information for identification
- Include the same informational components
- Retain the order of components
- Avoid special characters ( & * % $ £ ] { ! @)
	- These are often used for specific tasks in different operating systems
- Use '-' or '_' instead of ' '
	- Like special characters, these are parsed differently on different systems.
- limit '.' to one before the file extension 
- Software may or may not distinguish case
	- assume that TANGO, Tango and tango are the same
- include file extensions (often defaults) to accurately reflect the software environment in which the file was created

Organising data with Professor Richard Rodger from University of Edinburgh [youtube](https://www.youtube.com/watch?v=RhxVmYtKqIY)

## Exercise: 
Which components do you think are most useful?
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

## Conclusion
The goal of having folder and file naming conventions is primarily for easy identification when searching, browsing, and sorting. This way you can quickly navigate to the right place and identify the file or files you need at a glance.

Remember, you can use other means to save more information about your files and the data within them.We discussed this in more depth in the "Data Documentation" portion. 

Use codebook to explain your naming format along with any abbreviations or codes you have used.

This can be done inside the file itself or in a seperate Notebooks and README file that describe your file naming convention and file organization. 

## References
- Cornell. "File management" [Website](https://data.research.cornell.edu/content/file-management)
- DMPTool "Data Management General Guidance" [website](https://dmptool.org/dm_guidance)
- Library Carpentry. [lesson](https://data-lessons.github.io/library-data-intro/03-foundations/)
- MANTRA "Organizaing data" [module](http://mantra.edina.ac.uk/organisingdata/)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Spolsky, Joel. 2003. "The Absolute Minimum Every Software Developer Absolutely, Positively Must Know About Unicode and Character Sets (No Excuses!)"[blog](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)
- MIT Libraries [website](http://libraries.mit.edu/data-management/store/organize/)
- Meghan Frazer 2013 "An eleveator pitch for file naming conventions" [article](http://acrl.ala.org/techconnect/post/an-elevator-pitch-for-file-naming-conventions)

. Cornell Research Data Management Service Group. http://data.research.cornell.edu/content/file-management

## Materials