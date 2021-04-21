# Transforming data
## What is data transformation?

![img](img/transform.png)
In this reading, you will explore how data is transformed and the differences between wide and long data. **Data transformation** is the process of changing the data’s format, structure, or values. As a data analyst, there is a good chance you will need to transform data at some point. 

Data transformation usually involves these tasks:

* Adding, copying, or replicating data 
* Deleting fields or records 
* Standardizing the names of variables
* Renaming, moving, or combining columns in a database
* Joining one set of data with another
* Saving a file in a different format. For example, saving a spreadsheet as a comma separated values (CSV) file.

&nbsp;

## Why transform data?

Goals for data transformation might be: 

* Data **organization**: better organized data is easier to use
* Data **compatibility**: different applications or systems can then use the same data
* Data **migration**: data with matching formats can be moved from one system to another
* Data **merging**: data with the same organization can be merged together
* Data **enhancement**: data can be displayed with more detailed fields 
* Data **comparison**: apples-to-apples comparisons of the data can then be made 

&nbsp;

## A data transformation use case

Mario is a plumber who owns a plumbing company. After years in the business, Mario buys another plumbing company. Mario wants to merge the customer information from his newly acquired company with his own, but the other company uses a different database. So, Mario needs to make the data compatible. To do this, he has to transform the format of the acquired company’s data. Then, he must remove duplicate rows for customers they had in common. And when the data is compatible and joined together, Mario’s plumbing company will have a complete and merged customer database.

&nbsp;

## Transforming long data to wide data
**Long data** is data in which each row is a data point for an individual subject. Each subject has data in multiple rows.

**Long data example: Stock prices**
![img](img/transform2.png)



**Wide data** is data in which each data subject has a single row with multiple columns for the values of the various attributes (or variables) of the subject. 

**Wide data example: Stock prices**
![img](img/transform3.png)



You might notice that all the data included in the long format is also in the wide format. But wide data is easier to read and understand. That is why data analysts typically transform long data to wide data more often than they transform wide data to long data. The following table summarizes when each format is preferred:

| Wide data is preferred when                                        | Long data is preferred when                                                                                |
| ------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------- |
| Creating tables and charts with a few variables about each subject | Storing a lot of variables about each subject. For example, 60 years worth of interest rates for each bank |
| Comparing straightforward line graphs                              | Performing advanced statistical analysis or graphing                                                       |
