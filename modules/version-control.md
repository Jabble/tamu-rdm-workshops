# Version control
## Module objectives
- Understand the reason for using version control
- Identify elements of version control 
- Recognize the value of a Version Control System

## Introduction
**Versioning** is a way to keep track of changes to data over time. **Version control** is your set-up for tracking these changes and managing files as they change. Version control allows you to:

- Ensure what you do is transparent and reversible.
- Track your progress.
- Improve reproducibility.
- Reduce work when reconstructing how and why changes are made.

Your method of version control can be as simple as naming files and logging changes. Or, you can embrace a Version Control System to help you manage versioning. Regardless of your choice, the point is to find a way that helps you keep track of the changes made to files.

## Data stability
Data can be fixed or changing over the course of a project, and beyond a project's completion. You may work with:

1. **Fixed datasets** that never change after being collected or generated
2. **Growing datasets** where new data are added, but the old data are never changed or deleted
3. **Revisable datasets** where new data are added, and old data may be changed or deleted

*Examples of each*

The less stability in a dataset, the more complexity in tracking changes. This will impact the level of version control you may want to invest in.
 
Even fixed datasets will have several versions, raw data often needs to be transformed, cleaned or manipulated. But, keeping track of rapidly changing datasets can be a much bigger challenge. 

## Implementing version control
This will come up again, but I'd like to make the point that you'll always want to keep original data in a seperate file, raw and unchanged. Make a copy and start working with, and versioning, that.
 
We'll discuss two ways to implement version control.

1. Making copies of files as you work with them and adjusting the names. This will require you to document your changes seperately in your data documentation, and note when and how you choose to delete old versions. 

2. A Version Control System will require more investment at the beginning, but it will ease your work by automatically tracking changes as you work and allowing you to document your changes within the system.

### Simple: Saving files iteratively
Even a simple version control set-up is more than saving files with different names. You'll need to find ways to:

- Recognizably name new versions.
- Log a description of the changes made between versions, and/or track the changes themselves.
- Discard obsolete versions, especially if you have limited space.

### Example: non-linear workflow
raw data file 1
raw data file 2
combined 1+2 raw file
combined 1+2 v 1.0 -track changes
combined 1+2 v 2.0 -track changes

raw data file 3
combined 1+2+3 raw file -follow changes in combined 1+2 and track

### Tips
- Recognizably name new versions.
	- Save files iteratively after changes are made.
	- Confusing labels easily accumulate: revision, final, final2, definitive_copy, etc.
	- A common way is using ordinal numbers (1,2,3 etc.) for major version changes and decimals for minor changes e.g v1, v1.1, v2.6
- Log a description of the changes made between versions, and/or track the changes themselves.
	- use notes or readme files to document changes
	- use track changes features when working collaboratively in GooglDocs, Word Documents, on Wikis.
- Discard obsolete versions, especially if you have limited space.
	- Discard or delete obsolete versions (but retain the original 'raw' copy)
	- Use an auto-backup facility (if available) rather than saving or archiving multiple versions
	


Some structured examples of maintaining version control [document name] [version number] [status: draft/final]:

Smith_interview_July2010_V1_DRAFT

Lipid-analysis-rate-V2_definitive

2001_01_28_ILB_CS3_V6_AB_edited

### Exercise: 
Why should you discard or delete obsolete versions of data files?

Too many similar or related files may be confusing, both to yourself and to anyone else wanting to access or use your data. You may think that you know which data file is which but that may not always be the case as time passes and the number of different file versions increase. It is easier to maintain a manageable number of versions with a clear naming structure. As long as the original 'raw' or definitive copy is retained and processing is well documented, the intermediate working files can and should be discarded.

What advantages are there to a consistent approach to expressing data file versions?

A consistent approach to expressing data file versions means that you can easily identify the most recent copy of a file or a final version of a file without having to open each file (which would also require a good memory as to what was changed in the file and when!). If a common file naming or versioning procedure is used with research colleagues or collaborators it also means that file exchange and file sharing can be made easier.

- MANTRA "Organizaing data" [module](http://mantra.edina.ac.uk/organisingdata/)

### Robust: Using a Version Control System
Version Control Systems (VCS) are software tools to help you automate version control. Depending on how you work, this may require buy-in from collaborators.

"Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later."
Git. "Getting Started - About Version Control" [website](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)

This kind of system stores the changes made and allows you to write documentation each time you've made changes and decide to create a new version.

Consider using version control software e.g. 

- Subversion: Centralized Version Control System. Older. (https://subversion.apache.org)  

- Git: Distributed Version Control System. From software development community. Widely used with lots of help, integrates with services like Github and Bitbucket (https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)

- Mercurial: Distributed Version Control System. Simpler than Git. (https://www.mercurial-scm.org)

### Demo: Git
Benefits, but they have a steeper learning curve. We aren't going to get into the details in this workshop. But I will show you how one software looks. This is Git.

You implement Git by telling the software where it should look. So, a folder/directory it should pay attention to. If there are any changes within this folder/directory including addinf folders, adding files, making changes to exisitng files, deleting files, Git will track the changes. But, you need to log the changes you've made in order to Git to make distinct versions that you can roll back to. So, as soon as you make a change that is big enough where you want to make sure you don't lose anything between now and your future changes, you commit and then push changes to a new version.

## Conclusion

Even with a VCS, it is still a good idea to keep a seperate, unchanged, file with the original data.

A consistent approach to expressing data file versions means that you can easily identify the most recent copy of a file or a final version of a file without having to open each file (which would also require a good memory as to what was changed in the file and when!). If a common file naming or versioning procedure is used with research colleagues or collaborators it also means that file exchange and file sharing can be made easier.

## References
- DMPTool. "Data Management General Guidance" [website](https://dmptool.org/dm_guidance)