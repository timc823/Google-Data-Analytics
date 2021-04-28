## Weekly challenge 2

Latest Submission Grade: 100%

&nbsp;

### Question 1

Which of the following terms describe clean data? Select all that apply.


* **Complete**
* **Correct**
* **Relevant**
* Refutable 
  
> Clean data is complete, correct, and relevant to the problem being solved. Dirty data is incomplete, incorrect, and irrelevant to the problem being solved.

&nbsp;

### Question 2

Field length is a spreadsheet tool for determining if a field has been duplicated.

* True
* **False**

> Field length determines the number of characters that may be typed into a field.

&nbsp;

### Question 3

A data analyst notices that the customer in row 2 shares the same Customer ID as the customer in row 6. What does this scenario describe? 

|        | A             | B              | C                  | D               |
| ------ | ------------- | -------------- | ------------------ | --------------- |
| **1**  | **Last name** | **First name** | **Middle initial** | **Customer ID** |
| **2**  | Smith         | Leonardo       | R.                 | 64078           |
| **3**  | Lee           | Natasha        | E.                 | 92862           |
| **4**  | Wallace       | Luciana        | M.                 | 55107           |
| **5**  | Xiao          | Hua            | A.                 | 88492           |
| **6**  | Smith         | Leo            | R.                 | 64078           |
| **7**  | Chaudhuri     | Toby           | T.                 | 34694           |
| **8**  | Lee           | Tasha          | P.                 | 18295           |
| **9**  | Walton        | Mason          | Q.                 | 58239           |
| **10** | Richards      | Felix          | S.                 | 12765           |
| **11** | Guillermo     | Beth           | I.                 | 27593           |
| **12** | Walton        | Nadine         | J.                 | 67292           |
| **12** | Walton        | Nadine         | J.                 | 67292           |

* **Duplicate data**
* Mislabeled data
* Inconsistent data
* Obsolete data

> This is duplicate data because the customer data in row 2 is a duplicate of the customer data in row 6.

&nbsp;

### Question 4

Conditional formatting is a spreadsheet tool that changes how cells appear when values meet a specific condition. Data analysts can use conditional formatting to do which of the following tasks? Select all that apply.  

* **To identify blank cells or missing information**
* To calculate mathematical equations
* **To make cells stand out for more efficient analysis**
* To sort data in series of cells into a meaningful order

> Data analysts use conditional formatting to identify blank cells or missing information and to make cells stand out for more efficient analysis.

&nbsp;

### Question 5

A delimiter is a character that indicates the beginning or end of a data item. The split text to columns tool uses a delimiter to accomplish what task?


* To split duplicate substrings
* To split one column into two
* **To specify where to split a text string**
* To change the format of a column of text 

> The split text to columns tool uses a delimiter to specify where to split a text string.

&nbsp;

### Question 6

Question 6
Fill in the blank: A predetermined structure that includes a function’s required information and its proper placement is called _____.

* **Syntax**
* Validation
* Summary
* Algorithm

> Syntax is a predetermined structure that includes a function’s required information and its proper placement.

&nbsp;

### Question 7

You are working with the following selection of a spreadsheet:

|       | A             | B                                            |
| ----- | ------------- | -------------------------------------------- |
| **1** | **Customer**  | **Address**                                  |
| **2** | Sally Stewart | 9912 School St. North Wales, PA 19454        |
| **3** | Lorenzo Price | 8621 Glendale Dr. Burlington, MA 01803       |
| **4** | Stella Moss   | 372 W. Addison Street Brandon, FL 33510      |
| **5** | Paul Casey    | 9069 E. Brickyard Road Chattanooga, TN 37421 |

In order to extract the five-digit postal code from Brandon, FL, what is the correct function? 

* =LEFT(5,B4)
* =LEFT(B4,5)
* =RIGHT(5,B4)
* **=RIGHT(B4,5)**

> The correct syntax is =RIGHT(B4,5). The RIGHT function returns a set number of characters from the right side of a text string. B4 is the specified cell. And 5 is the number of characters to return.

&nbsp;

### Question 8

A data analyst in a human resources department is working with the following selection of a spreadsheet:
	
|       | A              | B                 | C              | D               |
| ----- | -------------- | ----------------- | -------------- | --------------- |
| **1** | **Year Hired** | **Last 4 of SS#** | **Department** | **Employee ID** |
| **2** | 2019           | 1192              | Marketing      |                 |
| **3** | 2014           | 2683              | Operations     |                 |
| **4** | 2020           | 1939              | Strategy       |                 |
| **5** | 2009           | 3208              | Graphics       |                 |

They want to create employee identification numbers (IDs) in column D. The IDs should include the year hired plus the last four digits of the employee’s Social Security Number (SS#). What function will create the ID 20093208 for the employee in row 5?

* **=CONCATENATE(A5,B5)**
* =CONCATENATE(A5+B5)
* =CONCATENATE(A5:B5)
* =CONCATENATE(A5*B5)

> To create the ID 20093208 for the employee in row 5, the function is =CONCATENATE(A5,B5). CONCATENATE joins together two or more text strings. (A5,B5) are the locations of the strings to be joined.

&nbsp;

### Question 9

An analyst is cleaning a new dataset containing 500 rows. They want to make sure the data contained from cell B2 through cell B300 does not contain a number greater than 50. Which of the following COUNTIF function syntaxes could be used to answer this question? Select all that apply.



* =COUNTIF(B2:B300,>50)
* **=COUNTIF(B2:B300,">50")**
* **=COUNTIF(B2:B300,"<=50")**
* =COUNTIF(B2:B300,<=50)

> One possible syntax is =COUNTIF(B2:B300,">50"). This returns the number of cells that are greater than 50. Another option is =COUNTIF(B2:B300,"<=50"). This returns the number of cells that are less than or equal to 50. Either one can confirm that the data does not contain a number greater than 50.

&nbsp;

### Question 10

A data analyst wants to search for a certain value in a column, then return a corresponding piece of information. Which function should they use?

* FIND
* VALUE
* MATCH
* VLOOKUP

> VLOOKUP is used to search for a certain value in a column, then return a corresponding piece of information.

&nbsp;

### Question 11

A data analyst needs to combine two datasets. Each dataset comes from a different system, and the systems store data in different ways. What can the data analyst do to ensure the data is compatible?


* **Map the data**
* Apply a data structure
* Use a data visualization
* Merge the data

> Data analysts use data mapping to note differences in data sources in order to ensure the data is compatible.

&nbsp;

### Question 12

Fill in the blank: A primary key references a _____ in which each value is unique.

* row
* **column**
* string
* variable

> A primary key references a column in which each value is unique.
