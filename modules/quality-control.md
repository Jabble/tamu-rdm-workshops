# Quality control
##  Objectives
- Understand the need for quality control
- Identify quality control practices

## Introduction
- In this section we'll focus a little more on quality assurance and control actions that prevent errors from entering or remaining in a dataset. 
- The goal is to ensure the quality of the data you plan to analyze, and to identify potential problems with data that could affect its use. 
- We've already discussed some quality assurance steps you can take when collecting data and we've talked about documenting your workflow. 
- Today we'll refer back to those discussions.

## Exercise: Maintaining quality 
- What are some actions you have taken or expect to take to maintain the quality of your data before, during, and after collection?

## QA/QC
Quality assurance and quality control are phrases used to describe a range of activities that aim to prevent errors from entering or staying in a data set.

We mentioned some techniques in data collection. But quality control extends throughout the data lifecycle and you may consider it a step in and of itself.

You may have a distinct quality control step in your data lifecycle, after you've collected your data and before you begin to process and analyze your data.
But it's likely that you will actively perform quality control actions during data collection and entry, when choosing to combine datasets, and as you perform analysis.




Perform basic quality assurance and quality control on your data (see here), during data collection, entry, and analysis. Describe any conditions during collection that might affect the quality of the data. 
Identify values that are estimated, 
double-check data that are entered by hand (preferably entered by more than one person), 
and use quality level flags (see here) to indicate potential problems. 
Check the format of the data to be sure it is consistent across the data set. 
Perform statistical and graphical summaries (e.g. max/min, average, range) to check for questionable or impossible values and to identify outliers. 
Communicate data quality using either coding within the data set that indicates quality, or in the metadata or data documentation. 
Identify missing values. 
Check data using similar data sets to identify potential problems. 
Additional problems with the data may also be identified during analysis and interpretation of the data prior to manuscript preparation.

We had an example of data loss due to the lack of standards, with Dr. Herbert's water samples.

Quality control also attempts to prevent data contamination.

### Data Contamination
The result of a process or phenomenon (other than the one of interest) that affects the value of a variable.


## Types of errors
Errors in data are common. The two types of errors that quality control actions aim to avoid are:

**Errors of Omission**

- Data or metadata not recorded.
- Examples: inadequate documentation, human error, anomalies in the field

**Errors of Commission**

- Incorrect or inaccurate data entered.
- Examples: malfunctioning instrument, mistyped data

## Collecting data 
For data that you collect, you should follow established procedures and methodology. And if you can, incorporate some quality assurance measures that we discussed, like data validation and double checking for errors, especially during manual data entry.

Another technique to employ is to assign responsibility for data quality to a specific person. This may work in a lab or group setting. If you're working on your own, it'll probably be you.

If the data you use, isn't data that you've collected, you should perform some quality checks before combining it with your data or using it on it's own.

## Combining datasets

Questions to ask:
Where does the data come from and who made it? The data’s origin will be intimately tied to its integrity. 
Is it a historically reliable source? Who funds it? Is it well recognized? Is it peer reviewed? Does the source have the prerequisite skills to ensure the data’s quality? Until this point it is no different than any other source. However, data need extra steps.
 
How was the data collected? How was it coded? Is there documentation of changes made to the data after collection? If the data are a collection of data from various sources then each of those sources must be evaluated individually, and can only then be judged as a coherent, comprehensive source. This is important because data put together from multiple sources is only as good as its weakest link: if one of the central variables is fundamentally flawed, then it does not matter that the remainder of the data was properly collected and cared for. Any research and conclusions drawn from the data will be questionable.
 
One typical “shortcut” is to consider whoever compiled the data as the source rather than the original data collector.  If the compiler is recognized as a credible source, that may go some way toward lending credibility to the data, however, that may not be appropriate in many cases. If the compilation took place for the sake of another project for example, the compiler would at best have taken into account the different goals and limitations pertaining to that project when deciding whether the data set was appropriate. Subsequently deeming the data “good” for another project, with different goals and limitations, cannot fully rely on the author of the compilation.   
Where has the data been? Who has played a role in shaping it? It is important to understand how the data got this far. How was the raw data manipulated? Has anyone changed it, combined it with other data or removed parts? If so, has this enriched the data or does it give reason to doubt the integrity of the data?
How does the data spend most of its time? That is, how has this data been used and how is similar data usually employed by others? If other researchers have shied away from drawing particular conclusions from this data, it is prudent to investigate.

Answering these questions provides evidence of data quality and exposes any major red flags, helping to indicate whether data will meet a researcher’s needs. 

Use quality control techniques and transform data where needed, but there are additional questions to ask of the data.

Review metadata for compatibility of context, methods, and meaning
For what purpose was the data collected?
How was the data collected?
Is it sensible to combine these datasets?

Maintain dataset provenance
- Where did the data come from? Did you collect it, or did you get your data form another source?
- 
Document transformations
Beware of accidental duplication


## Quality control after data collection
After collecting data and especially if the data are not yours, you will also want to conduct basic error checks.

- Check data formatting
	- For tabular data, make sure data line up in the proper columns and rows and follow good practices for tabular data arrangement discussed in Data gathering.
- Check for valid data
	- Identify missing, impossible, or anomalous values
- Perform statistical summaries


### Check data formatting
- use headers
- one observation per row and one variable per column
- each column of a single type

### Check for valid data
This is where automatic validation can be helpful. If you use codes these can also be checked against the list of allowed values to validate code entries. 
When coded data are digitized, they should be re-checked against the original source.

For tabular data, values should be consistent with the data type (integer, character, datetime) of the column in which they are entered. 

Dates and times:

- Ensure that dates and times are written correctly.
- Time zones should be clearly indicated (UTC or local)

### Identify missing values 
Missing values are common and many instruments will automatically add special codes for missing values in their datastream.

Missing values should be handled carefully to avoid affecting analyses. 
Codes for missing values should be used consistently throughout all data associated files and identified in documentation.

Common codes for missing text:

- N/A
- None 
- Null
- Not Applicable

Common codes for missing numbers:

- 99
- -99
- -999.99

### Identify estimated values 
Sometimes instruments fail and gaps appear in data. 

*show visual*
For example: a data table representing a series of temperature measurements collected over time from a single sensor may include gaps due to power loss, sensor drift, or other factors. In such cases, it is important to document that a particular record was missing.

It may also need to be replaced with an **estimated** or **gap-filled** value.

Whenever an original value is not available or is incorrect, and is substituted with an estimated value, the method for arriving at the estimate needs to be documented at the record level. 

This is best done in a **qualifier flag field**. 

Day, Avg Temperature, Flag
1, 31.2, actual
2, 32.3, actual
3, 33.4, estimated
4, 35.8, actual

### Identify anomalies and outliers
Outliers are extreme values for a variable given the statistical model being used
The goal is not to eliminate outliers but to identify potential data contamination

You can use exploratory data analysis:
- frequency distribution
- graphical representaiton
- calculate center and spread 

It is important to find outliers and anomolies in data in order to determine whether data may be contaminated.

Outliers may be the result of valid observations, but it is important to identify and examine their validity. Because, they may also be the result of errors in data collection and data recording. 

No outliers should be removed without careful consideration and verification that they don't represent true phenomena.

Three techniques for finding outliers in your data are:

- Statistical tests
- Visual determinations
- Comparing to related observations

## Statistical tests
Outliers may be detected by using Dixon’s test, Grubbs test or the Tietjen-Moore test.

Summary statistics 
Subtract values from mean

#### Visual deteminations
Box plots are useful for indicating outliers

Scatter plots help identify outliers when there is an expected pattern, such as a daily cycle

Normal probability plots

Regression

Mapping geographic coordinates

#### Comparing to related observations
Compare to reference data. 

Difference plots for co-located data streams can show unreasonable variation between data sources. 

Example: Difference plots from weather stations in close proximity or from redundant sensors can be constructed.

Comparisons of two parameters that should covary can indicate data contamination. 

Example: Declining soil moisture and increasing temperature are likely to result in decreasing evapotranspiration.

### Signs that outliers may be incorrect

- Data collected by instruments:

Values recorded by instruments should be checked to ensure they are within the sensible range of the instrument and the property being measured. Example: Concentrations cannot be < 0, and wind speed cannot exceed the maximum speed that the anemometer can record.

- Data collected by observations:

Range checks and comparisons with historic maxima will help identify anomalous values that require further investigation.
Comparing current and past measurements help identify highly unlikely events. For example, it is unlikely that the girth of a tree will decrease from one year to the next.



Data collected by instruments:
Values recorded by instruments should be checked to ensure they are within the sensible range of the instrument and the property being measured. Example: Concentrations cannot be < 0, and wind speed cannot exceed the maximum speed that the anemometer can record.
Analytical results:
Values measured in the laboratory should be checked to ensure that they are within the detection limit of the analytical method and are valid for what is being measured. If values are below the detection limit, they should be properly coded and qualified.
Any ancillary data used to assess data quality should be described and stored. Example: data used to compare instrument readings against known standards.
Observations (such as bird counts or plant cover):
Range checks and comparisons with historic maxima will help identify anomalous values that require further investigation.
Comparing current and past measurements help identify highly unlikely events. For example, it is unlikely that the girth of a tree will decrease from one year to the next.

## How to document actions
For quality control and assurance, you aren't necessarily cleaning the data or preparing it for analysis yet. You are simply checking if the data are valid and indicating quality control actions, and flags. 

If there are errors or anomolies, these will be handled during the preparation of the dataset for analysis, but they need to first be identified and noted.


As I mentioned earlier, maintaining documentation as you go along will save you having to try and think back about your procedures, ad hoc decisions you had to make while gathering your data, and the processing you did to transform and analyze raw data. 

- Document procedures and standards you followed including:
	- Data types and formats
	- Codes and terminology
	- Measurement units
- Document the checks made to data.
	 - This allows you to avoid needing to duplicate the error checking process.
- Mark data with quality control flags.
	- As part of any review or quality assurance of data, potential problems can be categorized systematically. For example data can be labeled as 0 for unexamined, -1 for potential problems and 1 for "good data." 
	- Some research communities have developed standard protocols; check with others in your discipline to determine if standards for data flagging already exist.

## Conclusion
Quality assurance and quality control will help you to avoid problems with your data and to prepare your data for analysis.

## References
- DataOne [website](https://www.dataone.org/best-practices/ensure-basic-quality-control)
Quality control (DataONE)
Preparation for analysis (DataONE)