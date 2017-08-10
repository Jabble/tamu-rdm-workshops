# Quality control and assurance
##  Objectives
- Understand the need for quality control
- Identify quality control practices

## Introduction
Activities that prevent errors from entering or remaining in a dataset. These are strategies to ensure data are usable for your analysis and procedures to identify potential problems with data that could affect its use. 

From the point you decide to collect data, you'll need to consider how you will make sure the quality of the data aren't compromised.

## Exercise: Quality control procedures
- Do you already have quality control procedures?
- What are some actions you will take to maintain the quality of your data before, during, and after collection?

## Types of errors
*Note about errors being common*

**Errors of Omission**

- Data or metadata not recorded
- Examples: inadequate documentation, human error, anomalies in the field

**Errors of Commission**

- Incorrect or inaccurate data entered
- Examples: malfunctioning instrument, mistyped data

### Example: Gathering physical samples
*Bruce's high-altitude water sample story. 2 months of data collection lost, because someone else made a mistake. Happily, this person is now a full professor anyway.*

What type of error was this?
 
## How to control quality
Quality control practices are specific to the type of data being collected, but we'll highlight some practices that you may be able to use.

### Before gathering data
Define standards including:

- Formats
- Codes	
- Measurement units
- Documentation practices

### During data collection and entry
Tips:

- Think about your data organization and design your data storage.
- Enforce consistent formats, terminology, codes, measurement units.
- Minimize number of times data must be entered.
	- Especially if this is manual.
- Double check manual entry for errors.
	- Preferably using a second person.

#### Example: A quality control procedure for data transcription
Manually entered data can suffer from a high error rate. Double data entry and/or double checking of data can dramatically improve data quality.

When transcribing data from paper records to digital representation, have at least two, but preferably more people transcribe the same data, and compare resulting digital files. At a minimum someone other than the person who originally entered the data should compare the paper records to the digital file. Disagreements can then be flagged and resolved.


### After data entry
Conduct error checks, these may include: 

1. For tabular data, make sure data line up in the proper columns.
2. Check for consistency
Dates and times:

Ensure that dates and times are valid
Time zones should be clearly indicated (UTC or local)
Data Types:

Values should be consistent with the data type (integer, character, datetime) of the column in which they are entered. Example: 12-20-2000A should not be entered in a column of dates).
Use consistent data types in your data files. A database, for instance, will prevent entry of a string into a column identified as having integer data.

Codes should be checked against the list of allowed values to validate code entries
When coded data are digitized, they should be re-checked against the original source. Double data entry, or having another person check and validate the data entered, is a good mechanism for identifying data entry errors.

2. Identify missing values and assign missing value codes 
Missing values are common in environmental data and many instruments will automatically add missing value codes in their datastream which will have to be dealt with for storage and analysis.

Missing values should be handled carefully to avoid their affecting analyses. Codes for missing values should be used consistently throughout all data associated files and identified in the metadata and/or data description files. The content and structure of data tables are best maintained when consistent codes are used to indicate that a value is missing in a data field. 

Commonly used approaches for coding missing values include:
Text:
N/A
None
Null
Not Applicable

Numeric:
99
-99
-999.99

3. Identify values that are estimated
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

4. Identify anomalies and outliers
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

No missing, impossible, or anomalous values
Perform statistical summaries

Look for outliers
Data collected by instruments:
Values recorded by instruments should be checked to ensure they are within the sensible range of the instrument and the property being measured. Example: Concentrations cannot be < 0, and wind speed cannot exceed the maximum speed that the anemometer can record.

Data collected by observations:
Range checks and comparisons with historic maxima will help identify anomalous values that require further investigation.
Comparing current and past measurements help identify highly unlikely events. For example, it is unlikely that the girth of a tree will decrease from one year to the next.
Codes should be used to indicate quality of data.


Outliers are extreme values for a variable given the statistical model being used
The goal is not to eliminate outliers but to identify potential data contamination

Methods to look for outliers
Graphical 
Normal probability plots
Regression
Scatter plots
Maps
Subtract values from mean


Geographic coordinates:

Map coordinates to detect errors

### When combining data sets
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

Consider the compatibility of the data you are integrating

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

### Documenting actions
As I mentioned earlier, maintining documentation as you go along will save you having to try and think back about your procedures, ad hoc decisions you had to make while gathering your data, and the processing you did to transform and analyze raw data. 

- Document checks made to data.
	 - This allows you to avoid needing to duplicate the error checking process.
- Document the changes made to data.
	- This allows you to undo them if necessary.
- Mark data with quality control flags.
	- As part of any review or quality assurance of data, potential problems can be categorized systematically. For example data can be labeled as 0 for unexamined, -1 for potential problems and 1 for "good data." 
	- Some research communities have developed standard protocols; check with others in your discipline to determine if standards for data flagging already exist.

## References
- DataOne [website](https://www.dataone.org/best-practices/ensure-basic-quality-control)
Quality control (DataONE)
Preparation for analysis (DataONE)