# Quality control
## Module objectives
- Understand the need for quality control
- Understand how to document cleaning 

## Why quality control?
- Data are dirty
- Ensure data are clean and usable
- Document caveats

## Primary and secondary data quality



## Data cleaning and transformation
There are a number of reasons you might need to transform your data during your research project or afterwards. Unlike the earlier discussion about migrating your file format, data transformation involves computing new values from old in the actual data content.

Some transformations are purely statistical, and are used to prepare the data to fit a model. An example was given earlier of one kind of transformation - logarithmic transformation to make a skewed distribution fit on a normal (bell) curve.

Of course there are implications for decisions about which form of the data to keep for the long term, which form to share with other researchers, and how to document all changes to the data. Other units in this module cover these topics.

In survey data collected from questionnaires, multiple choice and other kinds of responses are usually coded as numbers instead of character strings. This simple type of transformation has the advantages of easing data entry if typing in paper responses and avoiding inconsistencies (e.g. typos) in data values.

Qualitative data, for example interview transcripts, may be transformed into quantitative data by applying textual coding and categorisation techniques. Such variables (subjectively derived from a human thought process rather than computed) are understandably described as categorical or nominal, and can have a certain range of statistical techniques applied to them. Variables measured at an ordinal, interval or ratio level, that is 'real' numbers where a value reflects some measurement of the concept of interest, allow for a wider range of methods of analysis.

Another reason for data transformation may be to visualise the data effectively. A simple example is converting data where there is a numerator and a denominator, from ratios to percentages in order to display on a bar chart or pie graph. 

When preparing data for display (visualisation), questions of scale and granularity arise. For example, should a line chart have daily occurences along the Y axis, or be smoothed over (averaged) to show points by week or month? The answer depends on what is worth showing in the data. Anomalies may be smoothed over at a higher level; is this desirable, to eliminate noise, or deceptive (where anomalies may be revealing)?

A number of techniques may be used to transform confidential or sensitive data so that they may be shared with other researchers. These include:
aggregation: "the combination of related categories, usually within a common branch of a hierarchy, to provide information at a broader level to that at which detailed observations are taken." (OECD definition) Geographical data are also often aggregated to a higher unit, where information is deemed sensitive or revealing (e.g. postcode unit to postcode sector).

anonymisation: cases are stripped of revealing identifiers such as name and address. Pseudonymisation is a common technique for protecting identities in qualitative data.

perturbation: a deliberate distortion is introduced at the level of tabular data cells. Population Census data are sometimes released with perturbations as a trade-off for geographical detail.

From: MANTRA "File formats and transformation" [module](http://mantra.edina.ac.uk/fileformatandtransformation/)


## Tools for data manipulation
Tabular data

- Excel
- GoogleDocs
- OpenRefine
- NVIVO
- SAS
- SPSS
- STATA
- Matlab
- R
- Python (NumPy, SciPy, Pandas, IPython)

Quality control (DataONE)
Preparation for analysis (DataONE)