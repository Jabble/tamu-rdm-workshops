# File formats and metadata
## 3. Introduction
In this module, we'll look at converting data into different file formats, 
and taking advantage of your data documentation to create metadata that describe you data files. 

The goal is to ensure your data are useful when shared with others. 

## 4. Exercise
- We've talked a lot about spreadsheets.  What kind of file formats you are likely to work with in your research? 
- What are the outputs of the softwares you use?

- Will you also have code, audio, video, etc?
- Do you know how these files are saved?

## 5. File formats
In order to understand file formats, we need to think about how computers save digital contant and are able to display or interpret that content.

- File formats are a way of encoding information within a computer file. 
- The format specifies how bits (0's and 1's) are used to encode information.
- A program or application must be able to recognise the file format in order to access data within the file. 

Example:

- A web browser (chrome, safari, firefox, explorer) is able to process and display a file in the HTML (hyper-text markup language) 
- This file format appears as a webpage. 
- If the browser encounters another filetype, it may: 
	- need to call on a special plug-in to view it, 
	- let you download the file to view in another program if it cannot recognise it.

File formats are based on either:

- binary 
- text 

- A particular file format is often indicated as part of a file's name by a file name extension, or suffix. 
	- The extension follows a . after filename and contains three or four letters that identify the format (.jpg or .jpeg).

## 6. Files with binary encodings
Binary files can only be read by applicable software, and may be proprietary. 
Only binary formats can be executed. Compiled applications are sometimes referred to as binaries. 
But binary files can also mean that they contain images, sounds, compressed versions of other files

Some files may contain both binary and text (such as Rich Text Format - .rtf files). 
This also includes files that formatting and may include additional elements in addition to textual information 

The binary file formats used by Microsoft Office products fit in this last category.


### 7.
Image files are an example of files that use binary encodings.
Many software tools can interpret the binary encoding used for image files.
But, If you open them with a software that cannot interpret the particular binary encoding used to store the image, 
Like text processing software, you see meaningless symbols.
Text processing softwares can only handle text-based file formats, which use very different encoding standards.

### 8. Files with character encoding
Have you ever seen funny characters unexpectedly pop up in emails you've received, or perhaps in documents you've opened and tried to read on your computer?

- When we talk about "plain text" file formats
- That is formats that contain only text, where formatting such as bold or italics would be noted by textual mark-up
- it's worth understanding that there isn't actually a single "plain text."

- Plain text files are actually machine-readable only when a program knows how to interpret and display
- the character encoding standard used to create the files.

- All text characters are encoded in one way or another, and there are different encoding standards used in countries and by different software. 

- Sometimes a particular software expects one encoding, but a file is saved in another. 
- That's why when the file is opened by that software things can look a little wonky. 

Remember this if you're working with international collaborators who natively use a different language, 
they're more likely to use different encodings to display characters. 

Special characters usually cause the biggest problems.

### 9. ASCII and UTF-8 text encoding standards
Play it safe by making sue you're using ASCII or Unicode UTF-8 character encoding when you save plain text files.

The ASCII text-encoding standard is older.
It needs one byte to create 128 unique values (0–127) to represent the alphabetic, numeric, and punctuation characters commonly used in English.
plus a selection of control codes which do not represent printable characters.

UTF-8 is a newer character encoding capable of encoding all 1,112,064 valid code points in Unicode using one to four 8-bit bytes.
It is an international sandard and especially used for online text content.
It was designed for backward compatibility with ASCII, and is variable length can rep every character and is memory efficient (uses just as much apce as necessary).
The first 128 characters (US-ASCII) need one byte. 
The next 1,920 characters need two bytes to encode, which covers:

- the remainder of almost all Latin-script alphabets,
- Greek, Cyrillic, Coptic, Armenian, Hebrew, Arabic, Syriac, Thaana and N'Ko alphabets, 
- as well as Combining Diacritical Marks. 

Three bytes are needed for characters in the rest of the Basic Multilingual Plane, 
which contains virtually all characters in common use
including most Chinese, Japanese and Korean characters. 

Four bytes are needed for characters in the other planes of Unicode, 
which include less common CJK characters, 
various historic scripts, 
mathematical symbols, 
and emoji (pictographic symbols)

Well-known file extensions of 'plain text' are .txt, .csv, .asc, .html and .xml. 

Most software applications offer export or exchange formats that allow a text-formatted file to be created for importing into another program. 

From: Spolsky, Joel. 2003. "The Absolute Minimum Every Software Developer Absolutely, Positively Must Know About Unicode and Character Sets (No Excuses!)"[blog](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)
(i.e., ASCII, UTF-8)

## 10. File formats for data
### Your preferred formats
You might have software preferences that suit your research workflow or are required by your research group. 

From the data lifecycle perspective, we also want to think about:

- Interoperability: making sure that we can share data with people who use different software tools. 
- Preservation: making sure data files can be accessed 10 or more years down the line. 

Data formats are often closely tied to data types and arrangements. 
Earlier we discussed using spreadsheets for data entry, and we'll continue with this example.

Qualitative experimental data in a tabular arrangement can be saved in many formats depending on the software you chose to use. A few are:

|Formats                             |Extensions|
|------------------------------------|----------|
|Microsoft Excel spreadsheets        | .xslx    |
|Google Spreadsheets                 | .gsheet  |
|Comma-seperated values              | .csv     | 


## 11. Feature of files that last
- The file format you choose for your data is a primary factor in someone else's ability to access it in the future. 
- Think carefully about what file format will be best to manage, share, and preserve your data. 
- Technology continually changes and all contemporary hardware and software should be expected to become obsolete. 
- Consider how your data will be read if the software used to produce it becomes unavailable. 
- Although any file format you choose today may become unreadable in the future, some formats are more likely to be readable than others.

Formats likely to be accessible in the future are:

1. In common usage by the research community
2. Non-proprietary
- File formats that are non-proprietary (e.g. open source), or in widespread use, 
- will tend to retain the best chance of being readable in the future. 
- Proprietary formats, especially non-standard formats, used only by a specific software program or specific software version, are likely to present problems for future use. 
- Rapid changes in technology and the market mean that file formats can become obsolete quickly - often a software application is unable to read a file created by an earlier version of itself. The implications for research data management depend on how long data need to be retained for future use - your own or others'.
Files in proprietary formats usually must be opened by the software in which they were created. 
Someone without a licence to the software may not be able to open the file at all. 
Open formats, in which the software company or collective publishes the format rather than keeps it proprietary, 
are more likely to be readable by more than one application. 

Adobe PDF is an example of an open format that may be viewed in a number of applications, not just Adobe products.

3. Open and documented standards
4. Uncompressed (space permitting)
	- Why? Can't move easily from compressed to uncompressed.
	- You cannot go back to a higher quality, e.g. a higher resolution image from a lower one. 
5. Using standard character encodings 

## 12. Recommended formats
Examples of preferred format choices for data sharing, and especially for long-term preservation:

Text	PDF/A, HTML, XML, TXT 
Databases	XML, CSV 
Numbers/statistics	ASCII, DTA, POR, SAS, SAV
Geospatial	SHP, DBF, GeoTIFF, NetCDF
Audio	WAVE, AIFF, MP3, MXF
Images	TIFF, JPEG 2000, PDF, PNG, GIF, BMP
Moving Images	MOV, MPEG, AVI, MXF
Web Archive	WARC
Containers	TAR, GZIP, ZIP
Vector Images	Scalable Vector Graphics (.svg)

POR file extension is a portable version of SPSS

The Library of Congress, National Digital Information Infrastructure and Preservation Program (NDIIPP) has created a comprehensive resource on formats for preservation.  

## 13. Alternatives
Examples of discouraged format choices and better alternatives:
	
Discouraged Format	Alternative Format
Excel (.xls, .xlsx)	Comma Separated Values (.csv)
Word (.doc, .docx)	plain text (.txt), or if formatting is needed, PDF/A (.pdf)
PowerPoint (.ppt, .pptx)	PDF/A (.pdf)
Photoshop (.psd)	TIFF (.tif, .tiff)
Quicktime (.mov)	MPEG-4 (.mp4)

- If you find it necessary or convenient to work with data in a proprietary/discouraged file format, do so, 
- but consider saving your work in a more archival format when you are finished.

It’s important to store data (textual, image, dataset, etc.) in as open a format as possible, 
while still keeping the characteristics of the data and its representation intact. 

If data, or its documentation is held in a proprietary, platform-dependent format, it is likely that 

- these data will be inaccessible in the future, 
- or will need to undergo a costly migration process before it is accessible and useable.  

Examples of problematic formats include Microsoft Word, or Microsoft Excel. 
It is far better to convert data (files) to an open format (Open Document Format/ODF) or a more sustainable, platform-independent format such as CSV, or PDF/A.

## 14. Tips for converting file formats
At some time during your research you may need to convert or migrate your data files from one format to another. 

- This may be due to a new computer, 
- new software, 
- sharing with someone who has different software, 
- working on a shared platform instead of your own PC, 
- or simply in order to ensure that your data can be read and used in the future.

Big point: Non-proprietary and using an agreed international standard

- Advantage of creating or saving research data in a text format, is that they can be read in by any plain text editor and are human readable.
 
- They can be opened in any operating system, and by a wide range of applications. 
	- Least likely to become obsolete over time
	- Good for sharing and moving across software

- A typical example is Microsoft Excel or Google Docs built-in menu option to "Save As..." or "Export" 
- Save spreadsheet data in comma delimited format 
	- .csv or comma separated values
- The structure of the rows and columns is preserved through commas and line returns. 
	- Multiple worksheets must be saved as separate .csv files
	- Any text formatting or macros in the native format will be lost on conversion.
	- If you use something like highlighting, or freezing headers, or formulas within your Excel spreadsheets, this will be lost.


- Sometimes there is a de facto standard that is used; 
- for example, PDF, an openly published portable document format invented by Adobe, 
- has become a de facto standard for publishing documents online in a way that retains the original layout, fonts and text formatting.


### Lossiness
- Some lossiness 
- that is the loss of information and/or quality in the original data - 
- may occur when migrating from one file format to another. 
It is important for you to understand what is at risk for the type of data you are working with.

- Potential risks for loss or corruption on conversion or migration to new media

Word processed files: fonts, text formatting, headers, footers, footnotes, links to other documents

Numeric files: special characters (such as tabs), end of line returns, last characters in rows (due to row size limitations), and especially blanks used as a missing data code

Database files: relations among items in a table and among tables.

Image files: loss of layers, colour fidelity, resolution etc.

Multimedia: as above, but attention to frame rates, sound quality, codecs and wrappers is needed.

File sizes may change and even become surprisingly large.

It is worth briefing yourself on the format you are converting from and to before you begin; at least look them up on the Web. 


### Integrity
Check the integrity of converted files as thoroughly as possible immediately afterwards, 

- by counting rows and columns, 
- testing functionality, 
- testing export, 
- simply 'eyeballing' the data to check it looks as it should.

A checksum algorithm tool can be used to compare the bits of a file copied from one medium to another

- but these won't work if the file format changes, 
- or if comparing files on different computing platforms.

### Compression and bundling in containers
- At some point you may choose to compress your data files to share them
- This is called bit-rate reduction, which involves encoding information using fewer bits than the original representation.

- You should consider the processing time it takes to compress/decompress before or during use, 
- and the amount of computing resource this takes, in the case of very large files or shared servers. 

ZIP

- Zip (.zip) is a de facto standard compression format that is used on Windows, Mac, and Linux platforms, 
- A self-executing zip file (.exe) should not be used if the file is to be decompressed on another operating system.

- Zip is a "lossless" type of compression, which means the file should be identical to the original once unzipped. 
- There are also "lossy" types of compression associated with some multimedia file formats, 
	- which may result in some distortion or loss of quality/fidelity when played.

TAR

- Tar (tape archive) files are commonly used in Unix / Linux to bundle a set of files into one. 
- Tar files may also be combined with ziping to reduce the file size (.tar.Z or tar.gz or .tar.bz2).

## 15 Metadata 
Metadata is structured information that describes, explains, locates, or otherwise makes it easier to retrieve, use, or manage an information resource. 
Metadata is often called data about data or information about information

- We talked a little bit about metadata when we discussed quality assurance and questions to ask if you'd like to combine datasets.
	 - Things like: Is the dataset from a reliable source? How and for what purpose were the data collected?
- These questions can only be answered by having appropriate metadata and sufficient documentation associated with data files.

- Things like searching on a computer and online by author, title, format, or a descriptive phrase require
	 - that this kind of information (metadata) exists, 
	 - is appropriately formatted and located.

- This is usually done through the creation of a metadata record. 
- Attaching the digital object to its record makes it even more accessible and we'll get more into this later on.

## 16. Discussion
- Have you created or used metadata? 
- What is it good for?

## 17. Metadata for data
Helps to organize objects for:

- Discoverability
- Accessibility

- The creation of metadata is becoming a requirement for practical use of research observations and results. 

To:

- find data from other researchers to support your research; 
- use the data that you do find; 
- help other professionals to find and use data from your research; and
- use your own data in the future when you may have forgotten details of the research.
 
This will also depend on the existence of high-quality metadata. 

- Better metadata makes it easier to search for a data file
- and provides more information about ownership, reuse and the data structure 

This information is attached to the object, and will follow it throughout its lifecycle, and facilitate its use.

## 18. Distinguishing documentation and metadata
- Generally, documentation is maintained while working,
- and metadata would be created do describe paricular data or datasets as objects in and of themselves.

Documentation can be informal, created while working through project. May pertain to many different levels and provide general context.

Metadata formally describes a particular object (can be a data file or dataset), usually upon “publication” of the object. 
It is formatted as a record structured according to a particular schema. 
May derive from the documentation.

In conjunction they can aid in the accessibility and reusability of a dataset. 
Due to it’s structure, metadata is more accessible to computers (search engines, aggregators)

## 19. Types of metadata
- Descriptive metadata describes the object or data and gives the basic facts: who created it (i.e. authorship), title, keywords, and abstract. 
- Structural metadata describes the structure of an object including its components and how they are related.  
	- It also describes the format, process, and inter-relatedness of objects. 
	- It can be used to facilitate navigation, or define the format or sequence of complex objects.
- Administrative metadata includes information about the management of the object and may include information about: 
	- preservation and rights management, 
	- creation date, 
	- copyright permissions, 
	- required software, 
	- provenance (history), 
	- and file integrity checks

## 20. Creating metadata
When? Primarily when you plan to share the data. 
Likely will derive from your documentation. 
Metadata is typically manually created.  
Some metadata may be collected automatically by scientific instrumentation, as it collects the data. 

### Metadata records
Searching online or on a computer by author, title, format, or a phrase in the description requires that information to exist in the right place.

metadata are available in a "metadata record." Commonly containing at least:

Title
Creator
Identifier
Subject
Dates

- Ownership of an object may be indicated in a variety of ways, 
	-  creator, author, publisher, and source fields of an object’s metadata record.  
- Information about how an object may be reused will typically be indicated by an additional the rights element, or field.  
	- It may consist of a broad copyright statement, where the owner of the object has decided to retain all rights, 
	- or it may consist of licensing information (e.g. a Creative Commons license), 
	- which might, for instance, require attribution in exchange for the use of the object.  

- Information about the data structure of an object, if provided, may be indicated by information in the description field.
- For more complicated digital objects (e.g. data sets consisting of more than one file), this may include information about the other files, or the file structure. 



## 22. Metadata standards
There are many different metadata standards and specifications, 
some of them are discipline, or domain, specific. 
These standards should be followed to facilitate the successful and continued access to and reuse of data. 
They guide the collection and structure of metadata so that data are described, and referred to consistently.


## 23. Examples of metadata standards
More complicated metadata standards contain many more elements than the core ones we just mentioned.

Can be: 

-  Information about the format (or MIME type) 
-  Metadata for any special equipment, computing environment, or software necessary to reuse the object are also important to provide to the user.

This is where disciplinary metadata standards come in.

Examples of some standards used in different disciplines.

- Darwin Core:  Intended to facilitate the sharing of information about biological data
- Ecological Metadata Language (EML): Particularly developed for the ecological discipline
- CIF: An extensible standard file format and set of protocols for the exchange of crystallographic and related structured data.
- DDI: An international standard for describing data from the social, behavioral, and economic sciences. Expressed in XML, the DDI metadata specification supports the entire research data lifecycle.
- DataCite: A domain-agnostic list of core metadata properties chosen for the accurate and consistent identification of data for citation and retrieval purposes.
- DC: A basic, domain-agnostic standard which can be easily understood and implemented, and as such is one of the best known and most widely used metadata standards.

- DCC List: http://www.dcc.ac.uk/resources/metadata-standards/list
- RDA List: http://rd-alliance.github.io/metadata-directory/standards/

## 24. Creating metadata records
- As indicated metadata is structured information about a resource. 
- Metadata standards, such as Dublin Core, help organize information by providing general guidance and syntax rules. 
- However, because there has been a proliferation of different metadata standards to meet the research needs for different communities, 
- Standards also make use of controlled vocabularies and technical standards in order to facilitate interoperability.

- Controlled vocabularies are simply lists of predefined terms that ensure consistency of use, and help to disambiguate similar concepts.
- Technical standards ensure that the units such as date and time, format, etc… are entered consistently amongst different researchers.

### 25. Controlled vocabularies
- It is usually a good idea to use the controlled vocabulary that best matches the type of research you are describing.
- Like having particular codes for your data that you define or might be standard for a software or your discipline. 
- These would be specific predefined terms used to describe the data within a metadata record. 
- Kind of like "tags"

Controlled vocabularies are important because they solve the problems of natural language ambiguity such as homographs and synonyms. 

Some examples of controlled vocabularies include:
 
- ERIC Thesaurus for education terms (http://www.eric.ed.gov/ERICWebPortal/resources/html/thesaurus/about_thesaurus.html), the 
- IEE INSPEC Thesaurus of the Scientific and Technical terms (http://www.theiet.org/resources/inspec/products/aids/index.cfm), and the 
- Centre for Agricultural Bioscience international’s CAB Thesaurus (http://www.cabi.org/cabthesaurus/mtwdk.exe?yi=home).
- Medical Subject Headings (MeSH) (http://www.nlm.nih.gov/mesh/). 

### 26. Technical standards
Date and time is a particularly troublesome element to enter consistently because of different types of notation.

ISO 8601. This is important because different metadata standards may need different levels of granularity in the date and time and because different communities have different ways of expressing dates.  
The formats and required punctuation are found below. 

ISO 8601 technical standard:

YYYY (e.g. 1997)
Year and month:
YYYY-MM (e.g. 1997-07)

Complete date: YYYY-MM-DD (e.g. 1997-07-16)

- Don’t worry about knowing all the different technical standards and controlled vocabularies.  
- Typically the metadata standard you use will provide a best practice recommendation 
- for which controlled vocabularies and standards you should enter.  

## 27. Tips for metadata
- Consistent data entry is important.  
	- Review your metadata for typos, extraneous punctuation, and any inconsistencies in fielded entry, such as putting an author into a title field.
- Avoid extraneous punctuation as it can create retrieval issues. 
- Avoid most abbreviations
- Use templates and macros when possible
- Extract pre-existing metadata from your sources whenever possible
- Keep a data dictionary of the elements, technical standards, and controlled vocabularies you use in your project.
- Always use an established metadata standard.
	- Your discipline probably already has a best practices metadata standard specific to your research needs.

## Conclusion
- Identified appropriate file formats for sharing data.
- Reviewed basics of metadata standards


Understand what metadata is 
Understand why metadata is important
Identify applicable standards for capturing  and documenting metadata
Understand disciplinary practices associated with the collection and documentation of metadata
Identify an approach to creating metadata for a project

Generally comes about by a combination of manual and automatic extraction
Manual metadata is generally descriptive in nature
You will be entering it into a form, a spreadsheet, etc..
Automatic extraction is generally technical in nature
Generally will occur via software


## References
- Open Science Training Handbook. "Open Licensing and FIle Formats" [Website](https://open-science-training-handbook.gitbooks.io/book/content/02OpenScienceBasics/06OpenLicensingAndFileFormats.html)
- Abrams, Stephen. "File Formats" [PDF](http://www.dcc.ac.uk/resources/curation-reference-manual/completed-chapters/file-formats)
- Cornell Research Data Management Service Group. File formats. http://data.research.cornell.edu/content/file-formats
- Cornell University Library. eCommons: Cornell's Digital Repository. "Recommended File Formats" [Website](http://guides.library.cornell.edu/ecommons/formats)
- Cornell Research Data Management Service Group. Metadata and Describing Data. http://data.research.cornell.edu/content/writing-metadata
- DataONE. "Document and Store Data Using Stable File Formats" [Website](http://www.dataone.org/best-practices/document-and-store-data-using-stable-file-formats) Useful information about file formats.
- Library of Congress. "Sustainability of digital formats" [Website](https://www.loc.gov/preservation/digital/formats/index.shtml)
- NISO. "Understanding Metadata: What is metadata and what is it for?" [PDF](http://www.niso.org/apps/group_public/download.php/17446/Understanding%20Metadata.pdf)

Introduction to Metadata: Setting the Stage (Getty Research Institute) http://www.getty.edu/research/publications/electronic_publications/intrometadata/setting.html

Documentation and Metadata (MIT Libraries): http://libraries.mit.edu/guides/subjects/data-
management/metadata.html

Anne J. Gilliland for The J. Paul Getty Trust’s Introduction to Metadata (Online Edition, Version 3.0 http://www.getty.edu/research/publications/electronic_publications/intrometadata/setting.html)

Library of Congress makes digital format descriptions available on their [website](https://www.loc.gov/preservation/digital/formats/fdd/descriptions.shtml).
