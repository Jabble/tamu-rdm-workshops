# Quality control
##  Objectives
- Define data quality control and data quality assurance
- Understand the need for quality control
- Understand how to document cleaning 

## Introduction
Strategies for preventing errors from entering a dataset
Activities to ensure quality of data before collection
Activities that involve monitoring and maintaining the quality of data during the study

## Why quality control?
- Data are dirty
- Ensure data are clean and usable
- Document caveats


QA/QC best practices

- Before data collection
Define & enforce standards
Formats
Codes
Measurement units
Metadata


- During data collection/entry
Design data storage well
Minimize number of times items that must be entered repeatedly
Use consistent terminology
Atomize data: one cell per piece of information
Document changes to data
Avoids duplicate error checking
Allows undo if necessary


- After data collection/entry
Make sure data line up in proper columns
No missing, impossible, or anomalous values
Perform statistical summaries

Look for outliers
Outliers are extreme values for a variable given the statistical model being used
The goal is not to eliminate outliers but to identify potential data contamination


## Types of errors
Errors of Commission
Incorrect or inaccurate data entered
Examples: malfunctioning instrument, mistyped data
Errors of Omission
Data or metadata not recorded
Examples: inadequate documentation, human error, anomalies in the field

Methods to look for outliers
Graphical 
Normal probability plots
Regression
Scatter plots
Maps
Subtract values from mean


## Combining data sets

## Primary and secondary data quality

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


Enable transparency and reproducibility in the integration process
Ensure others understand and can evaluate your decision making process.
Automate the integration as much as possible
Especially when integrating many datasets or large datasets

## Data cleaning and transformation
There are a number of reasons you might need to transform your data during your research project or afterwards. Unlike the earlier discussion about migrating your file format, data transformation involves computing new values from old in the actual data content.

Some transformations are purely statistical, and are used to prepare the data to fit a model. An example was given earlier of one kind of transformation - logarithmic transformation to make a skewed distribution fit on a normal (bell) curve.

Of course there are implications for decisions about which form of the data to keep for the long term, which form to share with other researchers, and how to document all changes to the data. Other units in this module cover these topics.

In survey data collected from questionnaires, multiple choice and other kinds of responses are usually coded as numbers instead of character strings. This simple type of transformation has the advantages of easing data entry if typing in paper responses and avoiding inconsistencies (e.g. typos) in data values.

Qualitative data, for example interview transcripts, may be transformed into quantitative data by applying textual coding and categorisation techniques. Such variables (subjectively derived from a human thought process rather than computed) are understandably described as categorical or nominal, and can have a certain range of statistical techniques applied to them. Variables measured at an ordinal, interval or ratio level, that is 'real' numbers where a value reflects some measurement of the concept of interest, allow for a wider range of methods of analysis.

Another reason for data transformation may be to visualise the data effectively. A simple example is converting data where there is a numerator and a denominator, from ratios to percentages in order to display on a bar chart or pie graph. 

When preparing data for display (visualisation), questions of scale and granularity arise. For example, should a line chart have daily occurences along the Y axis, or be smoothed over (averaged) to show points by week or month? The answer depends on what is worth showing in the data. Anomalies may be smoothed over at a higher level; is this desirable, to eliminate noise, or deceptive (where anomalies may be revealing)?

A number of techniques may be used to transform confidential or sensitive data so that they may be shared with other researchers. These include:
aggregation: "the combination of related categories, usually within a common branch of a hierarchy, to provide information at a broader level to that at which detailed observations are taken." (OECD definition) Geographical data are also often aggregated to a higher unit, where information is deemed sensitive or revealing (e.g. postcode unit to postcode sector).

anonymisation: cases are stripped of revealing identifiers such as name and address. Pseudonymisation is a common technique for protecting identities in qualitative data.

perturbation: a deliberate distortion is introduced at the level of tabular data cells. Population Census data are sometimes released with perturbations as a trade-off for geographical detail.

From: MANTRA "File formats and transformation" [module](http://mantra.edina.ac.uk/fileformatandtransformation/)


## Ensure basic quality control

Best Practice: 
Quality control practices are specific to the type of data being collected, but some generalities exist:

Data collected by instruments:
Values recorded by instruments should be checked to ensure they are within the sensible range of the instrument and the property being measured. Example: Concentrations cannot be < 0, and wind speed cannot exceed the maximum speed that the anemometer can record.
Analytical results:
Values measured in the laboratory should be checked to ensure that they are within the detection limit of the analytical method and are valid for what is being measured. If values are below the detection limit, they should be properly coded and qualified.
Any ancillary data used to assess data quality should be described and stored. Example: data used to compare instrument readings against known standards.
Observations (such as bird counts or plant cover):
Range checks and comparisons with historic maxima will help identify anomalous values that require further investigation.
Comparing current and past measurements help identify highly unlikely events. For example, it is unlikely that the girth of a tree will decrease from one year to the next.
Codes should be used to indicate quality of data.

Codes should be checked against the list of allowed values to validate code entries
When coded data are digitized, they should be re-checked against the original source. Double data entry, or having another person check and validate the data entered, is a good mechanism for identifying data entry errors.
Dates and times:

Ensure that dates and times are valid
Time zones should be clearly indicated (UTC or local)
Data Types:

Values should be consistent with the data type (integer, character, datetime) of the column in which they are entered. Example: 12-20-2000A should not be entered in a column of dates).
Use consistent data types in your data files. A database, for instance, will prevent entry of a string into a column identified as having integer data.
Geographic coordinates:

Map coordinates to detect errors
Description Rationale: 
Quality control procedures identify potential problems with data that could affect its use.

DataOne [website](https://www.dataone.org/best-practices/ensure-basic-quality-control)


## Consider the compatibility of the data you are integrating

Best Practice: 
The integration of multiple data sets from different sources requires that they be compatible. Methods used to create the data should be considered early in the process, to avoid problems later during attempts to integrate data sets. Note that just because data can be integrated does not necessarily mean that they should be, or that the final product can meet the needs of the study. Where possible, clearly state situations or conditions where it is and is not appropriate to use your data, and provide information (such as software used and good metadata) to make integration easier.

Description Rationale: 
When using integrated data sets, it is crucial that the data are comparable and compatible to avoid mistakes in analyses and interpretation.

Related Best Practices: 
Confirm a match between data and their description in metadata
Document steps used in data processing
Define the data model
Additional Information: 
Burley, T.E., and Peine, J.D., 2009, NBII-SAIN Data Management Toolkit, U.S. Geological Survey Open-File Report 2009-1170, 96 p. Available from: http://pubs.usgs.gov/of/2009/1170/

Examples: 
Water-quality data collected by two separate agencies may be thematically similar but may have been sampled using completely different methods. Differences in such water-quality sample methods can include equipment, sampling method protocol, and lab analysis procedures. Analysis performed on integrated water-quality data that were collected using completely different methods would likely result in questionable results.

DataOne [website](https://www.dataone.org/best-practices/consider-compatibility-data-you-are-integrating)

- Double-check the data you enter
Ensuring accuracy of your data is critical to any analysis that follows.

When transcribing data from paper records to digital representation, have at least two, but preferably more people transcribe the same data, and compare resulting digital files. At a minimum someone other than the person who originally entered the data should compare the paper records to the digital file. Disagreements can then be flagged and resolved.

In addition to transcription accuracy, data compiled from multiple sources may need review or evaluation. For instance, citizen science records such as bird photographs may have taxonomic identification that an expert may need to review and potentially revise.

Description Rationale: 
Manually entered data can suffer from a high error rate. Double data entry and/or double checking of data can dramatically improve data quality.

- Identify missing values and define missing value codes
Best Practice: 
Missing values should be handled carefully to avoid their affecting analyses. The content and structure of data tables are best maintained when consistent codes are used to indicate that a value is missing in a data field. Commonly used approaches for coding missing values include:

Use a missing value code that matches the reporting format for the specific parameter. For example, use ""-999.99"", when the reporting format is a FORTRAN-like F7.2.
For character fields, it may be appropriate to use ""Not applicable"" or ""None"" depending upon the organization of the data file.
It might be useful to use a placeholder value such as ""Pending assignment"" when compiling draft information to facilitate returning to incomplete fields.
Do not use character codes in an otherwise numeric field.
Whatever missing value is chosen, it should be used consistently throughout all data associated files and identified in the metadata and/or data description files.

Description Rationale: 
Missing values are common in environmental data and affect the interpretation, analysis and calculations. Therefore, they need to be carefully defined and properly described. In addition many instruments will automatically add missing value codes in their datastream which will have to be dealt with for storage and analysis.


- Identify outliers
Best Practice: 
Outliers may not be the result of actual observations, but rather the result of errors in data collection, data recording, or other parts of the data life cycle. The following can be used to identify outliers for closer examination:

Statistical determination:

Outliers may be detected by using Dixon’s test, Grubbs test or the Tietjen-Moore test.
Visual determination:

Box plots are useful for indicating outliers
Scatter plots help identify outliers when there is an expected pattern, such as a daily cycle
Comparison to related observations:

Difference plots for co-located data streams can show unreasonable variation between data sources. Example: Difference plots from weather stations in close proximity or from redundant sensors can be constructed.
Comparisons of two parameters that should covary can indicate data contamination. Example: Declining soil moisture and increasing temperature are likely to result in decreasing evapotranspiration.
No outliers should be removed without careful consideration and verification that they are not representing true phenomena.

Description Rationale: 
Outliers may represent data contamination, a violation of the assumptions of the study, or failure of the instrumentation. Although outliers may be valid observations it is important to identify and examine their validity.

- Identify values that are estimated
Best Practice: 
Data tables should ideally include values that were acquired in a consistent fashion. However, sometimes instruments fail and gaps appear in the records. For example, a data table representing a series of temperature measurements collected over time from a single sensor may include gaps due to power loss, sensor drift, or other factors. In such cases, it is important to document that a particular record was missing and replaced with an estimated or gap-filled value.

Specifically, whenever an original value is not available or is incorrect and is substituted with an estimated value, the method for arriving at the estimate needs to be documented at the record level. This is best done in a qualifier flag field. An example data table including a header row follows:

Day, Avg Temperature, Flag
1, 31.2, actual
2, 32.3, actual
3, 33.4, estimated
4, 35.8, actual

Description Rationale: 
Correct interpretation of the content of a data table typically depends on knowing which data values were actually recorded in the field or estimate using other approaches.

- Mark data with quality control flags
Best Practice: 
As part of any review or quality assurance of data, potential problems can be categorized systematically. For example data can be labeled as 0 for unexamined, -1 for potential problems and 1 for "good data." Some research communities have developed standard protocols; check with others in your discipline to determine if standards for data flagging already exist.

The marine community has many examples of quality control flags that can be found on the web. There does not yet seem to be standards across the marine or terrestrial communities.

Description Rationale: 
Data quality should be able to be assessed by potential data users so that any problems are identified early in a project.


## Tools for data manipulation
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

Quality control (DataONE)
Preparation for analysis (DataONE)