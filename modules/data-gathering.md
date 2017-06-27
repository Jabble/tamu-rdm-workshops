# Data gathering
## Objectives
- Define data types. 
- Compare tabular data arrangements in spreadsheets.
- Recognize differences in plain text, spreadsheet, and database formats.
- Understand data validation.

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
- Which type(s) of data do you have past experience using, or which type(s) do you plan to use in your graduate research?
- Can those data be recreated? What are potential problems or limitations with recreating the type of data you listed?

## Data entry
We're discussing data stored in digital media. In some cases you may prefer to gather handwritten data. Handwritten (analog) data entry is easier in some situations, for example when working in the field to gather observational data or while running experiments in a messy lab. 

However, I assume that you will at some point want to enter–-or transfer--data into a digital format for easier manipulation. 	

We'll focus on arranging data, and then discuss digital formats and software tools for data entry. Some of this may also be useful to have in mind while writting data by hand.

## Tabular data structure
The term *tabular data* refers to data arranged into columns and rows. This is a popular structure, and useful for quality control and data analysis. Many software tools are excellent at working with tabular data, and these tools will allow you to easily clean, rearrange, analyze, and graph your data when you're ready to do so.

### Good practices with spreadsheets
Let's take a closer look at good practices for entering tabular data into spreadsheets.

[image](../images/spreadsheet_observation_variable-image.png)

- Rows represent observations.
- Columns represent variables.
- Cells contain data (values) for each variable in a given observation.

Again, the goal is to create quality data sets that are valid, and organized to support ease of use and reuse in later stages of the data lifecycle. Following good practices for tabular data arrangement will help you avoid most problems that commonly arise when working with data.

1. Add column names in the first row(s). 
	- Column names may also be called "field names", "fields", "variable names" or "variables".
	- This top row(s) is also called the "header". 
2. Use descriptive column names without spaces or special characters.
	- Often, these can be the names of variables, such as "age, "gender", "frequency", "date".
3. Include one observation per row, and one variable per column.
4. Ensure that data in each column are of a single type, e.g. date, text, number.
5. Use a standard format for values in each column, e.g. names, codes, dates.
6. Once gathered, leave the raw data raw. Use a copy for cleaning and analysis.

### Exercise: Common errors in spreadsheets
*Show tabular arrangement with errors using spreadsheet software*

Let's identify the problems with this dataset and try to correct them. What errors do you see with this arrangement of data? Why are they problematic, and what changes should be made?

*Walk through making the proposed changes*

Here are all the problems with the spreadsheet:

- Using one page for multiple tables
	- Multiple small tables require human intervention
- Using multiple tables for a single dataset
	- Splits data that will later need to be merged and often leads to inconsistencies
- Using a single table for multiple datasets
	- Although not strictly problematic, it can be unneccessarily repetitive
- Using values as column names
- Using column names with special characters
	- Some software may interpret special characters as operators
- Storing variables as both rows and columns
- Using mulitple values in a single cell
	- Makes it difficult to do an operation on the column.
- Using inconsistent formatting for values. Frequently dates, spellings, capitalizations, spaces.
	- Special characters
	- Difficult to filter and sort and run many other operations on the data en masse.
- Placing comments or units in cells
	- All values in a column should be of the same unit, else another column with the unit should be added. 
	- Mixing text and numbers makes it difficult to do an operation on the column.
- Using problematic null values
- Using formatting to convey information
- Using formatting to make the data sheet look pretty
- Including metadata in data

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

But, you can use several different formats for your tabular data. We'll take a closer look at using plain text, spreadsheet, and relational database formats to create and work with tabular data structures. Each of these formats has strengths and limitations. 

### "Plain text" formats
- Work best for a single tabular dataset, especially when it is simple and large.
- Easy to enter and manipulate data programmatically.
- Software-agnostic file formats:
	- Accessible to text editing software, spreadsheet software, and statistical programming environments.

*Show data entry into TextMate text editing software and saving to a CSV file format*

### Spreadsheet formats
- Work best for single or multiple tabular datasets, harder to use and maintain as complexity and size of datasets increase.
- Easy to enter and manipulate data manually.
- Provide functionality for cleaning and analyzing data.
- Multiple file formats, based on software:
	- Microsoft Excel Spreadsheets
	- Google Sheets
	- Numbers (Mac)
	- OpenDocument Spreadsheets

*Show data entry into a Google Sheet and export to different file formats*

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

*Show tabular data structures in a database model*

## Adding validation
In Databases, strict typing helps to prevent errors. This is similar to validation in a spreadsheet.

*Show Excel validation on a column*

You may also prefer to use a form for data entry.

*Google forms walkthrough*

## References
- Data Carpentry. "Data Organization in Spreadsheets" [lessons](http://www.datacarpentry.org/spreadsheet-ecology-lesson/)
- DataONE. "Data entry and manipulation" [modules](https://www.dataone.org/education-modules)
- Wickham, Hadley. 2014. Tidy Data. Journal of Statistical Software, 59:10. DOI: 10.18637/jss.v059.i10 [pre-print](/papers/tidy-data.pdf)|[publisher](http://www.jstatsoft.org/v59/i10/)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Whitmire, Amanda. 2014. "Types, Formats & Stages of Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)

## Material
- Microsoft Excel spreadsheet with poorly formatted data for rearrangement (all students can look and work with it)
- Example data to enter in plain text editor, Excel, and Google Form.