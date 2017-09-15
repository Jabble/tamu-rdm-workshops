# Data collection
## Objectives
- Identify data sources. 
- Compare tabular data arrangements in spreadsheets.
- Recognize differences in plain text, spreadsheet, and database formats.
- Bonus: Understand data validation.

## Introduction
In this module, we'll focus on data entry and how to arrange data to your advantage. 
The goal is to create quality data sets that are valid, and organized to support ease of use and reuse in later stages of the data lifecycle. We'll start broadly and then get more concrete and specific. 

## Ways to gather data
What you intend to study will inform how you gather data and the types of data you gather. In order to conduct your research, you may use and combine data from different sources. These can be grouped into five main categories. The category(ies) your data comes from will affect the choices that you make throughout your data management.

- **Observational data** are captured in situ, usually outside of the lab. Common types: Survey results, sensor readings, images.
- **Experimental data** are collected under controlled conditions, typically in lab. Common types: gene sequences, spectroscopy, cell counts. 
- **Simulation data** are machine generated results of using a model to study a system. Common types: climate models, economic models.
- **Derived and Compiled data** are created from existing sources, may be integrated from multiple sources and can be of many types. Common types: compiled databases, text mining, 3D models, geospatial data. 
- **Reference data** are published (possibly peer-reviewed) or curated datasets informing research. Common types: gene sequence databanks, chemical structures, census data, spatial data portals. 

**Example**: In order to study changes in bird populations at Big Thicket National Preserve over time, I combine my own observational data with reference data from previous research projects.


<!-- ## Quantitative and qualitative data
Data are often described as quantitive or qualitative. Quantitative data are expressed numerically (interval, ratio, possibly ordinal). Qualitative data are categorical (nominal, ordinal) data expressed in natural language.

### Exercise: Qualitative or quantitative?
- The number of website visits.
- Sport preferences (football, basketball, volleyball, hockey, ping pong)
- Frequency of different hair colors.
- Responses on a scale of agreement (strongly disagree, disagree, neutral, agree, strongly agree).
- Social security numbers. -->


### Exercise: Identify your data source(s)
*Raise hands or [etherpad](https://etherpad.net/p/Data_gathering)*

- Which source(s) of data do you have past experience using, or which source(s) do you plan to use in your graduate research?
- Can those data be recreated? What are potential problems or limitations with recreating the type data from the source(s) you listed?

#### Potential Answers
- Observational: Usually irreplaceable and therefore the most important to safeguard.
- Experimental: Often reproducible, but can be expensive or time-consuming.
- Simulation: Likely to be reproducible if the model and inputs are preserved.
- Derived and Compiled data: Reproducible, but can be very expensive and time-consuming.

## Data form
What's the form of the data? Data can come in many forms, including:

- Text: field or laboratory notes, survey responses
- Numeric: tables, counts, measurements
- Audiovisual: images, sound recordings, video
- Models, computer code
- Discipline-specific: FITS in astronomy, CIF in chemistry
- Instrument-specific: equipment outputs

## Data entry
We're discussing data stored in digital media. In some cases you may prefer to gather handwritten data. Handwritten (analog) data entry is easier in some situations, for example when working in the field to gather observational data or while running experiments in a messy lab. 

However, I assume that you will at some point want to enter–-or transfer--data into a digital format for easier manipulation. 	

We'll focus on arranging data, and then discuss digital formats and software tools for data entry. Some of this may also be useful to have in mind while writting data by hand.

## Tabular data structure
The term *tabular data* refers to data arranged into tables with columns and rows. This is a popular structure, and useful for quality control and data analysis. Many software tools are excellent at working with tabular data, and these tools will allow you to easily clean, rearrange, analyze, and graph your data when you're ready to do so.

### Good practices with spreadsheets
Let's take a closer look at good practices for entering tabular data into spreadsheets.

[image](../images/tabular_data_entry-image.png)

- Rows represent observations.
- Columns represent variables.
- Cells contain data (values) for each variable in a given observation.

### Exercise: Common errors in spreadsheets
*Show tabular arrangement with errors using Excel spreadsheet software*

Let's identify the problems with this dataset and try to correct them. Although we only mention a few good practices, many errors arise due to ignoring them. 

What errors do you see with this arrangement of data? Why are they problematic, and what changes should be made?

*Live walk through making proposed changes and discussing problems*

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
- Multiple "Null" values are problematic
	- Preferably leave the cell empty and use a separate column to qualify missing value.
- Using formatting to convey information, or make the sheet look pretty,
	- raw data should be organized for ease of quality assurance and analysis,
	- expressive reformatting may be useful for later presentation. 
- Metadata (descriptions) are included in the data,
	- descriptions of the data or dataset(s) belong outside of the data structure.

From: Behlai, Christie and Pawlik, Aleksandra. "Formatting problems" Data Organization in Spreadsheets. [lesson](http://www.datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes/)

### Tips to avoid problems
The goal is to create quality data sets that are valid, and organized to support ease of use and reuse in later stages of the data lifecycle. Following good practices for tabular data arrangement will help you avoid most problems that commonly arise when working with data.

1. Add column names in the first row(s), or "header". 
	- Column names may also be called "field names", "fields", "variable names", "variables". 
2. Use descriptive column names without spaces or special characters.
	- Often, these can be the names of variables, such as "age, "gender", "frequency", "date".
3. Include one observation per row, and one variable per column.
4. Ensure that data in each column are of a single type, e.g. date, text, number.
5. Use a standard format for values in each column, e.g. unique identifiers, names, codes, dates.
6. Once gathered, leave the raw data raw. Use a copy for cleaning and analysis.

### Dealing with missing data
Preferably leave the cell empty and use a separate column to qualify missing value. Optionally,

- in numeric fields, use a distinct value such as 9999 to indicate a missing value;
- in text fields, use NA (“Not Applicable” or “Not Available”). 

### Using codes
Codes are often used for categorical variables, they may be called "dummy codes" because they have no arithmetic meaning, doesn't make sense to add or subtract them.. Such as coding smokiers and nonsmokers as 1 or 0.

This should be documented seperately, in a *Codebook*. We'll cover Codebooks when we discuss data documentation.

<!-- As we mentioned at the beginning, the aim of data entry is to prepare you for later stages of the lifecycle. *You will see more of the result of these practices in the analysis workshop.* -->
## Formats and tools
We just looked at good practices for tabular data arrangement using a spreadsheet in Microsoft Excel. We did this because spreadsheets are easy to look at and manipulate, and Microsoft Excel is a popular tool for working with data. 

But, you can use several different formats for your tabular data. We'll look more closely at using plain text, spreadsheet, and relational database formats to create and work with tabular data structures. Each of these formats has strengths and limitations. 

### "Plain text" formats
- Work best for a single tabular dataset, especially when it is simple and large.
- Easy to enter and manipulate data programmatically.
- Software-agnostic file formats:
	- Accessible to text editing software, spreadsheet software, and statistical programming environments.

*Live walk through of data entry into TextMate text editing software and saving to a CSV file format*

### Spreadsheet formats
- Work best for single or multiple tabular datasets, harder to use and maintain as complexity and size of datasets increase.
- Easy to enter and manipulate data manually.
- Provide functionality for cleaning, analyzing, and presenting data.
- Multiple file formats, based on software:
	- Microsoft Excel Spreadsheets
	- Google Sheets
	- Numbers (Mac)
	- OpenDocument Spreadsheets

*Live walk through of data entry into Excel or Google Sheets spreadsheet software and exporting to different file formats*

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
In Databases, forced typing helps to prevent errors. This is similar to validation in a spreadsheet.

*Live walk through of Excel validation functionality*

You may also prefer to use a form for data entry into a spreadsheet. This can also add a validation layer. Google forms are a simple tool for this.

*Live walk through of Google forms pushing to CSV or a Google Sheet*

## References
- Data Carpentry. "Data Organization in Spreadsheets" [lessons](http://www.datacarpentry.org/spreadsheet-ecology-lesson/)
- DataONE. "Data entry and manipulation" [modules](https://www.dataone.org/education-modules)
- DMPTool "Data Management General Guidance" [website](https://dmptool.org/dm_guidance)
- Wickham, Hadley. 2014. Tidy Data. Journal of Statistical Software, 59:10 [pre-print](/papers/tidy-data.pdf) | [publisher](http://www.jstatsoft.org/v59/i10/)
- Whitmire, Amanda. 2014. "Types, Formats & Stages of Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Coursera. https://www.coursera.org/learn/data-visualization/lecture/7yx2o/video-lesson-what-do-we-mean-by-data
## Materials
- Microsoft Excel spreadsheet with poorly formatted data for rearrangement (all students can look and work with it)
- Example data to enter in plain text editor, Excel, and Google Form. Should also be the same as in Database format.
