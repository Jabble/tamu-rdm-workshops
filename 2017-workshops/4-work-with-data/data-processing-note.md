# Data processing
## 2. Introduction
- In addition to QA/QC tasks, you will need to do some data processessing as you prepare and analyze your data.
- We'll talk about common manipulations of data including some common data transformations and tools for processing data.
- We won't get deeply into data analysis, because this will largely depend on your specific data and project. 
- However, we will cover ways to document your process.
- Process your data in a manner that allows you to roll back changes if you make a mistake.

## 3. Preparing data for analysis
Typically the first step before data analysis is processing the data. 

**Processing** could be as simple as:

- Selecting a subset of the data for analysis or presentation. 
- Merging multiple datasets, 
- or manipulating the data themselves so they are more usable by a researcher or a computer program.  

A common requirement for large datasets is to reduce the amount of data in the working data file. This makes computing and handling of the dataset easier.

### Example 
- A sensor may take a temperature measurement every 5 seconds for one year. 
- For the study, only monthly patterns are important. 
- We might therefore only use one data point for every 5 minutes, and the dataset would be processed to remove the extra points.

## 4.  Data transformation
**Transformation** refers to making changes to data values. 
Transformations may be done at any point after data are gathered. 
They could be part of data entry, quality control, or seperate data processing steps. 

These are actions like:

- Normalizing data collected by multiple people and/or instruments, 
- Converting data to different units, 
- Or developing algorithms for converting raw data into meaningful values. 

### Examples
1. Sensor readings
- The string of numbers on the left is the raw output from a sensor. 
- This can (and may need to) be transformed into the table on the right, 
- by seperating (or parsing) out different elements. 
- In order to make the data more understandable for humans and useful for analysis.

2. Survey data 
- Collected from questionnaires, multiple choice and other kinds of responses are usually coded as numbers instead of character strings. 
- This simple transformation has the advantages of easing data entry if typing in paper responses and avoiding inconsistencies (e.g. typos) in data values.

3. Qualitative data
- For example interview transcripts, may be transformed into quantitative data by applying textual coding and categorisation techniques. 
- Such variables are categorical or nominal, and can have a some statistical techniques applied to them. 

3. Experimental data
- Variables measured at an ordinal, interval or ratio level, that is 'real' numbers where a value reflects some measurement of the concept of interest, 
- allow for a wider range of methods of analysis.

## 5. De-identification
De-identification of data refers to the process of removing or obscuring any personally identifiable information from individual records 

This is done to minimizes the risk of unintended disclosure of the identity of individuals and information about them. 

- Specific steps and methods used to de-identify information will vary depending on the circumstances, 
- Should be appropriate to protect the confidentiality of the individuals. 
- Note that PII may include not only direct idenfiers.
- But also any other sensitive and non-sensitive information that alone or combined is linked or linkable to a specific individual, and would allow identification. 

A number of techniques may be used to transform confidential or sensitive data so that they may be shared with other researchers. Some include:

- Anonymisation: cases/observations are stripped of revealing identifiers. 
	- Anonymization produces data where individual records cannot be linked back to an original because they do not include the required mapping to do so.	
- Aggregation/generalization: "the combination of related categories, usually within a common branch of a hierarchy, to provide information at a broader level to that at which detailed observations are taken." (OECD definition).
	- Geographical data are also often aggregated to a higher unit, where information is deemed sensitive or revealing.
	- A low population postal code can be aggregated to a larger geographic area (such as a city). 
	- A rare profession can be aggregated to a more general description.
- Masking: Replace sensitive information with realistic but fake data.
	- The purpose of this technique is to retain the structure and functional usability of the data, while concealing information that could lead to the identification, either directly or indirectly, of an individual value
- Shuffling: Data for one or more variables are switched with another record.
	- All of the values in the data set are real, but they are assigned to the wrong observation.
- Perturbation: a deliberate distortion is introduced at the level of tabular data cells. 
	- Population Census data are sometimes released with perturbations as a trade-off for geographical detail.
	- Involves making small changes to the data to prevent identification of individuals from unique or rare population groups.

## 6. De-identification tips

- Remove direct identifiers.
	- Names, addresses, institutions, photos, id numbers.
- Use pseudonyms or replacements.
	- Pseudonymisation is a common technique for protecting identities in qualitative data.
	- Avoid blanking out.
	- Identify where you have used replacements, for example with [brackets].
- Reduce the precision/detail through aggregation.
	- Birth year/decade for date of birth.
	- Could involce combining variables.
- Generalize meaning of detailed text variables.
	- Occupational expertise vs specific position.
- Restrict upper or lower ranges to hide outliers.
	- group income and age into wider categories.
- Use digital manipulation of audio and image files to remove personal identifiers.
	- Voice alteration, image blurring (eg, of faces).
	- This is labor intensive, expensive and can damage research potential of data.
	- Better solution:
		- Obtain consent to use and share unaltered data for research purposes (potentially with some access conditions).
		- Avoid mentioning information that discloses identity during audio recording.
- Avoid over-anonymization.
	- Removing / aggregating information can make the data more difficult to interpret, distort them, or make them misleading or unusable.
- Exercise additional care if working as a team.
	- Maintain consistency within the team and throughout the project.
- Keep master log of all replacements/ aggregations/ removals.
	- Keep in a secure location separate from the anonymized data files.
	- This is part of your documentation.

From: QDR [website](https://qdr.syr.edu/guidance/teaching)

## 7. Statistics
Some transformations are purely statistical, and are used to prepare the data to fit a model. 

- For example, a logarithmic transformation to make a skewed distribution fit on a normal (bell) curve.

Statistics are among the most common types of analyses performed on data. 

There are many different types of statistical analyses.  

1. Conventional statistics are often used to understand experimental data:
- The most common types are analysis of variance (ANOVA), multivariate analysis of variance (MANOVA), and regressions. 
- Conventional statistics tend to rely on assumptions such as random error and homogeneous variance. 

2. Descriptive statistics are traditionally applied to observational data. 
- Summary statistics that quantitatively describe or summarize features.
- describing the distribution of a single variable, including:
	 - central tendency (including the mean, median, and mode),
	 - dispersion (including the range and quartiles of the data-set,
	 - measures of spread such as the variance and standard deviation), 
	 - the shape of the distribution may also be described.
- more than one variable, descriptive statistics may be used to describe the relationship between pairs of variables.

3. Statistical analyses might also include temporal or spatial analyses, and nonparametric approaches which do not rely on specific assumptions about the data’s distribution.

## 8. Software for data manipulation and analysis
Tabular data

### Excel and GoogleDocs
- Generally popular tools.
- Excel: calculation, graphing tools, pivot tables, and a macro programming language called Visual Basic for Applications.
	- It has a battery of supplied functions to answer statistical, engineering and financial needs. 
	- In addition, it can display data as line graphs, histograms and charts, and with a very limited three-dimensional graphical display

### OpenRefine
- General tool used for data cleanup and transformation to other formats.
- Can be especially useful if you need to adjust and clean data you intend to combine.
	- Cleaning messy data: for example if working with a text file with some semi-structured data, it can be edited using transformations, facets and clustering to make the data cleanly structured.[8]
	- Transformation of data: converting values to other formats, normalizing and denormalizing.
	- Parsing data from web sites: OpenRefine has a URL fetch feature and jsoup HTML parser and DOM engine.[9]
	- Adding data to dataset by fetching it from webservices (i.e. returning json).[10] For example, can be used for geocoding addresses to geographic coordinates.[11]

- It is similar to spreadsheet applications (and can work with spreadsheet file formats); however, it behaves more like a database.
- Most operations in OpenRefine are done on all visible rows: transformation of all cells in all rows under one column
- Transformation expressions can be written in General Refine Expression Language (GREL)


### NVIVO
- Designed for qualitative researchers working with very rich text-based and/or multimedia information, where deep levels of analysis on small or large volumes of data are required.
- Popular in social sciences such as anthropology, psychology, sociology.
- NVivo is intended to help users organize and analyze non-numerical or unstructured data. The software allows users to:
	 - classify, sort and arrange information; 
	 - examine relationships in the data; 
	 - and combine analysis with linking, shaping, searching and modeling.

- NVivo supports data formats such as:
	- Audio files, videos, digital photos, Word, PDF, spreadsheets, rich text, plain text and web and social media data.[4] 
	- Users can interchange data with applications like Microsoft Excel, Microsoft Word, IBM SPSS Statistics, EndNote, Microsoft OneNote, SurveyMonkey and Evernote; and order transcripts from within NVivo projects, using TranscribeMe

### SAS
- SAS more powerfuls than SPSS and STATA, can handle big data, faster. But requires more coding.

- Designed for advanced analytics, multivariate analyses, business intelligence, and predictive analytics.
	- can mine, alter, manage and retrieve data from a variety of sources and perform statistical analysis on it.
- Popular for business intelligence and data analyses in health service research.
- SAS provides a graphical point-and-click user interface for non-technical users and more advanced options through the SAS language.

- Data should be in a spreadsheet table format or SAS format.
- SAS data can be published in HTML, PDF, Excel and other formats using the Output Delivery System

### SPSS
- SPSS and Stata have similar power and similar analysis for users. Difference SPSS has an easier user interface. Stata requires some coding, but easy if you know the right terms. If know both, prefer one over or the other depends on analysis.

- Used for logical batched and non-batched statistical analysis, data mining, and text analytics.
- Popular in social sciences, health sciences, and marketing.
	- Descriptive statistics: Cross tabulation, Frequencies, Descriptives, Explore, Descriptive Ratio Statistics
	- Bivariate statistics: Means, t-test, ANOVA, Correlation (bivariate, partial, distances), Nonparametric tests
	- Prediction for numerical outcomes: Linear regression
	- Prediction for identifying groups: Factor analysis, cluster analysis (two-step, K-means, hierarchical), Discriminant

- features of the base software:
- statistical analysis, 
- data management (case selection, file reshaping, creating derived data) 
- and data documentation (a metadata dictionary was stored in the datafile) are .

- SPSS Statistics can read and write data from ASCII text files (including hierarchical files), other statistics packages, spreadsheets and databases. 
- SPSS Statistics can read and write to external relational database tables via ODBC and SQL.
- Statistical output is to a proprietary file format (*.spv file, supporting pivot tables) for which, in addition to the in-package viewer, a stand-alone reader can be downloaded. 
- The proprietary output can be exported to text or Microsoft Word, PDF, Excel, and other formats.

### STATA
- General-purpose statistical software package.
- Populae in economics, sociology, political science, biomedicine and epidemiology.
- Capabilities include statistical analysis, graphics, simulations, regression, and custom programming

- Stata can import data in a variety of formats. This includes ASCII data formats (such as CSV or databank formats) and spreadsheet formats (including various Excel formats).
- Stata's proprietary file formats are platform independent, so users of different operating systems can easily exchange datasets and programs. 

### Matlab
- Multi-paradigm numerical computing environment built around the MATLAB scripting language.
- Users come from various backgrounds of engineering, science, and economics.
- Allows matrix manipulations, plotting of functions and data, implementation of algorithms, creation of user interfaces, and interfacing with programs written in other languages.

- The MATLAB application is built around the MATLAB scripting language. 
- Common usage of the MATLAB application involves using the Command Window as an interactive mathematical shell or executing text files containing MATLAB code.
- MATLAB supports object-oriented programming.
- MATLAB can call functions and subroutines written in the programming languages.

### R
- Environment for statistical computing and graphics.
- Used among statisticians and data miners 
- Open source programming language and software environment for statistical computing and graphics
- The capabilities of R are extended through user-created packages, which allow specialized statistical techniques, graphical devices, import/export capabilities

- The most commonly used graphical integrated development environment for R is RStudio.
- R functionality is accessible from several scripting languages such as Python,[54] Perl,[55] Ruby,[56] F#,[57] and Julia.[58]

### Python 
- Object oriented programming language with popular libraries for data analysis
- Popular in engineering
- NumPy: Library adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays. 
- SciPy: Library used for scientific computing and technical computing. builds on NumPy contains modules for optimization, linear algebra, integration, interpolation, special functions, FFT, signal and image processing, ODE solvers and other tasks common in science and engineering.
- Pandas: Library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming language.
- And more

### Note
- Different tools are good for different tasks. 
- Some will be more popular in your discipline.
- You may need to us multiple tools and combine them.

## 9. Documentation reminder
- Data preparation and analysis will likely be an iterative process.
- Workflows give a visual overview and explanation of the exact process followed across different tools.
- They can capture complex analysis processes at various levels of abstraction
	 - also provide the provenance information necessary for scientific reproducibility, 
	 - and result sharing among collaborators.
	 
- You can use the documentation tools we've already discussed to store or refer to workflows (Notebooks, README files)

Workflows formalize your process by giving a precise description of the procedure and have three components:

- Inputs
	 - information or material required
- Outputs
	- information or material produced & potentially used as input in other steps
- Transformation rules/algorithms 
	- (e.g. analyses)

Two types:

- Informal
	- You can create informal workflows describing your process and include them in your documentation.
- Formal/Executable
	- Another method you can use are formal workflows that are executable. 

## 10. Informal workflows
- Well-described version history.
- Commented scripts.
- Flowcharts.

## 11. Version history
- If you're using a version control system, you may be able to use the log or history of changes as an informal workflow.
- This depends on documenting version adequately and including information about transformation done between each version.

For example, with Git, you can export a log showing the history of your versioning (commits) and the documentation (messages you included for the new version) so it's worth making these messages meaningful.

## 12. Commented scripts
- Good coding practice encourages you to comment your scripts and describe what each part of your script is doing. 
- You can use Jupyter Notebooks for this, or any environment that you write code in. 
- Programming languages even have style guides you can refer to—like Python's PEP 8—for formatting block comments, inline comments and documentation strings.

## 13. Flow charts
- You can think of these like the general flow chart we made when thinking about the data lifecycle, 
- but filled in with more detail in the data quality control, and analysis portions.
- Showing the decisions you make and processing you conduct in detail as you work with your data.

- Powerful visual that can contain a lot of information.
- One place for an overview showing the connections between actions that may not be visible within:
	- individual commented scripts if you use multiple tools, 
	- or just from file versioning information.


- Inputs or outputs include data, metadata, or visualizations
- Analytical processes include operations that change or manipulate data in some way
- Predefined processes or subroutines specify a fixed multi-step process
- Decisions specify conditions that determine the next step in the process

## 14–15. Putting flow charts together
drawing.

- Specifies a process or computation to be executed (e.g., a software program to be executed, a web service to be invoked). 
- Steps are linked according to the data flow and dependencies among them. 

Tool: Lucid Chart in the Google Suite.

### Formal workflows
- Many tools only perform a small well-defined task, thus necessitating that several of them are joined in a pipeline to model a useful experiment.
- Due to the need to combine several tools into a single research analysis some researchers delegate technical details of workflow execution to Workflow Management Systems.
- Workflow systems exploit explicit representations made by the researcher of the complex computational processes to manage and automate execution across tools.

- The representation of workflows contain the details required to carry out each analysis step, 
	- including the use of specific execution and storage resources in distributed environments. 


Kepler [website](https://kepler-project.org)
Kepler is designed to help scien­tists, analysts, and computer programmers create, execute, and share models and analyses across a broad range of scientific and engineering disciplines.

The Kepler Project is dedicated to furthering and supporting the capabilities, use, and awareness of the free and open source, scientific workflow application, Kepler.  Kepler is designed to help scien­tists, analysts, and computer programmers create, execute, and share models and analyses across a broad range of scientific and engineering disciplines.  Kepler can operate on data stored in a variety of formats, locally and over the internet, and is an effective environment for integrating disparate software components, such as merging "R" scripts with compiled "C" code, or facilitating remote, distributed execution of models. Using Kepler's graphical user interface, users simply select and then connect pertinent analytical components and data sources to create a "scientific workflow"—an executable representation of the steps required to generate results. The Kepler software helps users share and reuse data, workflows, and compo­nents developed by the scientific community to address common needs.


Taverna [website](http://www.taverna.org.uk)
Taverna is an open source and domain-independent Workflow Management System – a suite of tools used to design and execute scientific workflows and aid in silico experimentation.


VisTrails [website](https://www.vistrails.org/index.php/Main_Page)
VisTrails is an open-source scientific workflow and provenance management system that provides support for simulations, data exploration and visualization.
https://www.vistrails.org/usersguide/v2.2/html/intro.html


## Conclusion
- Discussed preparing data for analysis and documenting data processing using workflows.
 
## References
- DataOne. "Lesson 09: Analysis and workflows" [module](https://www.dataone.org/education-modules)
- Kepler [website](https://kepler-project.org)
- Taverna [website](http://www.taverna.org.uk)
- VisTrails [website](https://www.vistrails.org/index.php/Main_Page)

