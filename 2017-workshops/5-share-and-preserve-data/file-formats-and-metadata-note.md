# File formats and metadata
## Introduction
In this module, we'll look at converting data into different file formats, and taking advantage of your data documentation to create metadata that describe you data files. 
The goal is to ensure your data are useful when shared with others. 

## Exercise
- What kind of files you are likely to work with in your research? 
- We talked a lot about spreadsheets. 
- Will you also have code, audio, video, etc?
- Do you know how these files are saved?

## File formats for data
- The file format you choose for your data is a primary factor in someone else's ability to access it in the future. 
- Think carefully about what file format will be best to manage, share, and preserve your data. 
- Technology continually changes and all contemporary hardware and software should be expected to become obsolete. 
- Consider how your data will be read if the software used to produce it becomes unavailable. 
- Although any file format you choose today may become unreadable in the future, some formats are more likely to be readable than others.

Formats likely to be accessible in the future are:

- Non-proprietary
- Open, with documented standards
- In common usage by the research community
- Using standard character encodings (i.e., ASCII, UTF-8)
- Uncompressed (space permitting)

## Recommended formats
Examples of preferred format choices for data sharing, and especially for long-term preservation:


Containers: TAR, GZIP, ZIP
Databases: XML, CSV 
Geospatial: SHP, DBF, GeoTIFF, NetCDF
Moving Images: MOV, MPEG, AVI, MXF
Audio: WAVE, AIFF, MP3, MXF
Numbers/statistics: ASCII, DTA, POR, SAS, SAV
Images: TIFF, JPEG 2000, PDF, PNG, GIF, BMP
Text: PDF/A, HTML, ASCII, XML, TXT (UTF-8)
Web Archive: WARC

## Alternatives
Examples of discouraged format choices and better alternatives:

Discouraged Format	Alternative Format
Excel (.xls, .xlsx)	Comma Separated Values (.csv)
Word (.doc, .docx)	plain text (.txt), or if formatting is needed, PDF/A (.pdf)
PowerPoint (.ppt, .pptx)	PDF/A (.pdf)
Photoshop (.psd)	TIFF (.tif, .tiff)
Quicktime (.mov)	MPEG-4 (.mp4)
Binary database formats

- If you find it necessary or convenient to work with data in a proprietary/discouraged file format, do so, 
- but consider saving your work in a more archival format when you are finished.


## Tabular data

Tabular data warrants special mention because it is so common across disciplines, mostly as Excel spreadsheets. 
If you do your analysis in Excel, you should use the "Save As..." command to export your work to .csv format when you are done. 
Your spreadsheets will be easier to understand and to export if you follow best practices when you set them up, such as:


Encrypted data may be effectively lost if it was encrypted with a key that has been lost (e.g., a forgotten password). For this reason, encrypted data representations are strongly discouraged.
Data that is legally encumbered may also be considered lost. So may data bound by ambiguous or unknown access and archiving rights, because the cost of clarifying the rights situation is often prohibitive. See data rights and licensing for guidance.

From: DMPTool "Data Management General Guidance" [website](https://dmptool.org/dm_guidance)

 file format is a way of encoding information within a computer file. A program or application must be able to recognise the file format in order to access data within the file. 

For example, a web browser is able to process and display a file in the HTML (hyper-text markup language) file format so that it appears as a Web page. If the browser encounters another filetype, it may need to call on a special plug-in to view it, or it may simply let you download the file to view in another program if it cannot recognise it.

A particular file format is often indicated as part of a file's name by a file name extension, or suffix. Conventionally, the extension follows a dot in the filename and contains three or four letters that identify the format (.jpg or .jpeg). 

In the Windows operating systems you can choose to display file suffixes or not. ("Hide extensions for known filetypes" is the default option in Windows Explorer, which can be reversed in order to see file extensions.) Macintosh files often do not have a suffix, which can be a problem when copied to another system to use.

Files in proprietary formats usually must be opened by the software in which they were created. Someone without a licence to the software may not be able to open the file at all. Open formats, in which the software company or collective publishes the format rather than keeps it proprietary, are more likely to be readable by more than one application. Adobe PDF is an example of an open format that may be viewed in a number of applications, not just Adobe products.

Filetypes are based on either text or binary encoding. 

Text files are machine-readable through a character encoding standard such as ASCII or Unicode. Binary files can only be read by applicable software, and may be proprietary. Only binary formats can be executed. Some files may contain both binary and text (such as Rich Text Format - .rtf files). 

A great advantage of creating or saving research data in a text format, where possible, is that such files can be read in by a plain text editor--like Windows Notepad -- and are human readable. They can be opened in any operating system, and by a wide range of applications. Therefore, text files are the most unlikely to become obsolete over time, and are a good format for sharing and long-term preservation.

Well-known file extensions of 'plain text' are .txt, .csv, .asc, .html and .xml. 

Most software applications offer export or exchange formats that allow a text-formatted file to be created for importing into another program. 

A typical example is Microsoft Excel, which through the Save As command, can save spreadsheet data in comma delimited format (.csv or comma separated values). The structure of the rows and columns is preserved through commas and line returns. However, multiple worksheets must be saved as separate .csv files and any text formatting or macros in the native format will be lost on conversion.

File formats that are non-proprietary (e.g. open source), or in widespread use, will tend to retain the best chance of being readable in the future. Proprietary formats, especially non-standard formats, used only by a specific software program or specific software version, are likely to present problems for future use. 

Rapid changes in technology and the market mean that file formats can become obsolete quickly - often a software application is unable to read a file created by an earlier version of itself. The implications for research data management depend on how long data need to be retained for future use - your own or others'.

Data formats that conform to an agreed international standard are less likely to become obsolete, because a variety of software applications should be able to read them. However, there are likely to be trade-offs in terms of software functionality, for example loss of formatting or macros.

Sometimes there is a de facto standard that is used; for example, PDF, an openly published portable document format invented by Adobe, has become a de facto standard for publishing documents on the World Wide Web in a way that retains the original layout, fonts and text formatting.

At some time during your research you may need to convert or migrate your data files from one format to another. This may be due to a new computer, new software, sharing with someone who has different software, working on a shared platform instead of your own PC, or simply in order to ensure that your data can be read and used in the future.

Some lossiness - that is the loss of information and/or quality in the original data - may occur when migrating from one file format to another. It is important for you to understand what is at risk for the type of data you are working with.

Potential risks for loss or corruption on conversion or migration to new media
Word processed files: fonts, text formatting, headers, footers, footnotes, links to other documents...

Numeric files: special characters (such as tabs), end of line returns, last characters in rows (due to row size limitations), and especially blanks used as a missing data code, last rows (due to row number limitations).

Database files: as above but also relations among items in a table and among tables.

Image files: loss of layers, colour fidelity, resolution etc.

Multimedia: as above, but attention to frame rates, sound quality, codecs and wrappers is needed.

File sizes may change and even become surprisingly large.

It is worth briefing yourself on the format you are converting from and to before you begin; at least look them up on the Web. 

Check the integrity of converted files as thoroughly as possible immediately afterwards, e.g. by counting rows and columns, testing functionality, testing export, etc. as well as simply 'eyeballing' the data to check it looks as it should.

A checksum algorithm tool can be used to compare the bits of a file copied from one medium to another, but these won't work if the file format changes, or if comparing files on different computing platforms.

At some point you may choose to compress your data files for the purpose of local or networked storage, transportation or transmission. This is called bit-rate reduction, which involves encoding information using fewer bits than the original representation. 

Zip (.zip) is a de facto standard compression format that is used on Windows, Macintosh, Linux and Unix platforms, though there are others, sometimes specific to a particular operating system. A self-executing zip file (.exe) should not be used if the file is to be decompressed on another operating system.

Zip is a "lossless" type of compression, which means the file should be identical to the original once unzipped. There are also "lossy" types of compression associated with some multimedia file formats, which may result in some distortion or loss of quality/fidelity when played.

Tar (tape archive) files are commonly used in Unix / Linux to bundle a set of files into one. Tar files may also be zipped to reduce the file size (.tar.Z or tar.gz or .tar.bz2). In Windows environments the zip file can be used for the same purpose - to bundle files together, with or without compression, or with more or less compression. Utilities for tar files in Windows also exist.

Lossiness can be one trade-off of compression. Another is the processing time it takes to compress/decompress before or during use, or the amount of computing resource this takes, in the case of very large files or shared servers.

From: MANTRA "File formats and transformation" [module](http://mantra.edina.ac.uk/fileformatandtransformation/)



Data formats are often closely tied to data types and arrangements. Earlier we discussed using spreadsheets for data entry, and we'll continue with this example.

Qualitative experimental data in a tabular arrangement can be saved in many formats depending on the software you chose to use. A few are:

|Formats                             |Extensions|
|------------------------------------|----------|
|Microsoft Excel spreadsheets        | .xslx    |
|Google Spreadsheets                 | .gsheet  |
|Comma-seperated values              | .csv     | 


### Questions
- Have you worked with spreadsheets?
- Which software do you prefer?
- Have you had to use a software you're uncomfortable with?
- Do you use multiple tools?

### Your preferred formats
You might have software preferences that suit your research workflow or are required by your research group. 

From the data lifecycle perspective, we also want to think about:

- Interoperability: making sure that we can share data with people who use different software tools. 
- Preservation: making sure data files can be accessed 10 or more years down the line. 

### Exercise: Opening an old file
Here is a data file from ...., try to open it.

Some software can become obsolete, or move to new file formats without supporting old ones, and be difficult to convert.

## Feature of files that last
Recommended file formats for data have a few features that make them likely to be accessible in different computing environments and for the long term. 

**These formats have the following features:**

- non-proprietary
- open and documented standard
- uncompressed
- standard character encoding (ASCII, or Unicode encoding)
- commonly used by the research community


In the case of tabular data, even if you use a spreadsheet software like Excel to work with data, the preferred format to save, export or later transform your data into is CSV. From both Excel or Google Docs this is a built-in menu option. 

Note that the CSV file is a much simpler plain text format. Without special encoding that these softwares add and are able to read. If you use something like highlighting, or freezing headers, or formulas within your Excel spreadsheets, this will be lost in the CSV.

For the curious, the Library of Congress makes digital format descriptions available on their [website](https://www.loc.gov/preservation/digital/formats/fdd/descriptions.shtml).

### Fun fact: Character encoding and internationalization
Have you ever seen funny characters unexpectedly pop up in emails you've received, or perhaps in documents you've opened and tried to read on your computer?

*Examples of character encoding fails*
That's because "There ain't no such thing as plain text." 

Software needs to know the character encoding in order to know how to interpret and diplay text characters. Sometimes a particular software expects one encoding, but a file is saved in another. When the file is opened by that software things can look a little wonky. Remember this if you're working with international collaborators who natively use a different language, they're more likely to use different encodings to display characters. Special characters usually cause the biggest problems.

Play it safe by making sue you're using ASCII or Unicode.

From: Spolsky, Joel. 2003. "The Absolute Minimum Every Software Developer Absolutely, Positively Must Know About Unicode and Character Sets (No Excuses!)"[blog](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)

### Converting formats
You may need to transform your data as part of working with it, when sharing with collaborators, externally, or for preservation purposes.
Change text encoding
Proprietary to non-proprietary
Why not move from compressed to uncompressed? You cannot go back to a higher quality, e.g. a higher resolution image from a lower one. Saving a rich file like .. as ... to save space. In doing so, you may lose important information... this is worth remembering if you work with image or graphic, video, and audio files.
*Walk through image compression*

### Walkthrough: Convert file formats
Open this file in excel.

## Conclusion
- Identify appropriate file formats for sharing data.
- Understand metadata
- Use a metadata schema

## References
- Cornell Research Data Management Service Group. File formats. http://data.research.cornell.edu/content/file-formats
- Cornell Research Data Management Service Group. Metadata and Describing Data. http://data.research.cornell.edu/content/writing-metadata
- DataONE. Document and Store Data Using Stable File Formats. http://www.dataone.org/best-practices/document-and-store-data-using-stable-file-formats. Useful information about file formats.
- Library of Congress. Recommended formats statement. VI. Datasets/Databases. https://www.loc.gov/preservation/resources/rfs/data.html