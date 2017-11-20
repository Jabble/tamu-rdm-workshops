# File organization
## 2. Worshops
Today we'll talk about storing digital data in 3 sections:

- File organization
- Version control
- Storage, Backup, and security

## 3. Introduction
First we'll look at organizing data files with accessibility in mind. 

The goal is for you to be aware of strategies that can help you focus on working with your data, rather than trying to find files. 

Professor Jeff Haywood at the University of Edinburgh on the importance of good file management [youtube](https://www.youtube.com/watch?v=i2jcOJOFUZg)

## 4. Discussion
- Do you or your research group already have a particular way of naming files? 
- Can you describe what goes into a file name?
- Does you have a method for organizing your computer folders/directories?

## 5. Example
- Here's an example of data file naming I recreated from PhD Comics. 
- It might be a bit of an exaggeration, but it illustrates some common problems that occur when people are in a hurry and don't have a convention.
- This is what you want to avoid.

What’s the problem here?

1. If you’re browsing, the sequence is unclear. The date could be helpful, but these may or may not be incremental versions
2. The file names seem to include comments rather than useful descriptive information.
3. If you are using the search feature on your computer. Very difficult to know what to search for since notes to self like ‘USETHISONE’ and ‘woohoo!!’ are unlikely to be standard terms you remember. File names are not a place for notes.

This also applies to including notes included in file names like “Draft” “FinalDraft” “FinalDraft-revised”…

### What to do instead?
- Offset notes to yourself to documentation, like your notebook or even a README file.
- Use a simple convention for naming files and directories/folders sensible things and organizing files.

## 6. Naming conventions
Naming conventions make files are easier to:

- organize,
- group,
- move, 
- sort, 
- find via searching (keywords) and browsing. 

Choosing a naming convention is one of those things to think about a little in advance.

- Set your standard
- Make it a habit to follow your convention
	- Ensure that the rules are followed systematically by including the **same information** in the **same order**.
- And more or less forget. If it isn't working for you, you can reasses and make changes.

conventions for your:

1. File names
2. Folder names
3. Directory structure

These conventions can also be documented in your README file or notes.

## 7. What's in a name?
- Starting at the low level, here are the "sensible things" that ought to go into a file name.
- Components you choose will depend on your project and expected use, but these components represent
- Descriptive information that will help you identify the content you seek when browsing, sorting, and/or searching,
	 - Especially in the case when additional context is lost or missing.

*Review components on slide*

## 8. Putting components together
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

*Organising data with Professor Richard Rodger from University of Edinburgh [youtube](https://www.youtube.com/watch?v=RhxVmYtKqIY)*


## 9. Arranging components into names
The choice of components and their arrangement will affect how files are ordered and sorted on your computer.

*Review components order and sorting*

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

Note: Each strategy has trade-offs

## 10. Example: Generic file naming convention
*Review how a naming convention may be written out in documentation*

- You'll want to write down your naming convention, so that you can keep track if you make changes or need a reminder. 
- And you can easily plop it into a README file or other documentation.


## 11. Directory structure
If you haven't already, you'll want to think in advance and consider the structure that will result from organizing your files and folders a particular way.

The directory structure should have clear connection with how you work and also be documented. 

Again, This is exactly the kind of thing for a README file. 

You may want to base your directory structure on things like:

- the projects your're working on, 
- the subject matter covered by those projects, 
- perhaps the person responsible if responsibilities are shared,
- types of documents you produce or expect to produce, 
- and can even get down to the run of an experiment.

### Example
Here is an example of a research project that involves several different types of analysis in multiple countries. 

It's worth thinking about

- which information is relevant to you
- how you would prefer to find files 
- and (in this case) how the structure would change if:
	- you add a new analysis, 
	- or expand your analyses to a new country or region.
	- Remember to think in terms of scalability, and where you'r most likely to expand. 
		- What happens when you have more data for a particular country, or decide to break-down analyses by region?
 
## 12. Exercise: Critique me!
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
Which components do you think are most useful?
generate potential file names for your data & document your strategy 
share your strategy with a partner & hear what they came up with
volunteer to share your idea with the class

## 13. Set, forget... repeat
Okay, you might not get it right the first time. 

### Batch renaming
Batch file renaming can help you rename a group of files at one time.

- It is helpful if you decide to change or adjust your file naming conventions and have already named a lot of files with one convention.


There are other situations in which batch renaming may be useful, such as:

- where images from digital cameras are automatically assigned base filenames consisting of sequential numbers
- where proprietary software or instrumentation generate crude, default or multiple filenames
- where files are transferred from a system that supports spaces and/or non-English characters in filenames to one that doesn't. Batch renaming software can be used to substitute characters.

The Mac OS has a built-in tool.
A few tools for Windows include: *See slides*

## Conclusion
- Reviewed the purpose of file naming conventions.
	- The goal of having folder and file naming conventions is primarily for easy identification when searching, browsing, and sorting. 
	- This way you can quickly navigate to the right place and identify the file or files you need at a glance.
- Discussed the components of sensible file names.
- Compared and critique file naming conventions.

Remember, you can use other means to save more information about your files and the data within them.

We discussed this in more depth in the "Data Documentation" portion. 

## References
Cornell. "File management" [Website](https://data.research.cornell.edu/content/file-management)
DMPTool "Data Management General Guidance" [Website](https://dmptool.org/dm_guidance)
Library Carpentry. [Lesson](https://data-lessons.github.io/library-data-intro/03-foundations/)
MANTRA "Organizaing data" [Module](http://mantra.edina.ac.uk/organisingdata/)
MIT Libraries [Website](http://libraries.mit.edu/data-management/store/organize/)
Frazer, Meghan. 2013. "An eleveator pitch for file naming conventions" [Article](http://acrl.ala.org/techconnect/post/an-elevator-pitch-for-file-naming-conventions)