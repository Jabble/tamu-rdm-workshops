# Data Collection
## 3. Introduction
- In the first section today, we’ll focus on data gathering and entry, and how to arrange data to your advantage. 
- The goal is to create quality data sets that are valid, and organized to support ease of use and reuse in later stages of the data lifecycle. 
- We'll start broadly and then get more concrete and specific. 

## 4. Ways to gather data
- What you intend to study will inform how you gather data and the types of data you gather. In order to conduct your research.
- You may use and combine data from different sources. 
- Data sources grouped into five main categories:

**Observational data** are captured in situ, usually outside of the lab. 
Common types: Survey results, sensor readings, images.
**Experimental data** are collected under controlled conditions, typically in lab. 
Common types: gene sequences, spectroscopy, cell counts. 
**Simulation data** are machine generated results of using a model to study a system. 
Common types: climate models, economic models.
**Derived and Compiled data** are created from existing sources, may be integrated from multiple sources and can be of many types. 
Common types: compiled databases, text mining, 3D models, geospatial data. 
**Reference data** are published (possibly peer-reviewed) or curated datasets informing research. 
Common types: gene sequence databanks, chemical structures, census data, spatial data portals. 

### Example 
In order to study changes in bird populations at Big Thicket National Preserve over time, I might combine my own observational data with reference data from previous research projects.

## 5. Discussion
- Which source(s) of data do you have experience using, or expect to use, in your graduate research?
- Follow up question: If these data are lost, what are potential problems or limitations with recreating data from the source(s) you listed?

## 6. Reproducibility
Data from some sources may be more easily reproduced than others.

- Observational: Usually irreplaceable and important to safeguard.
- Experimental: Often reproducible, can be expensive or time-consuming.
- Simulation: Likely to be reproducible, if the model and inputs are preserved.
- Derived and compiled data: Reproducible, but can be very expensive and time-consuming.

In all cases good practices during data collection and later on, can save you from the time, effort, and embarrassment of data loss when mistakes are made and things go wrong. 

## 7. Video
- TAMU Geosciences professor, Bruce Herbert describes a situation where he lost data due to a simple error while processing physical samples (documentation was lost). 
- 2 minute video
- He was unable to recover the data, and couldn’t gather the samples again due to the time and effort needed. 
- Limitations on data reproducibility are why good quality assurance practices are important throughout the process of working with data. Starting with data gathering and entry.


## 8. Data form
The type of data you gather, enter, and work with can take many forms.

Observational, Experimental, and Simulation data might include numeric outputs, textual data, images, sound recordings, or video saved as digital files 
from:

- survey responses, 
- lab instrument measurements and sensor readings (for physical samples and laboratory specimens), 
- computer simulations and model results.

In some cases you might prefer to gather handwritten data. Handwritten (analog) data entry is easier in certain situations. For example, 

- When working in the field to gather Observational data,
- Gathering questionnare results from participants, 
- While running Experiments in a messy lab.

At some point, you will want to enter–-or transfer--data into a digital format for easier manipulation.

- It is likely that you will use established data gathering and data entry procedures for the data that you work with.
- This ought include processes for ensuring data quality and avoiding data loss. 
- Step one is to enforce a consistent procedure.

## 9. Tips to assure quality during data collection
A few personal practices during data collection and entry can help ensure quality.

## During data collection and entry
Tips:

- Think about how data collection may go wrong and enforce consistent procedure and use of standards.
- Minimize number of times data must be entered and transferred. Especially if data entry is manual.

For manual entry especially:

- Consider adding an automatic validation layer.
- Double check for errors.
	- Preferably using a second person.

### Example: Data transcription
- Manually entered data can suffer from a high error rate. 
- Double data entry and/or double checking of data can dramatically improve data quality.

One procedure you might be familiar with is using multiple people to transcribe data:

- When transcribing data from paper records to digital representation, it’s recommended to have at least two or more people transcribe the same data. Then to compare resulting digital files. 
- At a minimum someone other than the person who originally entered the data should compare the paper records to the digital file. Disagreements can then be flagged and resolved.

## 10. Tabular data structure
Some types of research data and data files are fairly ubiquitous and can be found across disciplines. 

- Images, Mapping/GIS and video are data are widely used by researchers.
- Similarly, researchers in many disciplines use spreadsheets to store, manipulate, and later visualize data. 
- Spreadsheets are a form of tabular data. 

The term *tabular data* refers to data arranged into tables with columns and rows. 
Where:

- Rows represent observations or records.
- Columns represent variables.
- Cells contain data (values) for each variable in a given observation.

## 11. Tabular data structure
- The tabular data arrangement is popular because it is useful for quality control and later data analysis. 
- Many software tools and programming languages are excellent at working with tabular data.
- These tools will later allow you to easily clean, rearrange, analyze, and graph your data when you're ready. 

Have any of you used these tools?

- Open refine: tool for working with messy data, a little like excel but more powerful for cleaninf up tabular data. Originally developed at google and now open source software. 
- R: is a free software environment for statistical computing and graphics and a popular programming language for doing stats.
- Python: is a programming language often used for data analysis. It has many packages (additions) for working with, and analyzing data.
- SPSS: Statistics is a software package used for statistical analysis, now belongs to IBM. It’s widely used in social science. Many features are accessible via pull-down menus or can be programmed with a proprietary command language.
- SAS: is a software suite to perform statistical analysis and includes the SAS language as it's programming language for statistical analysis. SAS provides a graphical point-and-click user interface for non-technical users and more advanced options through the SAS language.
- Matlab: numerical computing environment also with a proprietary programming language.

Are there other tools you use?

To many dat analysis tools effectively, you’ll need to start with valid tabular data.

We'll focus on good practices for arranging digital data in a tabular structure during your data entry, and then discuss specific digital file formats and software for working with tabular data during data entry. 

## 12. Exercise: Common errors in spreadsheets

- Let’s start with how not to arrange your data.
- The dataset at this link is from a survey. Go ahead and download it.
- Several animal species were caught, to gather data about their gender and weight at different locations, called ‘plots’. The survey was conducted over a few years.

This spreadsheet showing the data illustrates some common errors. Some are probably more obvious than others. So take a few minute to pair up to identify and discuss errors in this spreadsheet. 

See how many different problems you can identify and note with this spreadsheet. Importantly, why are they problematic, and what changes should be made?

Go ahead and try fixing the errors you've identified.

Let's identify the problems with this dataset and try to correct them together

*Live walk through making proposed changes and discussing problems*

- Multiple tables are arranged on a single sheet,
	- requires manual intervention to read, reorganize, and analyze.
- One dataset is divided into multiple tables,
	- splits data that will later need to be merged,
	- difficult to assure quality and often causes inconsistencies.
- Multiple datasets are in a single table,
	- can be unnecessarily repetitive,
	- may cause inconsistencies.
- Variables are stored as both rows and columns,
	- confusion ensues.
- Column names include special characters,
	- some software may interpret special characters as operators.
- Values are used as column names,
	- for analysis, values are more useful within the table.
- Multiple values are in a single cell,
	- difficult to parse (separate) values and perform operations on the column.
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

## 13. Tips to avoid problems
The goal is to create quality data sets that are valid, and organized to support ease of use and reuse in later stages of the data lifecycle. 
Following good practices for tabular data arrangement will help you avoid most problems that commonly arise when working with data.

1. Add column names in the first row(s), or "header". 
	- Column names may also be called "field names", "fields", "variable names", "variables". 
2. Use descriptive column names without spaces or special characters.
	- Often, these can be the names of variables, such as "age", "frequency", "date".
3. Include one observation per row, and one variable per column.
4. Ensure that data in each column are of a single type, e.g. date, text, number.
5. Use a standard format for values in each column, e.g. standard species name, unique identifier, codes, dates as YYYY-MM-DD.
6. Once gathered, leave the raw data raw. Use a copy for cleaning and analysis.

Although we only mention a few good practices, many errors like the ones in the spreadsheet we looked at before arise due to ignoring them. 

## 14. Using codes
### Dealing with missing data
You may want to leave the cell empty and use a separate column to qualify missing value. Optionally,

- In numeric fields, use a distinct value such as 9999, -999 or -9999 to indicate a missing value;
- In text fields, use NA (“Not Applicable” or “Not Available”). 
- Avoid using special characters, such as commas, semicolons, or tabs, in the data itself if the data file is in (or will be exported to) a delimited format.

### Dummy codes
Numeric codes are also often used for categorical variables. Like in a study of tobacco use: 0 for non-smoker, 1 for smoker, 2 for chewer. And 9 for not available.

These may be called "dummy codes" because they have no arithmetic meaning, doesn't make sense to add or subtract them.

### Standard codes
When possible, you should use standard codes for your discipline. Examples include using Federal Information Processing (FIPS) codes for geographic entities and the Integrated Taxonomic Information System (ITIS) for authoritative species names.

https://www.census.gov/geo/reference/codes/cou.html 
https://www.itis.gov 

The meaning of codes should be documented separately from your data table, in a *Codebook* or data dictionary. We'll discuss these in a little bit when we talk about data documentation.

When using non-standard codes, you may still define the codes in the documentation or create a supplemental table with code definitions.

## 15. Formats and tools
We just looked at good practices for tabular data arrangement using a spreadsheet in Microsoft Excel.
We did this because spreadsheets are easy to look at and manipulate, and Microsoft Excel is a popular tool for working with data. 

But, I keep using the generic phrase “tabular data” because you can use several different digital formats and software to gather and arrange your data tabularly. 

After a break, we’ll look more closely at using 

- plain text 
- spreadsheet and
- relational database formats 

to create and work with tabular data structures. Each of these formats has strengths and limitations. 

## 16. Break
5-10 min

## 17. "Plain text" format
- Work best for a single tabular dataset, especially when it is simple and large.
- Easy to enter and manipulate data programmatically.

*Talk about values in image*

## 18. "Plain text" format
- Work best for a single tabular dataset, especially when it is simple and large.
- Easy to enter and manipulate data programmatically.
- Software-agnostic file format:
	- Accessible to text editing software, spreadsheet software, and statistical programming environments.

## 19. Spreadsheet formats
- Work best for single or multiple tabular datasets. You can have multiple sheets in a single file.
- Harder to use and maintain as complexity and size of datasets increase.
- Easy to enter and manipulate data manually.
- Provide functionality for cleaning, analyzing, and presenting data within the software.

## 20. Spreadsheet formats
- Multiple file formats, based on software tool:
	- Microsoft Excel Spreadsheets
	- Google Sheets
	- Numbers (Mac)
	- OpenDocument Spreadsheets

- These formats don't alwasy play nice together. 
- In that you can't always open a document saved by one software using another software, or you might encounter some problems with the formatting. 
- This is why saving or exporting as a plain text CSV file can be a better option when sharing data and when moving across software tools. 
- Note, that plain text formats will strip any formatting that you may do in a spreadsheet software.

## 21. Database formats
- Work best for linking large and complex datasets. 
- They're often used for storing data like financial records, medical records, manufacturing and logistical data.
- Easy to query datasets, select portions and combine.
- Steep learning curve and rigid in use.
- Control errors by:
	- Forced typing, meaning only integers are allowed in a column of type 'integer'
	- Maintaining record integrity, meaning columns cannot be sorted independently of each other
	
## 22. Database formats
A database consists of 

1. a set of tables, 
2. defined relationships between tables, 
3. a command language that facilitates data manipulation. 


## 23.–25. Database formats
*Walk through database tables, SQL command language, Results*

## 26. Database formats
- Multiple file formats and models, based on software:

You may have heard of some of these. If you're looking to learn Microsoft Access is a light-weight option. MySQL is a more robust free option, but more complicated.
	- MySQL: more robust free database software, that allows multiple users.
	- Postgre SQL: Advanced open source database
	- Microsoft SQL Server: Proprietary database software
	- Microsoft Access: personal database you can run on your computer to learn.
	
## 27. Adding validation
Databases, use forced typing helps to prevent errors. 
Meaning that you would define the type of variable that goes into a column as textual, numeric, or a date in advance.

- As I mentioned briefly when talking about tips to assure quality, you may want to incorporate a layer of automatic validation during data entry to assure the quality of your
- This is especially if you manually enter data.

You can also do a few simple things using software tools like Excel or Google forms and Google sheets to add an automatic validation step.

*Live walk through of Excel validation functionality with earlier sheet*

You may also prefer to use a form for data entry into a spreadsheet. This can also add a validation layer. Google forms are a simple tool for this.

*Live walk through of Google forms pushing to CSV or a Google Sheet*


## 28. Conclusion
- Discussed data sources and reproducibility. 
- Compared tabular data arrangements in spreadsheets.
- Reviewed differences in plain text, spreadsheet, and database formats.

Do you have questions or thoughts about what we've talked about so far?

## 29. References and resources
*Go over them*
