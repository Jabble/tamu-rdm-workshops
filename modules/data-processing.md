# Manipulating data
## Objectives


From the data management perspective, the important point here is to make sure you're aware that you will need to process and possibly transform your data. 
And to point out that this should be done in a manner that allows you to roll back changes if you make a mistake. 
 Or to return to the unchanged data in case you choose to use it in a different way in the future.

## 3. Introduction
- In addition to QA/QC tasks, you will need to do some data processessing as you prepare and analyze your data.
- We'll talk about common manipulations of data including some common data transformations and tools for processing data.
- We won't get deeply into data analysis, because this will largely depend on your specific data and project. 
- However, we will cover ways to document your process.
- Process your data in a manner that allows you to roll back changes if you make a mistake.

## 4. Preparing data for analysis
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

## 5.  Data transformation
**Transformation** refers to making changes to data values. 
Transformations may be done at any point after data are gathered. 
They could be part of data entry, quality control, or seperate data processing steps. 

These are actions like:

- Converting data to different units, 
- Normalizing data collected by multiple people and/or instruments, 
- Or developing algorithms for converting raw data into meaningful values. 

Some transformations are purely statistical, and are used to prepare the data to fit a model. 
An example: logarithmic transformation to make a skewed distribution fit on a normal (bell) curve.

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

## 6. De-identification and anonymization
- De-identification of data refers to the process of removing or obscuring any personally identifiable information from individual records in a way that minimizes the risk of unintended disclosure of the identity of individuals and information about them. 
- The Specific steps and methods used to de-identify information will vary depending on the circumstances, 
	- Should be appropriate to protect the confidentiality of the individuals. 

It is important to note that PII may include not only direct idenfiers, such as:
- names
- ID numbers
- social security numbers

But also any other sensitive and non-sensitive informtion that:  
- Slone or combined with other information that is linked or linkable to a specific individual, and would allow identification. 

Simple removal of direct identifiers from the data to be released DOES NOT constitute adequate de-identificatioon. 
Properly performed de-identification involves removing or obscuring all identifiable information until all data that can lead to individual identifocation have been expunged or masked.


A number of techniques may be used to transform confidential or sensitive data so that they may be shared with other researchers. These include:

- Aggregation: "the combination of related categories, usually within a common branch of a hierarchy, to provide information at a broader level to that at which detailed observations are taken." (OECD definition) Geographical data are also often aggregated to a higher unit, where information is deemed sensitive or revealing (e.g. postcode unit to postcode sector).
- Perturbation: a deliberate distortion is introduced at the level of tabular data cells. Population Census data are sometimes released with perturbations as a trade-off for geographical detail.
- Anonymisation: cases are stripped of revealing identifiers such as name and address. Pseudonymisation is a common technique for protecting identities in qualitative data.

### Anonymyzation
Anonymization of data refers to the process of data de-identification that produces data where individual records cannot be linked back to an original as they do not include the required translation variables to do so.

Remove direct identifiers
Names, addresses, institutions, photos

Reduce the precision/detail through aggregation
Birth year/decade for date of birth, region rather than town

Generalize meaning of detailed text variable
Occupational expertise vs. specific position

Restrict upper or lower ranges to hide outliers
Income, age – grouped into wider categories

Combine variables
Aggregated urban/rural location description from individual place names


THIS SLIDE ADDRESSES A CONCERN PARTICULAR TO QUALITATIVE DATA.

Digital manipulation of audio and image files can remove personal identifiers 
Voice alteration, image blurring (e.g., of faces)
However, this is labor intensive, expensive and can damage research potential of data
Better solution: 
Obtain consent to use and share unaltered data for research purposes (potentially with some access conditions)
Avoid mentioning information that discloses identity during audio recording

Avoid blanking out: use pseudonyms or replacements
Identify where you have used replacements, for example with [brackets]

Avoid over-anonymization
Removing / aggregating information can make the data more difficult to interpret, distort them, or make them misleading or unusable

Exercise additional care if working as a team
Maintain consistency within the team and throughout the project

Keep master log of ALL replacements/ aggregations/ removals made and keep in a secure location separate from the anonymized data files
This is part of your documentation.


From QDR [website](https://qdr.syr.edu/guidance/teaching)


## Data analysis
Conducted via personal computer, grid, cloud computing
Statistics, model runs, parameter estimations, graphs/plots etc.

The types of analyses, software, and hardware used by ecologists and environmental scientists vary widely.  Personal computers are commonly used to perform these analyses. Other computational tools are grid and cloud computing.
 
Grid computing integrates large-scale resources such as computational devices, data applications, and scientific instruments to understand and explore research questions efficiently. It is also commonly used to share, manage, and process large datasets in physics, geophysics, astronomy, and bioinformatics.  
 
Cloud computing is location-independent computing, whereby shared servers provide resources, software, and data to a various number of external computers located elsewhere.
 
Examples of data analyses that might be used with any of these computational tools are statistics, model runs and simulations, parameter estimations, plotting of spatial data, or visualizations such as graphs. The types of analyses vary widely both among and within scientific areas of study.

## Data visualization
Data may also be visualized during quality control as well as for exploratory analysis.

- Visualization as a method for exploratory analysis the limitations of data and a way to communicate data and presentation
- Good practices for visualization
- A few common types of visualizations, their value and limitations and/ or appropriate use 
- Tools for visualization


Another way to analyze data is by visually representing it.  Numbers in charts can be difficult to interpret but patterns can be readily apparent in a few well-chosen graphs or other visual representations.
 
Examples of different types of plots are scatter plots and Box-and-whisker plots, which show the statistical distribution of data. 
 
On the left is a scatter plot of temperatures for the month of August. The general pattern is easily discernable, and particularly warm measurements are readily apparent.
 
On the right is a box-and whisker plot of monthly temperatures. The boxes indicate averages, and measurements far from the averages are visible as red dots outside of the error bars.
 
Plots can be used to assure the quality of data as well. They can quickly show you potential data errors such as impossible values.


Another reason for data transformation may be to visualise the data effectively. A simple example is converting data where there is a numerator and a denominator, from ratios to percentages in order to display on a bar chart or pie graph. 

When preparing data for display (visualisation), questions of scale and granularity arise. For example, should a line chart have daily occurences along the Y axis, or be smoothed over (averaged) to show points by week or month? The answer depends on what is worth showing in the data. Anomalies may be smoothed over at a higher level; is this desirable, to eliminate noise, or deceptive (where anomalies may be revealing)?



## Statistics
Statistical analyses
    Conventional statistics
Experimental data
Examples: ANOVA, MANOVA, linear  and 
nonlinear regression
Rely on assumptions: random 
    sampling, random & normally 
    distributed error, independent error  
    terms, homogeneous variance
     Descriptive statistics
Observational or descriptive data
Examples: diversity indices, cluster 
analysis, quadrant variance, distance methods, 
principal component analysis, correspondence analysis

Statistical analyses (continued)
Temporal analyses: time series
Spatial analyses: for spatial autocorrelation
Nonparametric approaches useful when conventional assumptions violated or underlying distribution unknown
Other misc. analyses: risk assessment, generalized linear models, mixed models, etc.
Analyses of very large datasets
Data mining & discovery
Online data processing

Statistics are among the most common types of analyses performed on data. 

There are many different types of statistical analyses, only a few of which we show here.  

Conventional statistics are often used to understand experimental data. 
The most common types are analysis of variance (ANOVA), multivariate analysis of variance (MANOVA), and regressions. 
Conventional statistics tend to rely on assumptions such as random error and homogeneous variance. 

Descriptive statistics are traditionally applied to observational or descriptive data. 
Descriptive data might include the distribution of organisms in space, species-abundance relationships, inter-specific associations, community structure, similarity or dissimilarity, and community-habitat relationships. 
Statistics used to understand these types of data include diversity indices, cluster analysis, and principle components analysis, among many others.

Statistical analyses might also include temporal or spatial analyses, and nonparametric approaches which do not rely on specific assumptions about the data’s distribution, and many other types of analysis, including risk assessment and GLM’s.

Analyzing very large datasets requires special considerations.  The process can often be broken into two steps. 
The first involves discovering and mining for the data of interest. This is typically done via computers and involves pattern searching and the use of decision trees.
The second step involves online data processing. Large datasets can be analyzed using high-performance computing systems such as cloud computing.

## Using workflows to document actions
This will likely be an iterative process of analysis and visualization.

Can occur within your existing documentation tools. Your notes, your readme files.

The goal here is reproducibility of your workflow.
 You can use the documentation tools we've already discussed using documentation tools to track your data throughout the time that you work with it, and version control to help make sure that your changes are monitored and allow you to roll-back.

Now we'll talk about creating workflows that will allow you to explain your process to others in your dissertation, an article, or when sharing your data with collaborators or the community. 

Workflows formalize your process by giving a precise description of the procedure.

Three components:

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
	- Another method you can use are formal workflows that are reproducible. 


workflow specifies a process or computation to be executed (e.g., a software program to be executed, a web service to be invoked). The steps are linked according to the data flow and dependencies among them. The representation of these computational workflows contain many details required to carry out each analysis step, including the use of specific execution and storage resources in distributed environments, Workflow systems can exploit these explicit representations of the complex computational processes to manage their lifecycle and to automate their execution. Workflows can capture complex analysis processes at various levels of abstraction, and also provide the provenance information necessary for scientific reproducibility, result publication, and result sharing among collaborators.

### Informal workflows
flowcharts (powerful visual that can contain a lot of information in one place and show the connections between actions that may not be visible within one script if you use multiple tools, or just from version information. Overview.), commented scripts, well documented version history.

we talked about documentation, here's something you can do to document your analysis process

Inputs or outputs include data, metadata, or visualizations

Analytical processes include operations that change or manipulate data in some way

Decisions specify conditions that determine the next step in the process

Predefined processes or subroutines specify a fixed multi-step process

Could create one based on you version control. For example, with Git, you can export a log showing the history of your versioning (commits) and the documentation (messages you included for the new version) so it's worth making these messages meaningful.


### Putting them together
drawing
lucid chart.

### Formal workflows

we talked about documentation, here's another something you can do to document your analysis process

SHow executable workflow in Jupyter Notebook.

Many tools only perform a small well-defined task, thus necessitating that several of them are joined in a pipeline to model a useful experiment.
The need to combine several tools into a single research analysis still holds, but technical details of workflow execution are now delegated to Workflow Management Systems.

Kepler [website](https://kepler-project.org)
Kepler is designed to help scien­tists, analysts, and computer programmers create, execute, and share models and analyses across a broad range of scientific and engineering disciplines.

The Kepler Project is dedicated to furthering and supporting the capabilities, use, and awareness of the free and open source, scientific workflow application, Kepler.  Kepler is designed to help scien­tists, analysts, and computer programmers create, execute, and share models and analyses across a broad range of scientific and engineering disciplines.  Kepler can operate on data stored in a variety of formats, locally and over the internet, and is an effective environment for integrating disparate software components, such as merging "R" scripts with compiled "C" code, or facilitating remote, distributed execution of models. Using Kepler's graphical user interface, users simply select and then connect pertinent analytical components and data sources to create a "scientific workflow"—an executable representation of the steps required to generate results. The Kepler software helps users share and reuse data, workflows, and compo­nents developed by the scientific community to address common needs.


Taverna [website](http://www.taverna.org.uk)
Taverna is an open source and domain-independent Workflow Management System – a suite of tools used to design and execute scientific workflows and aid in silico experimentation.


VisTrails [website](https://www.vistrails.org/index.php/Main_Page)
VisTrails is an open-source scientific workflow and provenance management system that provides support for simulations, data exploration and visualization.
https://www.vistrails.org/usersguide/v2.2/html/intro.html

## Tools for data manipulation and analysis
Tabular data

Excel
GoogleDocs
OpenRefine
NVIVO
SAS
SPSS
STATA
Matlab
R
Python (NumPy, SciPy, Pandas, IPython)

Understand what data are capable of, and the limitations of data




## Conclusion

## References
- MANTRA. "File formats and transformation" [module](http://mantra.edina.ac.uk/fileformatandtransformation/)
- Gil, Y. et al. (2007) Examining the Challenges of Scientific Workflows. IEEE Computer, 40, (12), 26-34. Accepted version: http://eprints.soton.ac.uk/271187/1/computer07.pdf
