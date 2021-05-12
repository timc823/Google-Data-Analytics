## Weekly challenge 3

Latest Submission Grade: 100%

&nbsp;

### Question 1

In data analytics, what is the process of gathering data from multiple sources and combining it into a single, summarized collection?

* **Data aggregation**
* Data composition
* Data grouping
* Data mapping

> Data aggregation is the process of gathering data from multiple sources and combining it into a single, summarized collection.

&nbsp;

### Question 2

A data analyst uses the SUM function to add together numbers from a spreadsheet. However, after getting a zero result, they realize the numbers are actually text. What function can they use to convert the text to a numeric value?

* FIGURE
* **VALUE**
* CONVERT
* DIGIT

> The analyst can use the VALUE function to convert the text that represents a number to a numeric value. 

&nbsp;

### Question 3

When using VLOOKUP, there are some common limitations that data analysts should be aware of. One of these limitations is that VLOOKUP only returns the first match it finds, even if there are many possible matches within the column.

* **True**
* False

> One limitation of VLOOKUP is that it only returns the first match it finds, even if there are many possible matches within the column.

&nbsp;

### Question 4

A data analyst creates an absolute reference around a function array. What is the purpose of the absolute reference?

* To copy a function and apply it to all rows and columns
* To automatically change numeric values to currency values
* **To lock the function array so rows and columns don’t change if the function is copied**
* To keep a function array consistent so rows and columns will automatically change if the function is copied

> The purpose of an absolute reference is to lock the function array so rows and columns don’t change if the function is copied.

&nbsp;

### Question 5

The following is a selection from a spreadsheet:

|     | A             | B                                 | C                                  |
| --- | ------------- | --------------------------------- | ---------------------------------- |
| 1   | **Country**   | **Population in 2020 (millions)** | **Growth in population 2000-2020** |
| 2   | China         | 1,439,323,776                     | 13.4 %                             |
| 3   | India         | 1,380,004,385                     | 37.1 %                             |
| 4   | United States | 331,002,651                       | 17.3 %                             |
| 5   | Indonesia     | 273,523,615                       | 27.7%                              |
| 6   | Pakistan      | 220,892,340                       | 44.9%                              |
| 7   | Brazil        | 212,559,417                       | 21.9%                              |
| 8   | Nigeria       | 206,139,589                       | 66.3%                              |
| 9   | Bangladesh    | 164,689,383                       | 27.9%                              |
| 10  | Russia        | 145,934,462                       | -0.8%                              |

To search for the population of Brazil, what is the correct VLOOKUP syntax? 


* =VLOOKUP(Brazil, A2:B10, 3, false)
* =VLOOKUP(Brazil, A2:B10, 2, false)
* **=VLOOKUP("Brazil", A2:B10, 2, false)**
* =VLOOKUP(Brazil, A2,B10, 3, false)

> To search for the population of Brazil, the syntax is =VLOOKUP("Brazil", A2:B10, 2, false). “Brazil” is the reference. A2:B10 is the table array. The 2 indicates the number of the column from which the value should be returned. And the word false instructs the function to return an exact match.

&nbsp;

### Question 6

When creating a SQL query, which JOIN clause returns all matching records in two or more database tables?

* OUTER
* LEFT
* RIGHT
* **INNER**

> The INNER JOIN clause returns all matching records in two or more database tables.

&nbsp;

### Question 7

A data analyst writes a query that asks a database to return only distinct values in a specified range, rather than including repeating values. Which function do they use?

* COUNT
* RETURN
* **COUNT DISTINCT**
* RETURN VALUES

 
> When writing SQL queries, an analyst can use the COUNT DISTINCT 

&nbsp;

### Question 8
Fill in the blank: In a SQL statement, the _____ is the name of the segment that executes first. Select all that apply.

* central query
* **inner query**
* central select
* **inner select**

 
> In a SQL statement, the subquery — also called an inner query, inner select, or nested query — is the segment that executes first. 
