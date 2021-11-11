## Weekly challenge 2

Latest Submission Grade: 100%

&nbsp;

### Question 1

A data analyst is assigning a variable to a value in their company’s sales dataset for 2020. Which variable name uses the correct syntax? 

* `_2020sales`
* **`sales_2020`**
* `-sales-2020`
* `2020_sales`

> The variable with the correct syntax is sales_2020. A variable name in R may contain numbers and underscores as well but not as the first character.

&nbsp;

### Question 2

You want to create a vector with the values 43, 56, 12 in that exact order. After specifying the variable, what R code chunk allows you to create this vector? 


* `v(43, 56, 12)`
* `v(12, 56, 43)`
* **`c(43, 56, 12)`** 
* `c(12, 56, 43)`


> The code chunk **`c(43, 56, 12)`**  will create a vector with the values 43, 56, 12. A vector is a group of data elements of the same type stored in a sequence in R. You can create a vector by putting the values you want inside the parentheses of the combine function. 

&nbsp;

### Question 3

If you use the mdy() function in R to convert the string “**`April 10, 2019`**”, what will return when you run your code?

* `“4/10/2019”`
* **`“2019-04-10”`** 
* `“2019-10-4”`
* `“4.10.19”`


> If you use the mdy() function in R to convert the string “**`April 10, 2019`**”, the value returned will be “**`2019-04-10`**”. The mdy() function and other variations of the ymd() function convert string data types into date/time data types.

&nbsp;

### Question 4

Question 4
A data analyst inputs the following code in RStudio: 

**`sales_1 <- (3500.00 * 12)`**

Which of the following types of operators does the analyst use in the code? Select all that apply.

* **Assignment**
* **Arithmetic**
* Relational
* Logical

> In the code `sales_1 <- (3500.00 * 12)`, the analyst uses an assignment (`<-`) and an arithmetic (`*`) operator. The assignment operator assigns the calculated value in parentheses to the variable sales_1 and the arithmetic operator multiplies the values in parentheses to complete the calculation.

&nbsp;

### Question 5

Which of the following files in R have names that follow widely accepted naming convention rules? Select all that apply.

* **patient_details_1.R**
* **patient_data.R**
* p1+infoonpatients.R
* title*123.R
  
> The files with names that follow widely accepted naming convention rules are patient_data.R and patient_details_1.R. These file names end in .R and use only lowercase letters, numbers, and underscores. They are also clear, concise, and meaningful.resource about keeping your code readable for a refresher.
&nbsp;

### Question 6

* Comments
* Pipes
* Vectors
* **Packages**

> In R, packages include reusable R functions and documentation about how to use the functions. They also include sample data sets and tests for checking your code.

&nbsp;

### Question 7

Packages installed in RStudio are called from CRAN. CRAN is an online archive with R packages and other R-related resources.

* **True**
* False

> Packages installed in RStudio are called from CRAN. CRAN is an online archive with R packages and other R-related resources.

&nbsp;

### Question 8

A data analyst is reviewing some code and finds the following code chunk:
<pre><b> mtcars %>%
     filter(carb > 1) %>%
     group_by(cyl) %>%
</b></pre>
What is this code chunk an example of?


* Data frame
* Nested function
* **Pipe**
* Vector

> The code chunk is an example of a pipe. A pipe is a tool for expressing a sequence of multiple operations in R (in this case filtering and grouping). The operator for a pipe is %>%.
