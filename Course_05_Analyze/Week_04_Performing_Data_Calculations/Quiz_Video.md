### Video: Common calculation formulas

You are calculating the sum of a range of cells from A2 through F2. What is the correct syntax for this calculation?

* =SUM(A2*F2)
* **=SUM(A2:F2)**
* =SUM(A2,F2)
* =SUM(A2+F2)

> To calculate the sum of a range of cells from A2 through F2, the correct syntax is =SUM(A2:F2). Formulas begin with an equals sign. A2:F2 are the cell references to be summed. And the colon between the two cell references indicates that it is a range of cells.

You are analyzing the results of retail sales calculations. You click in cell H10 and find the following formula: =H9/G9. What operation is taking place in this cell?

* Addition
* Multiplication
* **Division**
* Subtraction

> In the formula =H9/G9, the operation is division. The operator for division is a slash (/).

&nbsp;

### Video: Functions and conditions

A data analyst is using the following formula: =COUNTIF(C2:C50, “=100”). Which part of the formula names the condition that the data must meet in order to be counted?


* **=100**
* C50
* C2
* COUNTIF

> In the formula =COUNTIF(C2:C50, “=100”), “=100” names the condition that the data must meet in order to be counted. In this formula, cells C2 through C50 will be counted if their value equals 100.

&nbsp;

### Video: Composite functions

You want to calculate a company’s annual revenue using financial data. You use the SUMPRODUCT function to multiply each of the values in the arrays B3:B7 and C3:C7, then add them together. What is the correct syntax to complete this calculation?


* **=SUMPRODUCT(B3:B7,C3:C7)**
* SUMPRODUCT(B3,B7:C3,C7) 
* =(SUMPRODUCT)(B3:B7*C3:C7)
* =SUMPRODUCT+(B3:B7/C3:C7) 

> The correct syntax is =SUMPRODUCT(B3:B7,C3:C7). Using this syntax will multiply each value in the first range by its corresponding value in the second range. Then, the values will be added together.

&nbsp;

### Video: Working with pivot tables

When using the Values menu in a pivot table, what does the Summarize By drop-down menu do?

* Chooses how to sort the values
* Selects the values for the pivot table
* **Changes the function applied to the values**
* Filters the values in ascending order

> The Summarize By drop-down menu changes the function applied to the values. The SUM function is the default function, but there are other options, such as COUNT.

A calculated field within a pivot table is used to carry out calculations based on what?

* The function in the calculated field
* **The values of other fields**
* The filtered values
* The syntax of the available formulas 

> A calculated field within a pivot table is used to carry out calculations based on the values of other fields. The calculated field is added as an additional row or column in a pivot table.

&nbsp;

### Video: Queries and calculations

A data analyst is writing a SQL query. Which commands would they use to first multiply values from a table, then place the totals in a new column? Select all that apply.

* **AS**
* **FROM**
* **SELECT**
* DIVIDE

> Use the SELECT, FROM, and AS commands in a query to first multiply values from a table, then place the totals in a new column. This will SELECT the values FROM a table and rename them AS the name of the column with the calculated values.

To find the average of a set of values, a data analyst can type AVERAGE in both spreadsheets and SQL. 

* TRUE
* **FALSE**

> The AVERAGE function finds the average of a set of values in spreadsheets. When using SQL, the function is AVG.  

&nbsp;

### Video: Embedding simple calculations in SQL

When using SQL, which of the following are reasons for using underscores in column names? Select all that apply.


* **It keeps the column names readable**
* **It helps avoid potential issues with servers and applications**
* It verifies that the values in the columns are accurate
* It tells the server that the values in the columns are for calculations 

> Using underscores instead of spaces helps avoid potential issues with servers and applications. It also helps to keep the column names readable.

What will appear in the Total_Small_Bags_Cost column after the following query is run?

```
SELECT 
Small_Bags,
Small_Bags_Cost,
Small_Bags * Small_Bags_Cost AS Total_Small_Bags_Cost
From avocado_data.avocado_prices
```

* The sum of the values in the Small_Bags and Small_Bags_Cost columns
* **The product of the values in the Small_Bags and Small_Bags_Cost columns**
* The sum of the values in the “Small_Bags_Cost” and “avocado_data.avocado_prices” columns
* The product of the values in the “Small_Bags_Cost” and “avocado_data.avocado_prices” columns

> The product of the values in the Small_Bags and Small_Bags_Cost columns will appear in the Total_Small_Bags_Cost column. The query will multiply the values in the two columns.

&nbsp;

### Video: Calculations with other statements

What will the following query return?

```
SELECT
Yes_Responses, 
Total_Responses,
Total_Responses - Yes_Responses AS No_Responses
FROM
Survey_1
```

* The number of “Yes” and “No” responses combined
* The result of dividing the total number of responses by “Yes” responses
* **The difference when "Yes" responses are subtracted from the total number of responses**
* The total when “Yes” responses are sorted from “No” responses 

> This query will return the difference when "Yes" responses are subtracted from the total number of responses. The calculation will appear in a new column named No_Responses. The division operator (/) could be used to divide these values.

What is the purpose of the EXTRACT command in a query? 

* **To extract a part from a given date**
* To extract a single word from a string 
* To extract a column from a database
* To extract a single value from a column

> The purpose of the EXTRACT command in a query is to extract a part from a given date. The EXTRACT command can extract any part from a date/time value. 


&nbsp;

### Video: Check and recheck

Fill in the blank: The data validation process is a form of data _____.


* transformation
* **cleaning**
* reporting
* formatting

> The data validation process is a form of data cleaning. During this process, data analysts check the quality of their data to make sure it’s complete, accurate, secure, and consistent.

&nbsp;

### Video: Temporary tables

A data analyst has a large number of sales records in a table. They want to perform calculations on a small subset of the table. Rather than filtering the data over and over, what should they do? 


* Use an alternate table
* **Use a temporary table**
* Use a backup table
* Use a copy of the table

> They should use a temporary table. A temporary table is created and exists for a short time on a database server. 

&nbsp;

### Video: Multiple table variations

Which of the following are methods for creating a version of a temporary table using SQL? Select all that apply.

* WHERE clauses
* **CREATE TABLE statements**
* **WITH clauses**
* **CREATE TEMP TABLE statements**

> WITH clauses, CREATE TABLE statements, and CREATE TEMP TABLE statements all create temporary tables in queries.

