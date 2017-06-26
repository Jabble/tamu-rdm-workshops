# Data gathering
## Objectives
- Recognize the diversity of data types. 
- Demonstrate arranging tabular data in spreadsheets.
- Validate data

## Introduction
Plan management -> **Collect and store**  -> **Assure quality** -> Analyze and present -> Share and preserve

In this module, we'll focus on data entry and how to arrange data to your advantage. The goal is to create quality data sets that are valid, and organized to support ease of use and reuse in later stages of the data lifecycle. We'll start broadly and then get more concrete and specific. 

## Ways to gather your data
What you intend to study will inform how you gather data and the types of data you gather. In order to conduct your research, you may use and combine different types of data. 

- **Observational data** are captured in situ. Common types: Survey results, sensor readings.
- **Experimental data** are collected under controlled conditions. Common types: gene sequences, spectroscopy, cell counts. 
- **Compiled data** are integrated from multiple sources and can be of many types. Common types: compiled databases, 3D models, geospatial data. 
- **Derived data** are created from existing sources. Common types: text and data mining.
- **Simulation data** are results of using a model to study a system. Common types: climate models, economic models.
- **Reference data** are published (possibly peer-reviewed) or curated datasets informing research. Common types: gene sequence databanks, chemical structures, census data, spatial data portals. 

**Example**: In order to study changes in bird populations at Big Thicket National Preserve over time, I combine my own observational data with reference data from previous research. 

### Exercise: Identify your data
- What type(s) of data do you have past experience using, or which type(s) do you plan to use in your graduate research?
- Can those data be recreated? What are potential problems or limitations with recreating the type of data you listed?

## Data entry
We're discussing data stored in digital media. In some cases you may prefer to write your data down by hand in a notebook or elsewhere, I'll call this analog data storage. 

Analog data entry can be easier for observational data in the field or experiemental data in a messy lab. However, I assume that you will want to enter, or transfer, data into a digital format for easier manipulation. 

We'll focus on arranging data, and then discuss formats and tools for data entry. Some of this may be also be useful to have in mind during analog data entry too.

## Tabular data arrangements
*Tabular data* refers to data arranged into columns and rows. This is a popular arrangement and helpful for later data analysis. Also, many software tools are excellent at working with tabuar data. These tools will allow you to easily clean, rearrange, analyze, and graph your data.

### Good practices with spreadsheets
Columns = variables, rows = observations, cells = data (values).

[image](../images/spreadsheet_observation_variable-image.png)

The following practices should help you avoid most common issues that arise when working with data.

1. Include column names (a.k.a. the header) in the first row(s).
2. Use descriptive column names without spaces or special characters.
3. Add one observation per row, and one variable per column.
4. Ensure that data in each column are of a single type, e.g. date, text, number.
5. Use a standard format for values in each column, e.g. names, codes, dates.
6. Once gathered, leave the raw data raw. Make a copy for cleaning and analysis.


### Common errors in spreadsheets
columns = variables, rows = observations, cells = data (values).


*Show tabular arrangement using spreadsheet software*

- Multiple tables in one sheet
	- Multiple small tables require human intervention
- Inconsistent and unclear column names with special characters 
	- Some software may interpret special characters as operators
- Inconsistent formatting for values, dates, site spellings, capitalizations, spaces
	 - Difficult to filter and sort and run many other operations on the data en masse.
- Mixed types in columns, multiple pieces of information in one cell.
	- Mixing text and numbers makes it difficult to do an operation on the column.

From: Behlai, Christie and Pawlik, Aleksandra. "Formatting problems" Data Organization in Spreadsheets. [lesson](http://www.datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes/)

Using multiple tables
Using multiple tabs
Not filling in zeros
Using problematic null values
Using formatting to convey information
Using formatting to make the data sheet look pretty
Placing comments or units in cells
Entering more than one piece of information in a cell
Using problematic field names
Using special characters in data
Inclusion of metadata in data table
Date formatting

### Exercise: Identify the problems
What issues do you see with this arrangement of data? And what change should be made?

*Walk through making the proposed changes*

### Good practices
These practices should help you avoid most common issues that arise when working with data.

1. Include column names (aka the header) on the first row(s).
2. Use descriptive column names without spaces or special characters.
3. Enter one observation per row, and one variable per column.
4. Ensure that data in each column are strictly of one type, e.g. date, text, number.
5. Use a standard format for values in each column, e.g. names, codes, dates.
6. Once gathered, leave the raw data raw. Make a copy for cleaning and analysis.

#### Dealing with missing data
Preferably leave field empty and use a separate column to qualify missing value. Optionally:

- in numeric fields, use a distinct value such as 9999 to indicate a missing value;
- in text fields, use NA (“Not Applicable” or “Not Available”).

Use "NULL" for no value. 

#### Using codes
This should be documented seperately, in a *Codebook*. We'll cover Codebooks when we discuss data documentation.

Now, why are these the good practices? Briefly now and you will see more in the analysis workshop. As we mentioned at the beginning, the aim of data entry is to prepare you for later stages of the lifecycle.

### Exercise: Finish arranging data
Are there additional changes we should make to the data we've been looking at?

*Finish rearranging problematic data*

## 5-minute Break

## Formats and tools
We just looked at good practices for tabular data arrangement using a spreadsheet in Microsoft Excel. We did this because spreadsheets are easy to look at and manipulate, and Microsoft Excel is a popular tool for working with data manually—one you're already likely familiar with. 

But, you can use several different formats for your tabular data. We'll now take a closer look at using plain text, spreadsheet, and relational database formats to create and work with tabular data arrangements. Each of these formats has strengths and limitations. 

### Plain text
- Works best for a single tabular dataset, especially when it is simple and large.
- Easy to enter and manipulate data programmatically.
- Software-agnostic file format:
	- Possible to enter and manipulate data using a text editing software, e.g. Notepad++, TextEdit, TextMate, Sublime Text, etc.
	- If correctly formatted, can be opened in a spreadsheet software. You may encounter problems doing this with very large datasets.

### Spreadsheet
- Works best for single or multiple tabular datasets. Hard to maintain as complexity and size of data increase.
- Easy to enter and manipulate data manually.
- Provides support for cleaning and analyzing data.
- Multiple file formats, based on software:
	- Microsoft Excel Spreadsheets
	- Google Sheets
	- Numbers (Mac)
	- OpenDocument Spreadsheets

### Database
A database consists of a set of tables, defined relationships between them, and a command language that facilitates data manipulation. What they're used for: predominant choice in storing data like financial records, medical records, manufacturing and logistical data. 

- Works best for linking large and complex datasets. 
- Easy to query datasets, select portions and combine.
- Steep learning curve and rigid use:
	- Force typing, meaning only integers are allowed in a column of type 'integer'
	- Maintain record integrity, meaning columns cannot be sorted independently of each other
- This format depends on software for creating databases:
	- MySQL
	- Postgre SQL
	- Microsoft SQL Server
	- Microsoft Access
	- Oracle Database

## Adding validation
In Databases, strict typing helps to prevent errors. This is similar to using validation in a spreadsheet.
You may also prefer to use a form for data entry

*Google forms walkthrough*

## References
- Whitmire, Amanda. 2014. "Types, Formats & Stages of Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- DataONE. "Data entry and manipulation" []()
- Data Carpentry. "Data Organization in Spreadsheets" [lessons](http://www.datacarpentry.org/spreadsheet-ecology-lesson/)

## Material
- Microsoft Excel spreadsheet with poorly formatted data for rearrangement (all students can look and work with it)
- Example data to enter in plain text editor, Excel, and Google Form.