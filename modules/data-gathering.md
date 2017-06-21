# Data gathering
## Objectives
- Awareness for the diversity of data types. 
- Identify appropriate data formats.

## Introduction
What, why and how to use file formats to your advantage.

Create quality data sets that are:
Valid
Organized to support ease of use and reuse

## Types of data
Data are often divided into two categories, quantitive and qualitative. Quantitative data are expressed numerically, they are often (but not always) continuous and measurable. Qualitative data are categorical data expressed in natural language. 

### Exercise: Qualitative or Quantitative?
- Counts indicating the number of occurances.
- Sport preferences (football, basketball, volleyball, hockey, ping pong)
- Responses on a scale of agreement (strongly disagree, disagree, neutral, agree, strongly agree).
- Social security numbers.

## Categories
What you intend to study will inform the data used.

- **Observational data** are captured in situ. Common types: Survey results, sensor readings.
- **Experimental data** are collected under controlled conditions. Common types: gene sequences, spectroscopy, cell counts. 
- **Compiled data** are integrated from multiple sources and can be of many types. Common types: compiled databases, 3D models, geospatial data. 
- **Derived data** are created from existing sources. Common types: text and data mining.
- **Simulation data** are results of using a model to study a system. Common types: climate models, economic models.
- **Reference data** are published (possibly peer-reviewed) or curated datasets informing research. Common types: gene sequence databanks, chemical structures, census data, spatial data portals. 

### Exercise: Identify your data
- Do you have experience with conducting research in the past? What have you done?
- What type(s) of data to you have past experience gathering, working with, or plan to gather in your graduate research?
- Can that data be recreated? What are the problems or limitations with recreating it, if it is lost?

## Gathering data
- data entry

### Analog v. Digital
We'll focus mainly on digital data data entry

### Tabular v. Relational

### Tabular data in spreadsheets
From: Data Carpentry. "Data Organization in Spreadsheets" [lessons](http://www.datacarpentry.org/spreadsheet-ecology-lesson/)

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

## Digital file formats for data
*What?*
Data formats are often closely tied to data types and arrangements.

Example: Qualitative experimental data in a tabular arrangement can be saved many formats depending on the software you use.

|Formats                             |Extensions| Library of Congress description|
|------------------------------------|----------|--------------------------------|
|Microsoft Excel spreadsheets        | .xslx    | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000398.shtml)|
|Google Spreadsheets                 | .gsheet  | |
|Comma-seperated values              | .csv     | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000323.shtml)|

### Preferred formats
*Why?*

- non-proprietary
- open and documented standard
- unencrypted
- uncompressed
- standard character representation (ASCII, Unicode)
- commonly used by the research community

### Excercise:



Moving Images: MOV, MP4
Quantitative: ASCII, SAS, SPSS
Geospatial: ESRI Shapefile (essential: .shp, .shx, .dbf; optional: *.prj, *.sbx, *.sbn), geo-referenced TIFF (.tif, .tfw), CAD data (.dwg), tabular GIS attribute data

Text: PDF/A, ASCII

|Textual Formats|File Extensions|
|---|---|
|Acrobat PDF/A|.pdf|
|Comma-Separated Values|.csv|
|Open Office Formats|.odt, .ods, .odp|
|Plain Text (US-ASCII, UTF-8)|.txt|
|XML|.xml|

|Image/Graphic Formats|File Extensions|
|---|---|
|JPEG|.jpg|
|JPEG2000|.jp2, .jpf|
|PNG|.png|
|SVG 1.1 (no Java binding)|.svg|
|TIFF|.tif, .tiff|

|Audio Formats|File Extensions|
|---|---|
|AIFF|.aif, .aiff|
|Free Lossless Audio Codec|.flac|
|WAVE|.wav|

|Video Formats|File Extensions|
|---|---|
|AVI (uncompressed)|.avi|
|Motion JPEG2000|.mj2, .mjp2|

For the curious, the Library of Congress makes digital format descriptions available on their [website](https://www.loc.gov/preservation/digital/formats/fdd/descriptions.shtml).

### Transformation
*How?*

You may need to transform your data as part of working with it, when sharing with collaborators, externally, or for preservation purposes.
Analog to digital
Proprietary to non-proprietary
Why not move from compressed to uncompressed?

### Exercise: Transform file formats




## References
- Whitmire, Amanda. 2014. "Types, Formats & Stages of Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- DataONE. "Data entry and manipulation" []()
- Data Carpentry. "Data Organization in Spreadsheets" [lessons](http://www.datacarpentry.org/spreadsheet-ecology-lesson/)


|SPSS Statistics Portable File Format| .por     | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000468.shtml)|
|Extensible markup language          | .xml     | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000075.shtml)|
