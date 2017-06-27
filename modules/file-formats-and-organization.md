# File formats and organization
## Objectives
- Choose appropriate file formats for data.
- Compare file naming conventions.
- Use/Design a file naming convention.

## Introduction
-  store those data sets in accessbile formats
- avoiding data loss and security incidents
- Keep organized 
	- Easier to find files
	- Focus on your working with your data

## Areas
- Digital file formats
- File storage: directory structure and file naming conventions

## Digital file formats for data
*What?*
Data formats are often closely tied to data types and arrangements.

Example: Qualitative experimental data in a tabular arrangement can be saved many formats depending on the software you use.

|Formats                             |Extensions| Library of Congress description|
|------------------------------------|----------|--------------------------------|
|Microsoft Excel spreadsheets        | .xslx    | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000398.shtml)|
|Google Spreadsheets                 | .gsheet  |								 |
|Comma-seperated values              | .csv     | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000323.shtml)|

### Preferred formats 
Reusing data in the future depends on the ability to access data. From the data management perspective, we want to think about the data lifecycle again, specifically possible sharing and preservation. For this reason, there are preferred formats for data that is intended to be accessible in the long term. 

These formats have the following features:

- non-proprietary
- open and documented standard
- unencrypted
- uncompressed
- standard character encoding (ASCII, or Unicode encoding)
- commonly used by the research community

In the case of tabular data, even if you use a spreadsheet software to ... the data, the preferred format to save, export or transform to is CSV. From Excel or Google Docs this is a built-in menu option. 


### Character encoding and internationalization
"There ain't no such thing as plain text"

"If you have a string, in memory, in a file, or in an email message, you have to know what encoding it is in or you cannot interpret it or display it to users correctly."

From: Spolsky, Joel. 2003. "The Absolute Minimum Every Software Developer Absolutely, Positively Must Know About Unicode and Character Sets (No Excuses!)"[blog](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)


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




## File naming conventions
### Useful information
BE CONSISTENT
Have conventions for naming:
(1) Directory structure
(2) Folder names
(3) File names
Always include the same information 
(e.g. date and time)
Retain the order of information
(e.g. YYYYMMDD, not MMDDYYY )

BE DESCRIPTIVE
Try to keep file and folder names under 32 characters
Within reason, Include relevant information such as:

Unique identifier (ie. Project Name or Grant # in folder name)
Project or research data name
Conditions (Lab instrument, Solvent, Temperature, etc.)
Run of experiment (sequential)
Date (in file properties too)
When using sequential numbering, make sure to use leading zeros to allow for multi-digit versions. For example, a sequence of 1-10 should be numbered 01-10; a sequence of 1-100 should be numbered 001-010-100.
No special characters: & , * % # ; * ( ) ! @$ ^ ~ ' { } [ ] ? < > - + /
Use only one period and before the file extension 
(e.g. name_paper.doc NOT name.paper.doc OR name_paper..doc)

### Strategies
Order by date
Order by type
Order by subject
Forced order by number

## Exercise
generate potential file names for your data & document your strategy 
share your strategy with a partner & hear what they came up with
volunteer to share your idea with the class

## Directory structure 




### References:
- Library Carpentry. [lesson](https://data-lessons.github.io/library-data-intro/03-foundations/)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Spolsky, Joel. 2003. "The Absolute Minimum Every Software Developer Absolutely, Positively Must Know About Unicode and Character Sets (No Excuses!)"[blog](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)

Plain text formats are your friend
Naming files sensible things is good for you and for your computers. Without structured information, our lives would be much poorer. **Examples**


|SPSS Statistics Portable File Format| .por     | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000468.shtml)|
|Extensible markup language          | .xml     | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000075.shtml)|