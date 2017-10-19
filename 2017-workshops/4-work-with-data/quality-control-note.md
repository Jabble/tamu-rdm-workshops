# Quality control
In the last few weeks we've talked a little about:

- Collecting and entering your data, 
- Ways you can document your data as you work with it, 
- and storing data and security.

Today we'll discuss working with your data more and cover two topics:

- Quality control
- Data processing

## 3. Introduction
- Focus on quality assurance and control actions that prevent errors from entering or remaining in a dataset. 
- Goal is:
	 - ensure the quality of the data you plan to analyze
	 - identify potential problems with data that could affect its use. 
- We've already mentioned quality assurance steps you can take when collecting and entering data.
	- Today we'll refer back to that discussion.

## 4. Discussion
- In your projects, what are some actions you have taken or expect to take to maintain the quality of your data before, during, and after collection?
	- Do you have procedures for data gathering an entry?
	- Do you have procedures for data cleaning and manipulation?
	
## 5. QA/QC
Quality assurance and quality control are phrases used to describe a range of activities that aim to prevent errors from entering or staying in a data set.

- We mentioned some techniques in data collection. 
- Returning to the data lifecycle, It's likely that QA/QC activities will occur in multiple parts of data lifecycle. 
- But you may also want to consider having a distinct step in your work during which you take the time to perform quality assurance and control.
- This would best be placed:
	- after you've collected your data,
	- perhaps before, or as, you begin to process you data, 
	- and before you actually analyze your data.
- Additional problems with the data may also be identified during analysis and interpretation of the data prior to manuscript preparation, 
	- Having a QA/QC step let's you identify problems early.

## 6. Reducing errors
Quality control also attempts to prevent data contamination.

- Where the result of some process or phenomenon (other than the one of interest) affects the value of a variable.

Errors in data are common. The two types of errors that quality control actions aim to avoid are:

1. Errors of Omission
- Data or metadata not recorded.
- Examples: inadequate documentation, human error, anomalies in the field or experiment.

2. Errors of Commission
- Incorrect or inaccurate data entered.
- Examples: malfunctioning instrument, mistyped data.

## 7. Collecting and entering data 
For data that you collect, follow established procedures and methodology. 

If you can, incorporate some quality assurance measures that we discussed: 

- Assign responsibility for data quality to a specific person. 
	- This may work in a lab or group setting. If you're working on your own, it'll probably be you.
- Add data validation in your spreadsheets.
- Double check for mistakes, especially during manual data entry or transcription.

## 8. Combining datasets
If the data you want to use, aren't data that you've collected, review metadata/documentation for compatibility.

You can ask some basic questions to get a sense of the expected data quality before you look deeply at the data themselves.

1. Where does the dataset come from and who made it? 
	- The data’s origin will be intimately tied to its integrity. 
	- Is it a historically reliable source? 
	- Who funds it? Is it well recognized? 
	- Is it peer reviewed? Does the source have the prerequisite skills to ensure the data’s quality? 
 
2. How and for what purpose were the data collected? 
	- Does the methodology match your data and your expectations.
	- Does the formatting and variables match or map to your data.
	- How was it coded? 

3. Is there documentation of changes made to the data after collection? 
	- Who has played a role in shaping the data?
	- How was the raw data manipulated? 
	- Has anyone changed it, combined it with other data or removed parts? 
	- If so, has this enriched the data or does it give reason to doubt the integrity of the data?

4. Have other researchers drawn conclusions from the data?
	- This may give you an indication of the strength of the data.
	- How has this data been used and how is similar data usually employed by others?
	- If others have found it valuable, it may be useful to you too.
	- If others have steered away from drawing strong conclusions, this could point to potential problems with the data.

Answering these questions provides evidence of data quality and can exposes any major red flags. 

## 9. After data collection
After collecting data and when combining datasets, especially if the data are not yours, you will also want to conduct basic error checks.

- Check data formatting
	- For tabular data, make sure data line up in the proper columns and rows and follow good practices for tabular data arrangement discussed in Data gathering.
- Check for valid data
	- Identify missing, impossible, or anomalous values
- Perform statistical summaries


## 10. Check data formatting
- use headers
- one observation per row and one variable per column
- each column of a single type

## 11. Check values
### Ensure standard dates and codes
This is where automatic validation can be helpful. 
If you use codes these can also be checked against the list of allowed values to validate code entries. 

Dates and times:

- Ensure that dates and times are written correctly.
- Time zones should be clearly indicated (UTC or local)

### Find and identify missing values with codes
- Missing values are common and should be pretty easy to identify and replace with codes if needed.
- Either as empty cells or instrument-specific codes for missing values.
- Missing values should be handled carefully to avoid affecting analyses. 
	- Consider the software you plan will use for analysis and the missing value codes those tools recognize.
- The same codes for missing values should be used consistently throughout all data associated files 
- and as always, identify them in documentation.

Common codes for missing text:

N/A
None 
Null
Not Applicable

Common codes for missing numbers:

99
-99
-999.99

### Flag values that have been estimated or gap-filled 
Sometimes instruments fail and gaps appear in data. 

For example: a data table representing a series of temperature measurements collected over time from a single sensor may include gaps due to power loss, sensor drift, or other factors. 

In such cases, The record may also need to be replaced with an **estimated** or **gap-filled** value.

Whenever an original value is not available or is incorrect, and is substituted with an estimated value, the method for arriving at the estimate needs to be documented at the record level. 

- This is best done in a **qualifier flag field**. 

Day, Avg Temperature, Flag
1, 31.2, actual
2, 32.3, actual
3, 33.4, estimated
4, 35.8, actual

## 12. Find anomalies and outliers
- Outliers are extreme values for a variable given the statistical model being used.
- It is important to find outliers and anomolies in data in order to determine whether data may be contaminated.
- No outliers should be removed without careful consideration and verification that they don't represent true phenomena.
- Outliers may be the result of valid observations, or the result of errors in data collection and data recording
- It is important to identify and examine their validity to understand why they appeared and whether it is likely similar values will continue to appear.

Three techniques for finding outliers in your data are:

- Make visual determinations. 
- Compare to related observations.
- Use statistical tests.

## 13. Visual deteminations
<!-- Another way to analyze data is by visually representing it.
Numbers in charts can be difficult to interpret but patterns can be readily apparent in a few well-chosen graphs or other visual representations.

Examples of different types of plots are scatter plots and Box-and-whisker plots, which show the statistical distribution of data.
 
On the left is a scatter plot of temperatures for the month of August. The general pattern is easily discernable, and particularly warm measurements are readily apparent.
 
On the right is a box-and whisker plot of monthly temperatures. The boxes indicate averages, and measurements far from the averages are visible as red dots outside of the error bars.
 
Plots can be used to assure the quality of data as well. They can quickly show you potential data errors such as impossible values.


Another reason for data transformation may be to visualise the data effectively.
A simple example is converting data where there is a numerator and a denominator, from ratios to percentages in order to display on a bar chart or pie graph.
When preparing data for display (visualisation), questions of scale and granularity arise. For example, should a line chart have daily occurences along the Y axis, or be smoothed over (averaged) to show points by week or month? The answer depends on what is worth showing in the data. Anomalies may be smoothed over at a higher level; is this desirable, to eliminate noise, or deceptive (where anomalies may be revealing)? -->

- Plotting or mapping your data It may help you to find anomalies. 
- This makes it much easier to compare values tha a table. 
- You can look at values relative to one another in space.

A few simple examples include:

- Scatter plots: identify outliers when there is an expected pattern.
- Box plots: identify extreme values in the tails of a distribution.
- Mapping: indicate anomalies in geographic coordinates.

What other techniques would you use? What can they show you?

1. Normal probability plot: 
- graphical technique for assessing whether or not a data set is approximately normally distributed.
- The data are plotted against a theoretical normal distribution in such a way that the points should form an approximate straight line. 
- Departures from this straight line indicate departures from normality.

[NIST](http://www.itl.nist.gov/div898/handbook/eda/section3/normprpl.htm)

2. Linear Regression
- Modeler should first determine whether or not there is an expected relationship between the variables of interest.
- Linear regression attempts to model the relationship between two variables by fitting a linear equation to observed data. 
- One variable is considered to be an explanatory variable, and the other is considered to be a dependent variable.
- A scatterplot can be a helpful tool in determining the strength of the relationship between two variables. 
- If there appears to be no association between the proposed explanatory and dependent variables (i.e., the scatterplot does not indicate any increasing or decreasing trends), then fitting a linear regression model to the data probably will not provide a useful model. 
- A valuable numerical measure of association between two variables is the correlation coefficient, 
	- A value between -1 and 1 indicating the strength of the association of the observed data for the two variables.
- After a regression line has been computed for a group of data, a point which lies far from the line (and thus has a large residual value) is known as an *outlier*. 
	- Such points may represent erroneous data, or may indicate a poorly fitting regression line. 
	- If a point lies far from the other data in the horizontal direction, it is known as an *influential observation*. 

[Yale](http://www.stat.yale.edu/Courses/1997-98/101/linreg.htm)

## 14. Related observations
- Examine reference data. 
- Create difference plots for co-located data streams.
	 - This can show unreasonable variation between data sources. 
	- Example: Difference plots from weather stations in close proximity or from redundant sensors can be constructed.
- Compare two parameters that should covary. 

## 15. Statistical tests
Outliers may be detected by using statistical tests like: 

1. Dixon's test
- Used to test for a single outlier in a univariate data set (one variable). 
- Test whether the minimum value, maximum value, or either the minimum or maximum value is an outlier.
- Primarily used for small data sets (Dataplot limits the sample to be between 3 and 30). 

[NIST](http://www.itl.nist.gov/div898/software/dataplot/refman1/auxillar/dixon.htm)

2. Grubbs test
- Also known as the maximum normed residual test.
- Used to detect a single outlier in a univariate data set that follows an approximately normal distribution.
- Grubbs' test detects one outlier at a time. This outlier is expunged from the dataset and the test is iterated until no outliers are detected.
- multiple iterations change the probabilities of detection, and the test should not be used for sample sizes of six or fewer since it frequently tags most of the points as outliers.
- If you suspect more than one outlier may be present, it is recommended that you use either:
	 - The Tietjen-Moore test, 
	 - or the generalized extreme studentized deviate test.


3. Tietjen-Moore test

- A generalization of the Grubbs test 
- Can be used to test for multiple outliers in a univariate data set. 
- As with the Grubbs test, the Tietjen-Moore test assumes that the underlying distribution follows an approximately normal distribution.
- Requires that the suspected number of outliers be specified exactly. 
- If not specified correctly, this can distort the conclusions.
- If this is not known, it is recommended that the generalized extreme studentized deviate test be used instead.

[NIST](http://www.itl.nist.gov/div898/software/dataplot/refman1/auxillar/tietjen.htm)

4. Generalized extreme Studentized deviate (ESD) test
- Used to detect one or more outliers in a univariate data set that follows an approximately normal distribution.
- Only requires that an upper bound for the suspected number of outliers be specified.

[NIST](http://www.itl.nist.gov/div898/software/dataplot/refman1/auxillar/esd.htm)

These are a few examples. You may know more or more sophisticated tests. Is there something else you would use for your data?

## 16. Examine outliers
Try to identify how these values entered the dataset to detemine if they are valid values.

1. Data collected by instruments:
- Values recorded by instruments should be within the sensible range of the instrument and the property being measured. 
	- Concentrations cannot be < 0.
	- Wind speed cannot exceed the maximum speed that the anemometer can record.
- If not, something may be wrong with the instrument.

2. Data collected by observations:
- Compare current and past measurements to identify highly unlikely, or impossible events.
- Range checks and comparisons with historic maxima will help identify the values that require further investigation.

Flag values using standard codes.

Keep values prior to analysis.

- You may want to remove outliers during your analysis.
- At this point, it is worth identifying them, but leaving them in the data in case they are important later.

## How to document actions
- For quality control and assurance, you aren't necessarily cleaning the data or preparing it for analysis yet. 
- You are simply checking if the data are valid and indicating quality control actions, and flagging issues. 
- If there are errors or anomolies, these will be handled during the preparation of the dataset for analysis, but they need to be identified and noted.

Maintaining documentation as you go along will save you having to try and think back about:

- your procedures, 
- ad hoc decisions you had to make while gathering your data, 
- and the processing you did to transform and analyze raw data. 

- Document procedures and standards you followed including:
	- Data types and formats
	- Codes and terminology
	- Measurement units
- Document the checks made to data and notes on quality.
	 - This allows you to avoid needing to duplicate the error checking process.
- Mark data with quality control flags.
	- As part of any review or quality assurance of data, potential problems can be categorized systematically. For example data can be labeled as 0 for unexamined, -1 for potential problems and 1 for "good data." 
	- Some research communities have developed standard protocols; check with others in your discipline to determine if standards for data flagging already exist.

## Conclusion
-  Reviewed the purpose of quality control actions.
- Identified common quality control practices.


## References
- DataOne. “Develop a quality assurance and quality control plan” [website](https://www.dataone.org/best-practices/develop-quality-assurance-and-quality-control-plan)
- DataOne. “Ensure basic quality control” [website](https://www.dataone.org/best-practices/ensure-basic-quality-control)
- NIST/SEMATECH. “e-Handbook of Statistical Methods” [ebook](http://www.itl.nist.gov/div898/handbook/)


