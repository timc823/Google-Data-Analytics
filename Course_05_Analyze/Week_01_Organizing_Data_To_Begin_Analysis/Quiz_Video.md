### Video: The analysis process

During which analysis phase does an analyst sort and filter data?

* Organize
* Get input from others
* **Format and adjust**
* Transform

> An analyst sorts and filters data during the format and adjust analysis phase. 

&nbsp;

### Video: Always a need to organize

Fill in the blank: _____ involves arranging data into a meaningful order to make it easier to understand, analyze, and visualize.

* Organizing
* Prioritizing
* **Sorting**
* Filtering

> Sorting involves arranging data into a meaningful order to make it easier to understand, analyze, and visualize.

To narrow the scope of a query, a data analyst filters by a particular criteria. This type of filtering must be done one variable at a time.

* True
* **False**

> Filtering can be done by single variable or multiple variables, depending on the query’s needs.

&nbsp;

### Video: Using sorts and filters

You are working on an international project and need to invoice your customers for the work you complete. The database you use contains an Invoices table. The invoices table contains the following columns: InvoiceId, CustomerId, InvoiceDate, BillingAddress, BillingCity, BillingState, BillingCountry, BillingPostalCode, Total.

Create a query to return all the columns from this table for only customers in Germany who have an invoice total greater than $5.

```
select total
from invoices 
where BillingCountry='Germany' AND Total > 5.
```

How many rows are returned from this query?
12

Correct
Twelve rows are returned when making the following query:
    ```
    SELECT * FROM invoices WHERE BillingCountry='Germany' AND Total > 5. 
    ```
The AND clause allows you to write a query with more than one condition. This means that this query will return a list of 12 customers to charge that are from Germany and have invoices totaling more than $5.

&nbsp;

### Video: Sorting datasets

When you use the menu function Sort Range, nothing in your spreadsheet gets rearranged except for the fields in the specified range.

* **True**
* False

> The menu function Sort Range only sorts fields within the specified range. Data across rows are not kept together when sorted.

Which menu sort function is used to keep data together across rows?

* Sort Range
* Sort Row
* Sort Column
* **Sort Sheet**

> Sort Sheet is the menu sort function that keeps data together across rows. It also sorts all the data in the sheet, based on the ranking of a specified column.

&nbsp;

### Video: The SORT function

Which of the following statements accurately describe the difference between a menu sort function and a written SORT function?

* A menu sort function sorts data permanently, while the written SORT function only sorts it temporarily.
* A menu sort function rearranges the data, while the written SORT function rewrites it.
* A menu sort function rearranges the data, while the written SORT function changes it.
* A menu sort function changes the data, while the written SORT function rearranges it.

> A menu sort function rearranges the data, while the written SORT function changes the existing data.

&nbsp;

### Video: Sorting queries in SQL

You are working on a project about music and have a table of genres you need to sort. The Genres table contains the columns GenreId and Name.

Write a SQL query to return the name of each genre from this table in alphabetical order.

```
select GenreId , Name 
from Genres 
order by Name 
```

What are the first and last genres returned, respectively? Separate your answers by a comma followed by a space.
```
Alternative, World
```
> Alternative and World are returned when making the following query:
    ```
    SELECT Name FROM genres ORDER BY Name
    ```
Not specifying ascending or descending in your query will sort by ascending order on default. This is appropriate for sorting in alphabetical order.


You are working on a project about music and have a table of tracks you need to sort.

The database you use contains a Tracks table. The table contains the following columns: TrackId, Name, AlbumId, MediaTypeId, GenreId, Composer, Milliseconds, Bytes, and UnitPrice.

Write a SQL query to pull all columns from the Tracks table for only tracks with Chris Cornell as the composer and a unit price of less than $1. Sort the results in ascending order by GenreId.

```
select *
from Tracks
where Composer = 'Chris Cornell' AND UnitPrice <1
Order by GenreId ASC
```
What is the name of the first track that the query returns?
```
Loud Love
```

> Loud Love is the first value returned in the Name column when making the following query: 
    ```
    SELECT * FROM Tracks WHERE Composer='Chris Cornell' AND UnitPrice < 1 ORDER BY GenreId. 
    ```
When executed, this query returns a list of tracks that were composed by Chris Cornell and have a unit price of less than $1. The list would be sorted by GenreId in ascending order.

&nbsp;

### Video: Sorting queries in SQL
### Video: 
### Video: 

