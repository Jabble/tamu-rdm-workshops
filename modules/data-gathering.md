# Data gathering
## Objectives
- Recognize the diversity of data types. 
- *Arrange data in text editing, spreadsheet, and database software. (digital data entry)*

## Introduction
*Bring in datalifecycle stages?*

In this module, we'll focus on data entry and how to use digital file formats to your advantage. The goal is to create quality data sets that are valid and organized to support ease of use and reuse, and store those data sets in accessbile formats. We'll start broadly and get more concrete and specific. 

## Types of data
Data are often divided into two categories, quantitive and qualitative. Quantitative data are expressed numerically, they are often (but not always) continuous and measurable. Qualitative data are categorical data expressed in natural language. 

### Exercise: Qualitative or Quantitative?
- Counts indicating the number of occurances.
- Sport preferences (football, basketball, volleyball, hockey, ping pong)
- Responses on a scale of agreement (strongly disagree, disagree, neutral, agree, strongly agree).
- Social security numbers.

## Categories
What you intend to study will inform the data you gather. In order to conduct your research, you may use different types of data in combination. 

- **Observational data** are captured in situ. Common types: Survey results, sensor readings.
- **Experimental data** are collected under controlled conditions. Common types: gene sequences, spectroscopy, cell counts. 
- **Compiled data** are integrated from multiple sources and can be of many types. Common types: compiled databases, 3D models, geospatial data. 
- **Derived data** are created from existing sources. Common types: text and data mining.
- **Simulation data** are results of using a model to study a system. Common types: climate models, economic models.
- **Reference data** are published (possibly peer-reviewed) or curated datasets informing research. Common types: gene sequence databanks, chemical structures, census data, spatial data portals. 

**Example**: Studying changes over time in the bird populations at Big Thicket National Preserve, I may combine my own observational data with reference data from previous research. 

### Exercise: Identify your data
- Do you have experience with conducting research in the past? What have you done?
- What type(s) of data to you have past experience gathering, working with, or plan to gather in your graduate research?
- Can that data be recreated? What are the problems or limitations with recreating it, if it is lost?

## Gathering data
We'll focus mainly on digital data entry and storage. This said, you may prefer to write your data and notes down by hand (analog), or may use both digital and anolog data entry. I'm assuming here that you will at some point want to enter or transfer those data and notes into a digital format for easier manipulation. We'll focus on data right now, and will come back to notes when we discuss documentation. 

## Data entry
Data entry can be done through a form or directly in a text editing, spreadsheet, or database software. We'll focus on these three and good practices for using them. These practices may extend to other sorts of data entry as well. 
### Tabular v. Relational

### Tabular data in spreadsheets
From: Data Carpentry. "Data Organization in Spreadsheets" [lesson](http://www.datacarpentry.org/spreadsheet-ecology-lesson/)

Spreadsheets tool for working with data that lends itself to a tabular arrangement for:

- Data entry
- Organizing data
- Subsetting and sorting data
- Statistics
- Plotting

Structuring data in spreadsheets
The cardinal rules of using spreadsheet programs for data:

Put all your variables in columns - the thing you’re measuring, like ‘weight’ or ‘temperature’.
The columns of data have consistent types.   Each column contains only numbers, dates, or text.
There are consistent names, codes, and formats used in each column. For instance, all dates are in the same format (mm/dd/yyyy), Species are all referred to by standard codes.
Put each observation in its own row.
Don’t combine multiple pieces of information in one cell. Sometimes it just seems like one thing, but think if that’s the only way you’ll want to be able to use or sort that data.
Leave the raw data raw - don’t change it!
Export the cleaned data to a text-based format like CSV (comma-separated values) format. This ensures that anyone can use the data, and is required by most data repositories.
Data are all in one table, which is much easier for a statistical program to work with than multiple small tables which each require human intervention
Create descriptive column names without spaces or special characters

Missing data
Preferably leave field empty (NULL = no value)
In numeric fields, use a distinct value such as 9999 to indicate a missing value 
In text fields, use NA (“Not Applicable” or “Not Available”)
Use Data flags in a separate column to qualify missing value


*Good data entry and poor data entry examples*

Data entry in Google form
Validation

### Relational data in databases


## References
- Whitmire, Amanda. 2014. "Types, Formats & Stages of Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- DataONE. "Data entry and manipulation" []()
- Data Carpentry. "Data Organization in Spreadsheets" [lessons](http://www.datacarpentry.org/spreadsheet-ecology-lesson/)
- Spolsky, Joel. 2003. "The Absolute Minimum Every Software Developer Absolutely, Positively Must Know About Unicode and Character Sets (No Excuses!)"[blog](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)

|SPSS Statistics Portable File Format| .por     | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000468.shtml)|
|Extensible markup language          | .xml     | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000075.shtml)|
