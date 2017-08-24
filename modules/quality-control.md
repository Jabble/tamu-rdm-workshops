# Quality control
##  Objectives
- Understand the need for quality control
- Identify quality control practices

## Introduction
In this module, we'll focus on actions that prevent errors from entering or remaining in a dataset. 

The goal is to ensure the quality of the data you plan to analyze, and to identify potential problems with data that could affect its use. 

## Exercise: Maintaining quality 
- Have you worked with quality assurance or control procedures before?
- What are some actions you have taken or expect to take to maintain the quality of your data before, during, and after collection?

## Types of errors
Errors in data are common. The two types of errors that quality control actions aim to avoid are:

**Errors of Omission**

- Data or metadata not recorded.
- Examples: inadequate documentation, human error, anomalies in the field

**Errors of Commission**

- Incorrect or inaccurate data entered.
- Examples: malfunctioning instrument, mistyped data

### Video: Physical samples
Dr. Bruce Herbert on data quality assurance procedures [youtube](https://youtu.be/xy7b_6MIB4k)

2 months of data collection lost, because someone made a mistake. Happily, Dr. Herbert is now a full professor.

- What type of error was this?
- What would keep this from happening in the future?
 
## How to control quality
Quality control practices are specific to the type of data being collected. It is likely that you will use established data gathering procedures, which include processes for ensuring data quality. 

We'll highlight some practices that you may be able to incorporate during data entry, and after data entry to help ensure quality.

## During data collection and entry
Tips:

- Enforce consistent procedure and use of standards.
- Minimize number of times data must be entered. Especially if data entry this is manual.

For manual entry:

- Consider adding an automatic validation layer (as mentioned in Data gathering).
- Double check for errors.
	- Preferably using a second person.

## Example: Data transcription
Manually entered data can suffer from a high error rate. Double data entry and/or double checking of data can dramatically improve data quality.

When transcribing data from paper records to digital representation, have at least two, but preferably more people transcribe the same data, and compare resulting digital files. At a minimum someone other than the person who originally entered the data should compare the paper records to the digital file. Disagreements can then be flagged and resolved.

## After data entry
Conduct error checks

### Check data formatting
For tabular data, make sure data line up in the proper columns and rows and follow good practices for tabular data arrangement discussed in Data gathering.

### Check for valid data
This is where automatic validation can be helpful. If you use codes these can also be checked against the list of allowed values to validate code entries. When coded data are digitized, they should be re-checked against the original source.

Data Types:

For tabular data, values should be consistent with the data type (integer, character, datetime) of the column in which they are entered. 

Dates and times:

- Ensure that dates and times are written correctly.
- Time zones should be clearly indicated (UTC or local)

### Identify missing values 
Missing values are common and many instruments will automatically add special codes for missing values in their datastream.

Missing values should be handled carefully to avoid affecting analyses. Codes for missing values should be used consistently throughout all data associated files and identified in documentation.

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

#### Statistical tests
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


## How to document actions
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