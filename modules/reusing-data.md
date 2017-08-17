# Reusing data
- Finding and accessing data sources
- Evaluating data sources
- Combining and cleaning datasets
- Credit for work and incentives
- Citation


### When combining data sets
Use quality control techniques, but there are additional quesitons to ask of the data.

Review metadata for compatibility of context, methods, and meaning
For what purpose was the data collected?
How was the data collected?
Is it sensible to combine these datasets?

Maintain dataset provenance
- Where did the data come from? Did you collect it, or did you get your data form another source?
- 
Document transformations
Beware of accidental duplication




Ensure compatibility
Convert to common units
Choose appropriate numeric precision
Evaluate and standardize missing value codes

Document all assumptions
What assumptions underlie the original datasets?
What assumptions did you make in combining the datasets?


Recognize that you are creating a new dataset
Revisit the data life cycle to ensure the new dataset is properly documented, validated, and preserved


Enable transparency and reproducibility in the integration process
Ensure others understand and can evaluate your decision making process.
Automate the integration as much as possible
Especially when integrating many datasets or large datasets

Consider the compatibility of the data you are integrating

Best Practice: 
The integration of multiple data sets from different sources requires that they be compatible. Methods used to create the data should be considered early in the process, to avoid problems later during attempts to integrate data sets. Note that just because data can be integrated does not necessarily mean that they should be, or that the final product can meet the needs of the study. Where possible, clearly state situations or conditions where it is and is not appropriate to use your data, and provide information (such as software used and good metadata) to make integration easier.

Description Rationale: 
When using integrated data sets, it is crucial that the data are comparable and compatible to avoid mistakes in analyses and interpretation.

Related Best Practices: 
Confirm a match between data and their description in metadata
Document steps used in data processing
Define the data model
Additional Information: 
Burley, T.E., and Peine, J.D., 2009, NBII-SAIN Data Management Toolkit, U.S. Geological Survey Open-File Report 2009-1170, 96 p. Available from: http://pubs.usgs.gov/of/2009/1170/

Examples: 
Water-quality data collected by two separate agencies may be thematically similar but may have been sampled using completely different methods. Differences in such water-quality sample methods can include equipment, sampling method protocol, and lab analysis procedures. Analysis performed on integrated water-quality data that were collected using completely different methods would likely result in questionable results.

DataOne [website](https://www.dataone.org/best-practices/consider-compatibility-data-you-are-integrating)