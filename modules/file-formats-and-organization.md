# File formats and organization
## Objectives
- Choose appropriate file formats for data.
- Compare file naming conventions.
- Design a file naming convention.

## Introduction
Plan management -> **Collect and store**  -> Assure quality -> Analyze and present -> **Share and preserve**

In this module, we'll look at saving data and transforming data into different file formats, as well as organizing data with future accessibility in mind. The goal is to stay organized in order to focus on working with your data and ensure your data is stored in a way that you can easily share it with others. 

## Digital file formats for data
Data formats are often closely tied to data types and arrangements. Earlier we discussed using spreadsheets for data entry, and we'll continue with this example.

Qualitative experimental data in a tabular arrangement can be saved in many formats depending on the software you chose to use. A few are:

|Formats                             |Extensions|
|------------------------------------|----------|
|Microsoft Excel spreadsheets        | .xslx    |
|Google Spreadsheets                 | .gsheet  |
|Comma-seperated values              | .csv     | 

### Question:
- Have you worked with spreadsheets?
- Which software do you prefer?
- Have you had to use a software you're uncomfortable with?
- Do you use multiple tools?

## Preferred formats
You might have preferences that suit your workflow or are required by your research group, and it's likely that any of those formats will do while you're working with the data. From the data lifecycle perspective, we're thinking about:

- Interoperability: making sure that we can later share data with people who use different software. 
- Preservation: making sure the data files can be accessed 10 or more years down the line. 

### Exercise: Opening an old file
Here is a data file from ...., try to open it.

When some software may be obsolete use different file formats, and be difficult to convert.

## Recommended file formats for sharing data
For this reason, recommended file formats for data have a few features that make them likely to be accessible in different computing environments and for the long term. 

These formats have the following features:

- non-proprietary
- open and documented standard
- unencrypted (when shared)
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


## File organization
Naming files sensible things is good for you and for your computers. Without structured information, our lives would be much poorer. There's one rule from which all organization schemes can develop. 

Be consistent. 

Have conventions for your:

1. Directory structure
2. Folder names
3. File names

### Directory structure

### Folder and file naming conventions
The file and folder names are primarily for easy identification and sorting. Remember, you can use other means to save more information about your files and the data within them. We discussed this in more depth in the "Data Documentation" portion. This can be done inside the file itself or in a seperate README file that describes your file naming convention.

**Tips for constructing names**

- Be descriptive
- Include relevant information for identification
- Always include the same informational components
- Retain the order of components
- Keep names under 32 characters
- Avoid special characters
- Use '-' or '_' instead of ' '
- limit '.' to one before the file extension 

When constructing files, the following components are often relevant. Use them alone or in a combination that suits your needs.

|informational component | recommendation | example |
|----------|----------|----------|
|Name | project name or research data||
|Sequential numbering | Run of experiment Include leading zeros| 001.txt |
|Dates | Use [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format for dates to retain the order| |
|Unique identifier | A subject id for files, grant number in the folder name| |
|Experimental Condition | such as lab instrument, solvent, temperature, etc.| |


### Strategies and trade-offs
Order the components of a name to organize your file by:

Date
Type
Subject
Sequential number (forced order)

## Exercise
I'll share my directory structure and file naming schemes I use with you:
[screenshot](../images/20170726-124454-screenshot.png)
[screenshot](../images/20170726-125025-screenshot.png)

generate potential file names for your data & document your strategy 
share your strategy with a partner & hear what they came up with
volunteer to share your idea with the class


## References
- Library Carpentry. [lesson](https://data-lessons.github.io/library-data-intro/03-foundations/)
- Whitmire, Amanda. 2014. "Organizing Your Data" [slides](https://figshare.com/articles/GRAD521_Research_Data_Management_Lectures/1003835)
- Spolsky, Joel. 2003. "The Absolute Minimum Every Software Developer Absolutely, Positively Must Know About Unicode and Character Sets (No Excuses!)"[blog](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)

## Materials