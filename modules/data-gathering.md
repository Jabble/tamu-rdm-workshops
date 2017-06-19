# Data gathering
## Objectives
- Identify types of data and appropriate formats

## Areas
- analog and digital data gathering
- data discovery
- data entry and manipulation (DataONE)
- file formats and transformations

## Introduction
What, why and how to use file formats to your advantage.


## Types of data
Data are often divided into quantitive and qualitative. Quantitative data are expressed numerically, are often (but not always) continuous and measurable. Qualitative data are categorical data expressed in natural language. 

### Exercise: Qualitative or Quantitative?
- Counts indicating the number of occurances.
- Sport preferences (football, basketball, volleyball, hockey, ping pong)
- Responses on a scale of agreement (strongly disagree, disagree, neutral, agree, strongly agree).
- Social security numbers.

### Categories
What you intend to study will infotm the data types you gather and work with 
**Observational data** are captured in situ. Common examples: Survey results, sensor readings.
**Experimental data** are collected under controlled conditions. Common examples: gene sequences, spectroscopy, cell counts. 
**Compiled data** are integrated from multiple sources and can be of many types. Common examples: compiled databases, 3D models, geospatial data. 
**Derived data** are created from existing sources. Common examples: text and data mining.
**Simulation data** are results of using a model to study a system. Common examples: climate models, economic models.
**Reference data** are published (possibly peer-reviewed) or curated datasets informing research. Common examples: gene sequence databanks, chemical structures, census data, spatial data portals. 

### Exercise: Identify your data
- Do you have experience with conducting research in the past? What have you done?
- What type of data to you have past experience gathering, working with, or plan to gather in your graduate research?
- Can that data be recreated? What are the problems or limitations with recreating it, if it is lost?

## Gathering data
- data entry, analog and digital

### Digital formats for data
*What?*
Data formats are often closely tied to data types. Example: Qualitative, tabular, experimental data can be encoded in many formats.

|Format                            | Extension| Library of Congress description|
|------------------------------------|----------|--------------------------------|
|Microsoft Excel spreadsheets        | .xslx    | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000398.shtml)|
|Google Spreadsheets                 | .gsheet  |
|Comma seperated values              | .csv     | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000323.shtml)|
|SPSS Statistics Portable File Format| .por     | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000468.shtml)|
|Extensible markup language          | .xml     | [link](https://www.loc.gov/preservation/digital/formats/fdd/fdd000075.shtml)|


### Spreadsheets
- pros/cons
- Easy to share and to lose track


### Databases
- Easy to share and maintain consistent
- needs a manager

### Preferred formats
*Why?*

- non-proprietary
- unencrypted
- uncompressed

Moving Images: MOV, MP4
Audio: Free Lossless Audio Codec (.flac), WAVE, MP3
Quantitative: ASCII, SAS, SPSS
Geospatial: ESRI Shapefile (essential: .shp, .shx, .dbf; optional: *.prj, *.sbx, *.sbn), geo-referenced TIFF (.tif, .tfw), CAD data (.dwg), tabular GIS attribute data
Digital Images: TIFF v.6, JPEG 2000
Text: PDF/A, ASCII

<table summary="file formats">
<tbody>
<tr>
<td><strong>Textual Formats</strong></td>
<td><strong>File Extensions</strong></td>
</tr>
<tr>
<td>Acrobat PDF/A</td>
<td>.pdf</td>
</tr>
<tr>
<td>Comma-Separated Values</td>
<td>.csv</td>
</tr>
<tr>
<td>Open Office Formats</td>
<td>.odt, .ods, .odp</td>
</tr>
<tr>
<td>Plain Text (US-ASCII, UTF-8)</td>
<td>.txt</td>
</tr>
<tr>
<td>XML</td>
<td>.xml</td>
</tr>
<tr>
<td>&#160;</td>
<td>&#160;</td>
</tr>
<tr>
<td><strong>Image/Graphic Formats</strong></td>
<td><strong>File Extensions</strong></td>
</tr>
<tr>
<td>JPEG</td>
<td>.jpg</td>
</tr>
<tr>
<td>JPEG2000</td>
<td>.jp2, .jpf</td>
</tr>
<tr>
<td>PNG</td>
<td>.png</td>
</tr>
<tr>
<td>SVG 1.1 (no Java binding)</td>
<td>.svg</td>
</tr>
<tr>
<td>TIFF</td>
<td>.tif, .tiff</td>
</tr>
<tr>
<td>&#160;</td>
<td>&#160;</td>
</tr>
<tr>
<td><strong>Audio Formats</strong></td>
<td><strong>File Extensions</strong></td>
</tr>
<tr>
<td>AIFF</td>
<td>.aif, .aiff</td>
</tr>
<tr>
<td>WAVE</td>
<td>.wav</td>
</tr>
<tr>
<td>&#160;</td>
<td>&#160;</td>
</tr>
<tr>
<td><strong>Video Formats</strong></td>
<td><strong>File Extensions</strong></td>
</tr>
<tr>
<td>AVI (uncompressed)</td>
<td>.avi</td>
</tr>
<tr>
<td>Motion JPEG2000</td>
<td>.mj2, .mjp2</td>
</tr>
</tbody>
</table>


### Transformation
*How?*

### Exercise: Transform file formats

## References
Whitmire, Amanda. 2014. "Types, Formats & Stages of Data" (slides)[https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835]
Whitmire, Amanda. 2014. "Organizing Your Data" (slides)[https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835]