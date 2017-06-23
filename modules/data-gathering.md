# Data gathering
## Objectives
- Recognize the diversity of data types. 
- *Arrange data in text editing, spreadsheet, and database software. (digital data entry)*

## Introduction
*Bring in datalifecycle stages?*

In this module, we'll focus on data entry and how to arrange data to your advantage. The goal is to create quality data sets that are valid and organized to support ease of use and reuse. We'll start broadly and get more concrete and specific. 

## Ways to get your data
What you intend to study will inform how you gather data and the types of data you gather. In order to conduct your research, you may use different types of data in combination. 

- **Observational data** are captured in situ. Common types: Survey results, sensor readings.
- **Experimental data** are collected under controlled conditions. Common types: gene sequences, spectroscopy, cell counts. 
- **Compiled data** are integrated from multiple sources and can be of many types. Common types: compiled databases, 3D models, geospatial data. 
- **Derived data** are created from existing sources. Common types: text and data mining.
- **Simulation data** are results of using a model to study a system. Common types: climate models, economic models.
- **Reference data** are published (possibly peer-reviewed) or curated datasets informing research. Common types: gene sequence databanks, chemical structures, census data, spatial data portals. 

**Example**: In order to study changes in bird populations at Big Thicket National Preserve over time, I combine my own observational data with reference data from previous research. 

### Exercise: Identify your data
- Do you have experience with conducting research in the past? What have you done?
- What type(s) of data to you have past experience gathering, working with, or plan to gather in your graduate research?
- Can that data be recreated? What are the problems or limitations with recreating it, if it is lost?

## Data entry
We'll mainly discuss digital data. In some cases you may prefer to write your data down by hand (I'll call this analog). Analog data entry could be easier for observational data in the field or experiemental data in a messy lab. However, I'm still assuming that you will at some point want to enter, or transfer, data into a digital format for easier manipulation. We'll focus on how to arrange digital data, formats and tools for digital data entry, and tools for converting data from analog to digital. 

## Tabular data arrangements
Tabular data refers to an arrangement of data into columns and rows. 

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

*Show tabular arrangement using spreadsheet software*


## Formats and tools
We just looked at good practices for tabular data arrangement using a spreadsheet in Microsoft Excel. We did this because spreadsheets are easy to look at and manipulate, and Microsoft Excel is a good software tool for entering and manipulating datasets at this scale. But, you can use different digital formats for your tabular data. Each format has different strengths. 

We'll take a look at using plain text, spreadsheet, and relational database formats to create and work with tabular data arrangements.

### Plain text
- Best for a single tabular dataset, especially when it is simple but large.
- Easy to enter and manipulate data programmatically.
- This format is software-agnostic:
	- Possible (but difficult) to enter and manipulate data using a text editing software such as Notepad++, TextEdit, TextMate, Sublime Text, etc.
	- If correctly formatted, plain text can be opened in a spreadsheet software. You may encounter problems doing this with very large datasets.

### Spreadsheets
- The format is base on the spreadsheet software, such as Microsoft Excel or Google Sheets.
- Easy to use, but harder to maintain as complexity and size of data increase.
- Provide support for calculations and the creation of charts and graphs.
- Flexible about cell content type—cells in same column can contain numbers or text
- Lack record integrity--can sort a column independently of all others)
- Can use sheets for multiple data sets, but more difficult to link and extract data across datasets

### Relational Databases
- Best for large and complex datasets
- Easy to query to select portions of data and combine datasets
- Data fields are typed – For example, only integers are allowed in integer fields
- Columns cannot be sorted independently of each other
- Steeper learning curve than a spreadsheet
- This format depends on software for creating relational databases such as, .. .. .. 


## Let's take a look at how data entry can work with each of these.
Data entry in Google form
From the lense of one good practice, validation





### Spreadsheets
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




### Relational databases
The same good practices apply in relational databases. They're more complicated to set up, but make following some of the above practices easier. Built in.  

A database consists of a set of tables, defined relationships between them (which table is related to which other table), and also a powerful command language that facilitates data manipulation.
Here, a dataset for plant phenology has been divided into three tables, one describing site information, one describing characteristics of each sample, and one describing the plant species found.   
What they're used for: Relational databases are currently the predominant choice in storing data like financial records, medical records, personal information and manufacturing and logistical data.
Database features includes explicit control over data types and has the advantages of quality control and performance.   

A common format for working with data are Digital data entry can be done into a text editing, spreadsheet, or database software. We'll focus on these three and good practices for using them. These practices may extend to other sorts of data entry as well.




## References
- Whitmire, Amanda. 2014. "Types, Formats & Stages of Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- DataONE. "Data entry and manipulation" []()
- Data Carpentry. "Data Organization in Spreadsheets" [lessons](http://www.datacarpentry.org/spreadsheet-ecology-lesson/)