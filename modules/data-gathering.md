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
	- May also be called "field names", "fields", "variable names", "variables", or "headers". 
2. Use descriptive column names without spaces or special characters.
	- Often, these can be the names of variables, such as "age, "gender", "frequency", "date".
3. Include one observation per row, and one variable per column.
4. Ensure that data in each column are of a single type, e.g. date, text, number.
5. Use a standard format for values in each column, e.g. names, codes, dates.
6. Once gathered, leave the raw data raw. Use a copy for cleaning and analysis.

### Exercise: Common errors in spreadsheets
*Show tabular arrangement with errors using spreadsheet software*

Let's identify the problems with this dataset and try to correct them. Although we only mention a few good practices, many errors arise due to ignoring them. 

What errors do you see with this arrangement of data? Why are they problematic, and what changes should be made?

*Walk through making the proposed changes*

Here are all the problems with the spreadsheet:

- Multiple tables are arranged on a single sheet,
	- requires manual intervention to read, reorganize, and analyze.
- One dataset is divided into multiple tables,
	- splits data that will later need to be merged,
	- difficult to assure quality and often causes inconsistencies.
- Mulitple datasets are in a single table,
	- can be unneccessarily repetitive,
	- may cause inconsistencies.
- Variables are stored as both rows and columns,
	- confusion ensues.
- Column names include special characters,
	- some software may interpret special characters as operators.
- Values are used as column names,
	- for analysis, values are more useful within the table.
- Mulitple values are in a single cell,
	- difficult to parse (seperate) values and perform operations on the column.
- Values have inconsistent and have problematic formatting,
	- this frequently involves special characters, dates, spellings, capitalization, using spaces;
	- difficult to perform operations on the column such as filtering and sorting.
- Values include comments and units,
	- the values in a column should be of the same unit, or another column with the unit should be added. 
	- mixing types (e.g. text and numbers) makes it difficult to perform operations on the column.
- Null values are problematic
	- Preferably leave the cell empty and use a separate column to qualify missing value.
- Using formatting to convey information, or make the sheet look pretty,
	- raw data should be organized for ease of quality assurance and analysis,
	- expressive reformatting may be useful for later presentation. 
- Metadata (descriptions) are included in the data,
	- descriptions of the data or dataset(s) belong outside of the data structure.

From: Behlai, Christie and Pawlik, Aleksandra. "Formatting problems" Data Organization in Spreadsheets. [lesson](http://www.datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes/)

### Dealing with missing data
Preferably leave field empty and use a separate column to qualify missing value. Optionally:

- in numeric fields, use a distinct value such as 9999 to indicate a missing value;
- in text fields, use NA (“Not Applicable” or “Not Available”). 

### Using codes
This should be documented seperately, in a *Codebook*. We'll cover Codebooks when we discuss data documentation.

<!-- As we mentioned at the beginning, the aim of data entry is to prepare you for later stages of the lifecycle. *You will see more of the result of these practices in the analysis workshop.* -->
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
- Provide functionality for cleaning, analyzing, and presenting data.
- Multiple file formats, based on software:
	- Microsoft Excel Spreadsheets
	- Google Sheets
	- Numbers (Mac)
	- OpenDocument Spreadsheets

*Show data entry into Excel or Google Sheets and export to different file formats*

### Database formats
A database consists of 

1. a set of tables, 
2. defined relationships between tables, 
3. a command language that facilitates data manipulation. 

They're often used for storing data like financial records, medical records, manufacturing and logistical data. 

- Work best for linking large and complex datasets. 
- Easy to query datasets, select portions and combine.
- Steep learning curve and rigid in use.
- Control errors by:
	- Forced typing, meaning only integers are allowed in a column of type 'integer'
	- Maintaining record integrity, meaning columns cannot be sorted independently of each other
- Multiple file formats and models, based on software:
	- MySQL
	- Postgre SQL
	- Microsoft SQL Server
	- Microsoft Access
	- Oracle Database

*Show image of tabular data structures in a database model*

## Adding validation
In Databases, strict typing helps to prevent errors. This is similar to validation in a spreadsheet.

*Show Excel validation functionality*

You may also prefer to use a form for data entry into a spreadsheet. Google forms are a simple tool for this.

*Show Google forms pushing to CSV or Google Sheet*

## References
- Data Carpentry. "Data Organization in Spreadsheets" [lessons](http://www.datacarpentry.org/spreadsheet-ecology-lesson/)
- DataONE. "Data entry and manipulation" [modules](https://www.dataone.org/education-modules)
- Wickham, Hadley. 2014. Tidy Data. Journal of Statistical Software, 59:10 [pre-print](/papers/tidy-data.pdf) | [publisher](http://www.jstatsoft.org/v59/i10/)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Whitmire, Amanda. 2014. "Types, Formats & Stages of Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)

## Material
- Microsoft Excel spreadsheet with poorly formatted data for rearrangement (all students can look and work with it)
- Example data to enter in plain text editor, Excel, and Google Form. Should also be the same as in Database formats.