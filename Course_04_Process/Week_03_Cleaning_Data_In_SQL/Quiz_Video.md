### Video: Understanding SQL capabilities

SQL and spreadsheets process large amounts of data at the same speed.

* True
* **False**

> SQL can process large amounts of data much more quickly than spreadsheets. This is one of the reasons why data analysts use SQL when working with vast, complex datasets.

&nbsp;

### Video: SQL versus spreadsheets

A team of analysts is working on a data analytics project. How could data in a SQL database be more useful to the team than data in spreadsheets? Select all that apply.

* They can use SQL to make working with smaller datasets easier.
* They can track changes to SQL queries across the team.
* They can use SQL to interact with the database program.
* They can use SQL to pull information from the database at the same time.

> Data stored in a SQL database is useful to a project with multiple team members because they can access the data at the same time, use SQL to interact with the database program, and track changes to SQL queries across the team.

&nbsp;

### Video: Widely used SQL queries

The media_types table contains the following columns: MediaTypeId and Name.

Create a query to return the Name column from this table.

```
select name 
from media_types 
```

What is the media type name of the 1st result returned? 
(Enter the exact name that appears in the table.)

```
MPEG audio file
```

> MPEG audio file is the media type name of the 1st result returned when making the following query:
    ```
    SELECT Name FROM media_types;
    ```

&nbsp;

The customers table contains the following columns: CustomerId, FirstName, LastName, Company, Address, City, State, Country, PostalCode, Phone, Fax, Email, SupportRepId.

Create a query to return the LastName and Country columns from this table for only customers in Germany.

```
select LastName, country
from customers
where country = 'Germany'
```

What is the last name of the customer for the 3rd result returned?
```
Zimmermann
```


> Great job. Zimmermann is the last name of the customer for the 3rd result returned when making the following query:
    ```
    SELECT LastName,Country FROM customers WHERE Country = 'Germany';
    ```

&nbsp;

### Video: Cleaning string variables using SQL

If adding DISTINCT to the query didn't make sense, you may need a refresher on how to write a query. Try the following. 

The tracks table contains the following columns: TrackId, Name, AlbumId, MediaTypeId, GenreId, Composer, Milliseconds, Bytes, and UnitPrice.

Create a query to return the TrackId, AlbumId, Composer and UnitPrice columns from this table.

```
select TrackId, AlbumId, Composer, UnitPrice
from tracks
```

What is the AlbumId of the 6th track? Please respond using a numeric value, i.e. enter '4' and not 'four'.

```
1
```

&nbsp;

In a query, if you use the LENGTH, SUBSTR, or TRIM function in a WHERE clause, you can select data based on a string condition. If you are having trouble with these, you may need a refresher on how you created a WHERE clause with a numeric condition. The concept is the same, so try the following:

The invoices table contains the following columns: InvoiceId, CustomerId, InvoiceDate, BillingAddress, BillingCity, BillingState, BillingCountry, BillingPostalCode, Total.

Create a query to return the CustomerId, InvoiceDate and Total columns from this table for only invoice totals over $20.

```
select CustomerId, InvoiceDate, Total
from invoices
where Total > 20
```

How many results are returned?
```
4
```

> Four results are returned when making the following query:
    ```
    SELECT CustomerId,InvoiceDate,Total FROM invoices WHERE Total > 20;
    ```

&nbsp;

### Video: Advanced data-cleaning functions part 2

Data analysts use which function to add strings together and create new text strings for unique keys?

* CAST
* TRIM
* LENGTH
* **CONCAT**

> Data analysts use the CONCAT function to add strings together and create new text strings for unique keys.
