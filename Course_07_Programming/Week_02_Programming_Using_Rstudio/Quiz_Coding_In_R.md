## L3 Coding in R

&nbsp;

### Question 1

An analyst includes the following calculation in their R programming: `midyear_sales <- (quarter_1_sales + quarter_2_sales) - overhead_costs` Which variable will the total from this calculation be assigned to?

* **`midyear_sales`**
* `quarter_1_sales`
* `quarter_2_sales`
* `overhead_costs`

> The total from this calculation will be assigned to the variable midyear_sales. The assignment operator <- follows the variable mid_sales, so the value of the calculated total is assigned to this variable.

&nbsp;

### Question 2

An analyst is checking the value of the variable x using a logical operator, so they run the following code:

`x > 35 & x < 65`

Which values of x would return `TRUE` when the analyst runs the code? Select all that apply.

* 35
* **50**
* **60**
* 70

> The values 50 and 60 will return `TRUE` when the analyst runs the code `x > 35 & x < 65`. In this code, the logical operator & tells the server to return `TRUE` when the value of the variable is greater than 35 and less than 65. 

&nbsp;

### Question 3

A data analyst inputs the following code in RStudio:
sales_1 <- 100 * sales_2
Which of the following types of operators does the analyst use in the code? Select all the apply. 

* relational 
* **arithmetic**
* **assignment** 
* logical 

> The analyst uses assignment and arithmetic operators in the code. The assingment operator (<-) assigns the variable sales_1 to the value of 100 * sales_2. The multiplication operator (*) multiplies 100 by sales_2. 

&nbsp;

### Video: The gift that keeps on giving

Fill in the blank: Packages in R include _____. Select all that apply. 


* **reusable R functions**
* **tests for checking your code**
* **sample datasets**
* visualizations

> Packages in R include reusable R functions, documentation about how to use the functions, sample datasets, and tests for checking your code.

&nbsp;

### Video: Welcome to the tidyverse

Tidyverse is a collection of packages in R with a common design philosophy.

True
False

> Tidyverse is a collection of packages in R with a common design philosophy. The tidyverse packages are especially useful for data manipulation, exploration, and visualization.

&nbsp;

### More on the tidyverse

Which tidyverse package is used for data visualization?

* **ggplot2**
* readr
* tidyr
* dplyr

> The ggplot2 package is used for data visualization, specifically plots. You can use ggplot2 to create a lot of different visualizations by applying different properties to the data variables.

&nbsp;

### Working with pipes

A nested function is a function contained within code that performs a broader function.


* **True**
* False

> A nested function is a function contained within code that performs a broader function. The nested function performs its own specific function within the code.

&nbsp;


Which of the following operators is the pipe operator?


* !=
* <-
* *
* **%>%**

> The pipe operator is %>%. You can use it in R programming to call out a pipe to express a sequence of multiple operations.

