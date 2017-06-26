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
We're discussing data stored in digital media. In some cases you may prefer to gather handwritten data. Handwritten (Analog) data entry can be easier in particular situations, for example when working in the field to gather observational data or while running experiements in a messy lab situation. 

However, I assume that you will at some point want to enter–-or transfer--data into a digital format for easier manipulation. 	

We'll focus on arranging data, and then discuss formats and tools for data entry. Some of this may be also be useful to have in mind while writting data by hand.

## Tabular data arrangements
*Tabular data* refers to data arranged into columns and rows. This is a popular arrangement of data and often helpful for later data analysis. Many software tools are excellent at working with tabuar data, and these tools will allow you to easily clean, rearrange, analyze, and graph your data when you're ready to do so.

### Good practices with spreadsheets
Let's take a closer look at good practices for a tabular data arrangement.

[image](../images/spreadsheet_observation_variable-image.png)

- Rows represent observations.
- Columns represent variables.
- Cells contain data (values) for each variable in a given observation.

Again, the goal is to create quality data sets that are valid, and organized to support ease of use and reuse in later stages of the data lifecycle. Following these 6 practices for tabular data arrangement will help you avoid most problems that commonly arise when working with data.

1. Include column names (a.k.a. the header) in the first row(s).
2. Use descriptive column names without spaces or special characters.
3. Add one observation per row, and one variable per column.
4. Ensure that data in each column are of a single type, e.g. date, text, number.
5. Use a standard format for values in each column, e.g. names, codes, dates.
6. Once gathered, leave the raw data raw. Use a copy for cleaning and analysis.

### Exercise: Common errors in spreadsheets
*Show tabular arrangement with errors using spreadsheet software*

Let's identify the problems with this dataset and try to correct them. What errors do you see with this arrangement of data? Why are they problematic? And what change should be made?

*Walk through making the proposed changes*

Here are all the problems with the spreadsheet:

- Using multiple tables
	- Multiple small tables require human intervention
- Using multiple tabs
- Not filling in zeros
- Using problematic null values
- Using formatting to convey information
- Using formatting to make the data sheet look pretty
- Placing comments or units in cells
	- Mixing text and numbers makes it difficult to do an operation on the column.
- Entering more than one piece of information in a cell
	- Makes it difficult to do an operation on the column.
- Using problematic field (column) names
	- Some software may interpret special characters as operators
- Using special characters in data
- Inclusion of metadata in data table
- Inconsistent formatting for values, dates, site spellings, capitalizations, spaces
	 - Difficult to filter and sort and run many other operations on the data en masse.

From: Behlai, Christie and Pawlik, Aleksandra. "Formatting problems" Data Organization in Spreadsheets. [lesson](http://www.datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes/)

### Dealing with missing data
Preferably leave field empty and use a separate column to qualify missing value. Optionally:

- in numeric fields, use a distinct value such as 9999 to indicate a missing value;
- in text fields, use NA (“Not Applicable” or “Not Available”).

Use "NULL" for no value. 

### Using codes
This should be documented seperately, in a *Codebook*. We'll cover Codebooks when we discuss data documentation.

Now, why are these the good practices? Briefly now and you will see more in the analysis workshop. As we mentioned at the beginning, the aim of data entry is to prepare you for later stages of the lifecycle.

## Formats and tools
We just looked at good practices for tabular data arrangement using a spreadsheet in Microsoft Excel. We did this because spreadsheets are easy to look at and manipulate, and Microsoft Excel is a popular tool for working with data. 

But, you can use several different formats for your tabular data. We'll take a closer look at using plain text, spreadsheet, and relational database formats to create and work with tabular data arrangements. Each of these formats has strengths and limitations. 

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
In Databases, strict typing helps to prevent errors. This is similar to validation in a spreadsheet.
You may also prefer to use a form for data entry

*Google forms walkthrough*

## References
- Data Carpentry. "Data Organization in Spreadsheets" [lessons](http://www.datacarpentry.org/spreadsheet-ecology-lesson/)
- DataONE. "Data entry and manipulation" [modules](https://www.dataone.org/education-modules)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Whitmire, Amanda. 2014. "Types, Formats & Stages of Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)

## Material
- Microsoft Excel spreadsheet with poorly formatted data for rearrangement (all students can look and work with it)
- Example data to enter in plain text editor, Excel, and Google Form.