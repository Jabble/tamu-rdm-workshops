# Data documentation
## 2.  Introduction
In this section, we'll focus on documenting your data 

- to help you share information about your project with your advisor, 
- write your thesis or dissertation, 
- and to ensure your data are useful later.

Data documentation starts during collection and continues throughout the time you work with the data, including when performing quality assurance and analysis.

## 3. Why document 
It will enable:

- You to get a mess of details out of your head, so that you can focus on doing your work and avoid forgetting important considerations.
- You can reproduce and improve workflows in the future.
Other researchers, including your collaborators, to find the right data and use them properly.

Clear and detailed documentation is essential for data to be understood, interpreted, and used. 

Generally, data documentation explains the 

- who
- what
- where
- when
- and why of data

## 4. Discussion
- As you are working on a research project, what sort of information do you document?
- How do you document that information?


## 5. What to document
- If you have experience with research, you may already have a process for documenting your data or be familiar with the information you need to note. 
	- We’ll talk about formalizing that process a little. 
- If you're new to research or you're working outside of a lab context, you may want to dig more deeply into good practices for documenting you work.

The practices we discuss today build into our future conversation about sharing data and using metadata standards to describe datasets.

Let’s start by breaking documentation down into two levels.

**High-level** documentation explains your research goals and the progress of your project. And gives an overview of your work and methods. 

**Low-level** documentation explains the details of the data, how it has been collected, stored, and changed over time. This is the nitty gritty of your process.

Both of these are valuable to create and maintain throughout your research, because they will help you to recall your work and explain it to others as you get into the messy details of research.

## 6. Project documentation 
Explains:

- Rationale and context for data collection
- Research questions/hypotheses
- Data sources, collection methodology, protocols
- Data validation and quality assurance actions
- Transformation of raw or derived data for integration or analysis
- Data confidentiality, access, and use conditions

## 7. Dataset documentation 
Explains:

- Variable names and descriptions
- Codes and classification schemes
- Algorithms used to transform data 
- Structure and organization of files
- Relationship among data files or tables in a database schema
- Version information
- File formats and software used

## 8. How to document
We’ve gone over the generak information that is worth documenting, and likely for you to find valuable. 
Now let’s talk a little about the ways in which you may want to document your project and data.

- Laboratory notebooks
- Codebooks and data dictionaries
- README and log files

## 9. Notebooks 
For projects including observational and experimental data sources, lab and field notebooks are crucial components of data management. However, notebooks are also helpful to save project-level documentation when working with data from other sources.

Keeping a notebook is the most thorough method of documentation we’ll discuss, and can serve as a personal thinking tool as well as a reference.

- Provide a central and physical location for protocols, results, and happenings. 
	- You have one place to go.
	- This gives context when you go back to see what you were thinking one or two years ago.
- Encourage a thoughtful process. 
	- The act of writing forces you to explore and clarify ideas.
- Enable continuity in the face of unexpected events or time passing. 
- Provide a record of how your data were collected, organized, and processed. 
	- Establishing a legal and scientific provenance (historical record) of your work.
	
## 10. Analog and digital
### Physical notebooks
- Great in a messy lab or the field. May be easier to carry with you and work with.
- Free-form, and flexible note taking and 
	- allows you to easily mix media (photos, drawings, calculations, notations)
- can be scanned or photographed later and saved to a computer as an image file.

### Digital notes
- Can be useful in a lab setting for collaborative work and sharing notes and responsibilities in a single place.
- Electronic lab notebooks (ELNs) are becoming more popular in biological sciences.
- You might also simply prefer to enter your notes on a computer, sync across computers, and link your notes other digital files using a general-purpose note-taking software.
- Here it's worth noting the file format that different not taking softwares use, and what your export options are (if you even need to change software or share notes outside of the software)

## 11. Analog lab notebook example (features and tips)
- stitched binding that lays flat when open
- larger size is generally better
- Page numbers at top here, better quality paper and pre-numbered pages are worth it
- Date at top to indicate when notes were taken and thoughts were had.
- Signature at bottom as a certification of authorship
- Allos for Mistakes crossed out clearly and noted
- Pasting-in images

## 12. Note-taking software
Are you familiar with any of these?

1. SciNote: sciNote is a free electronic laboratory notebook (ELN) (at the basic level) You may use something like this if you work in the biological sciences, they are becoming more common in a lab setting.


The next two are Computer and Mobile Software that is more general-purpose:

2. OneNote: general-purpose note taking software. If you like the MS Office suite this might be for you. 
3. Evernote: Is a popular general-purpose note taking software. One of it’s neat features is that it will grab articles from websites, format and save them as notes for you.

4. Jupiter Notebooks: Worth knowing about, especially if you write code, and especially if you code in Python, but also Bash, R, MATLAB. Browser-based tool for interactive authoring of documents. They allow you to interleave executable code with explanatory text.

### Scinote
- Scinote organized into projects that different teams can see. 
- Each project can contain named experiments that contain information and can be moved, copied, and archived.
- A Task is a basic unit within an Experiment. 
- Within a Task, you can add Protocols, Results or Samples. 
- You can connect Tasks into Workflows to assure traceability of your work. 
- Inside of a Task you can create Protocol steps and upload existing protocol files. 
- After you have finished a certain step, click the Complete step button. 
- Exact time and the person who completed the step are recorded and can be seen in the Activity
- Centralized lab notebook and can also serve as an experiment management system for labs and teams.
- You can also generate reports of your work

### Onenote
- Microsoft product. May be nice if your comfortable with the Microsoft office ecosystem.
- Allows you to write notes and add images and other media anywhere on the page. 
- Organized into notebooks with sections and pages
- Can be synced online
- Can save notes as PDF, and may be able to share online. 
- But it’s worth being careful using these notebooks because they might not be the friendliest in trying to export away from Microsoft products.

### Evernote
- Application with a free and paid option
- Online and on desktop, synchronize across computers
- Allows you to grab information from webpages
- Can include Text, links, images and annotations
- Allows for organization into notebooks
- Can link to other services like Google Drive.
- Can share within the app, or export as HTML, save as a PDF file

### Jupyter notebooks
- If you write code, and especially if you code in Python, but also Bash, R, MATLAB. [Website](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels)
- Jupyter notebook software runs locally using a browser-based tool for interactive authoring of documents. 

They allow you to:

- Interleave executable code with explanatory text.
	- Can include inputs and outputs of the computations, explanatory text, mathematics, images, and rich media representations of objects.
	- Specifically a neat thing is that you can write your notes including LaTeX for mathematical expressions, and they will be formatted for you.
- Execute code from the browser, with the results of computations attached to the code which generated them.
- Edit code with automatic syntax highlighting, indentation, and tab completion.
- These documents are internally JSON files. Since JSON is a plain text format, they can be version-controlled and shared with colleagues.

Notebooks may be exported to a range of static formats, including HTML (for blog posts and web pages), LaTeX, PDF, and slide shows, publication-quality figures rendered by the matplotlib library.

## 18. Good practices and tips
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

## 19. Good practices and tips
- Note mistakes in detail and what needed to be fixed
- Annotate all calculations and include units
- If data are logged or added on a computer, record file names of data
	- Include where they are stored and backed up
- Describe the locations of physical materials: data binders, seeds, samples, etc.
- Use images to simplify documentation
	- Take photos or make quick drawings of set-ups, locations, etc.

## 20. README files
README files are another tool you can use to document your data. They are usually stand-alone plain text files within a folder and aptly named “README.txt”.

These documents are common in software development where they account for and describe the the files and folders in a project. 

For data, README files are useful for outlining more detailed information about your datasets, in addition to describing the organization of the digital files and folders that contain your data. They can also contain some contextual information about the project.

They help you, or if you are sharing your data, someone else to get oriented by outlining how the data in different files connect, where files are located, and what to expect within each file. 

If you use a notebook, you can extract information from the notebook and include the necessary details in the README.

## 21. Example: README template
README files can be free-form, or very structured, to describe the contents, structure, and layout of a data collection.

This is a structured template example from Cornell university, to give you an idea of the type of information that is relevant.

Your own README’s don’t need to be this detailed, but you can use this as a template, to develop your own template, or simply for ideas about the information you would like to capture about your data.

## 22. README tips
I recommend that you use a README.txt file at the top level of your project folder to explain the purpose of the project, the relevant summary and contact details, and general organization of your files. 

This is equivalent to using the first page of your laboratory notebook to give a general description of your project.

## 23. Codebooks and data dicitonaries
- While README files describe a collection of data and how the digital files and data within them are organized; 
- Codebooks and data dictionaries are give a detailed description of the data at the level of each variable within a dataset.

They can be contained within a README doc. 
We saw an example of this in the Cornell template within the “DATA-SPECIFIC INFORMATION FOR: [FILENAME]” section.

They can also be separate files, or even part of a data spreadsheet like the one we looked in the data collection portion.

- **Codebooks** are commonly used in social sciences, as a document containing the list of codes used in research. 
- A well-documented codebook "contains information intended to be complete and self-explanatory for each variable in a particular data file.” 
- **Data dictionaries** are sometimes considered less informative than a codebook, but contain the same kind of information. 
- For the purposes of this presentation, data dictionaries and codebooks are pretty much the same thing.

## 24.–26 Example: Tabular data with a data dictionary
Go ahead and download these two files. One of them contains data, and the other one contains a code book.

The Data are from the Duke Lemur Center about the weight of lemurs. 

Let's look at this first. The data are clean, especially compared to the messy spreadsheet were were working with before. 
You might also have notices that these data were saved in a plain text file (CSV) and MS Excel was able to open and display the data. 
I could also open this data in a plain text editor.

Okay, so we have a clean dataset to look at.
But they cannot be interpreted from the spreadsheet alone. 

- For example, What does the variable ‘AgeAtWt_mo_NoDec’ mean?
- What does the value  ‘CMED’ within the variable ‘Taxon’ mean?

### Data dictionary
Enter the data dictionary in the form of the README.docx file.

- lays out information on each variable in the dataset. For example, it defines the variable “AgeAtWt_mo_NoDec” as
- Age in months with no decimal:  AgeAtWt_mo  value rounded down to a whole number for use in computing average individual weights (FLOOR(AgeAtWt_mo))

- it also lists the the various taxonomic codes used within the ‘taxon’ variable.

This way we can actually understand and make use of the data in the CSV file.

## 27. DDI Codebook example
We just looked in detail as a data dictionary for a dataset about Lemurs. 
 I’d also like to share what a more detailed codebook could look like.

This little snippet is from a codebook that uses the DDI standard. 
DDI stands for the Data Documentation Initiative (also known as DDI Metadata).
An international standard for describing surveys, questionnaires, statistical data files, and social sciences study-level information.

This snippet is from the documentation for a National Household Survey, done in Canada in 2011.
We're looking at information about the number of bedrooms in Canadian households.

It includes the same kind information as the codebook we looked at.
At the top “BEDRM” is the variable name and a definition is included.˜
then “value” and label” indicate the code and it’s meaning

This codebook contains more information about the variable (data quality note, statistics about the variable)

## 28. Good practices and tips
This list represents the types of things you would want to know when faced with an unknown dataset. 
And what ought to be included in a document like a codebook or data dictionary.

Name assigned to the variable
What the variable represents.
Variable format, how the variable was actually recorded in the raw data 
numeric, string; how many characters wide it is; how many decimal places it has
For scale variables: The variable's units of measurement
For categorical variables: If coded numerically, the numeric codes and what they represent
Null value indicator and missing value codes
Known issues with the data (systematic errors, missing values, etc.)
Relationship to other variables

## 29. Conclusion
- Identified relevant project-level and data-level documentation.
- Reviewed documentation tools including lab notebooks, README files, and codebooks.
	- Lab notebooks can be used for thorough note taking and thinking.
	- If you’re working with a single dataset, a codebook or a data dictionary may be enough documentation about the data. 
	- If you’re working with a set of folders and data files, a readme file can be useful to explain how those files are organized.

Any questions about these things?

## 30. References and resources
*Go over them*
- Data Packaging Guide [Website](https://github.com/saverkamp/beyond-open-data/blob/master/DataGuide.md)