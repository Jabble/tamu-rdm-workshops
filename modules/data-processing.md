# Manipulating data
## Objectives
From the data management perspective, the important point here is to make sure you're aware that you will need to process and possibly transform your data. And to point out that this should be done in a manner that allows you to roll back changes if you make a mistake. Or to return to the unchanged data in case you choose to use it in a different way in the future.
## Introduction
In this module, we'll discuss common manipulations of data including some common data transformations and tools for processing data. Again, we will speak from the data management perspective and generally cover the considerations you may want to make. 

We will not get deeply into data analysis, because this will largely depend on your specific data and project. However, we will cover sawys to document your process.

## Preparing data for analysis
Typically the first step before data analysis is processing and cleaning the data. This generally involves making changes to a dataset that are aimed at preparing the data for analysis.

**Processing** could be as simple as selecting a subset of the data for analysis or presentation. It could also involve merging multiple datasets, or manipulating the data themselves so that they are more usable by a researcher or a computer program.  

A common requirement for large datasets is to reduce the amount of data in the working data file. This makes computing and handling of the dataset easier.

For example: A sensor may take a temperature measurement every 5 seconds for one year. For the study, only monthly patterns are important. We might therefore only use one data point for every 5 minutes, and the dataset would be processed to remove the extra points.

## Data transformation
The data themselves may also need to be changed, or transformed.

**Transformation** refers to making changes to data values. Transformations may be done at any point after data are gathered. They could be part of data entry, quality control, or seperate data processing steps. 

These are actions like converting data to different units, normalizing data collected by multiple people and/or instruments, or developing algorithms for converting raw data into meaningful values. 

Data transformation can involve computing new values from the actual data content, like unit conversions, linear and nonlinear algorithms

Some transformations are purely statistical, and are used to prepare the data to fit a model. An example: logarithmic transformation to make a skewed distribution fit on a normal (bell) curve.

*Show example*
For example: I'll show a simple data transformation, the string of numbers on the left is the raw output from a sensor. This can (and may need to) be transformed into the table on the right, by seperating (or parsing) out different elements. In order to make the data more understandable for humans and useful for analysis.

Survey data 
collected from questionnaires, multiple choice and other kinds of responses are usually coded as numbers instead of character strings. This simple transformation has the advantages of easing data entry if typing in paper responses and avoiding inconsistencies (e.g. typos) in data values.


Qualitative data, for example interview transcripts, may be transformed into quantitative data by applying textual coding and categorisation techniques. Such variables are described as categorical or nominal, and can have a certain range of statistical techniques applied to them. Variables measured at an ordinal, interval or ratio level, that is 'real' numbers where a value reflects some measurement of the concept of interest, allow for a wider range of methods of analysis.








A number of techniques may be used to transform confidential or sensitive data so that they may be shared with other researchers. These include:

aggregation: "the combination of related categories, usually within a common branch of a hierarchy, to provide information at a broader level to that at which detailed observations are taken." (OECD definition) Geographical data are also often aggregated to a higher unit, where information is deemed sensitive or revealing (e.g. postcode unit to postcode sector).

anonymisation: cases are stripped of revealing identifiers such as name and address. Pseudonymisation is a common technique for protecting identities in qualitative data.

perturbation: a deliberate distortion is introduced at the level of tabular data cells. Population Census data are sometimes released with perturbations as a trade-off for geographical detail.



## Data visualization
Data may also be visualized during quality control as well as for exploratory analysis.

- Visualization as a method for exploratory analysis the limitations of data and a way to communicate data and presentation
- Good practices for visualization
- A few common types of visualizations, their value and limitations and/ or appropriate use 
- Tools for visualization


Another reason for data transformation may be to visualise the data effectively. A simple example is converting data where there is a numerator and a denominator, from ratios to percentages in order to display on a bar chart or pie graph. 

When preparing data for display (visualisation), questions of scale and granularity arise. For example, should a line chart have daily occurences along the Y axis, or be smoothed over (averaged) to show points by week or month? The answer depends on what is worth showing in the data. Anomalies may be smoothed over at a higher level; is this desirable, to eliminate noise, or deceptive (where anomalies may be revealing)?

## How to document actions
The goal here is reproducibility of your workflow. You can use the documentation tools we've already discussed using documentation tools to track your data throughout the time that you work with it, and version control to help make sure that your changes are monitored and allow you to roll-back.

Now we'll talk about creating workflows that will allow you to explain your process to others in your dissertation, an article, or when sharing your data with collaborators or the community. 

You can use the documentation that you to create informal workflows describing your analysis. Another method you can use are formal workflows that are reproducible. 

- Document the changes made to data.
	- This allows you to undo them if necessary.


### Informal workflows
we talked about documentation, here's something you can do to document your analysis process

### Formal workflows
we talked about documentation, here's another something you can do to document your analysis process


## Tools for data manipulation and analysis
Tabular data

- Excel
- GoogleDocs
- OpenRefine
- NVIVO
- SAS
- SPSS
- STATA
- Matlab
- R
- Python (NumPy, SciPy, Pandas, IPython)

- Understand what data are capable of, and the limitations of data

## Conclusion

## References
- MANTRA. "File formats and transformation" [module](http://mantra.edina.ac.uk/fileformatandtransformation/)