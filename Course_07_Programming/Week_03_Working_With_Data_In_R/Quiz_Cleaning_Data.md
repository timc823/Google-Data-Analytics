## L3 Cleaning data

&nbsp;

### Question 1

A data analyst is cleaning their data in R. They want to be sure that their column names are unique and consistent to avoid any errors in their analysis. What R function can they use to do this automatically?

* rename()
* select()
* rename_with()
* **clean_names()**

> The clean_names() function will automatically make sure that column names are unique and consistent. 

&nbsp;

### Question 2

A data analyst is trying to sort the penguins bill_length_mm data in descending order. They input the following code: 

`penguins %>%`

What code does the analyst add to organize the column *bill_length_mm* in descending order?

* **`arrange(-bill_length_mm)`**
* `arrange(=bill_length_mm)`
* `arrange(+bill_length_mm)`
* `arrange(%>%bill_length_mm)`

> You add the code chunk **`arrange(bill_length_mm)`** to sort the column bill_length_mm in ascending order. The correct code is **`penguins %>% arrange(bill_length_mm)`**. Inside the parentheses of the arrange() function is the name of the variable you want to sort. The code returns a tibble that displays the data for bill_length_mm from shortest to longest. The shortest bill length is 32.1mm.

&nbsp;

### Question 3

A data analyst is working with customer information from their company’s sales data. The first and last names are in separate columns, but they want to create one column with both names instead. Which of the following functions can they use?

* separate()
* **unite()**
* arrange()
* select()

> The unite() function can be used to combine columns. 
