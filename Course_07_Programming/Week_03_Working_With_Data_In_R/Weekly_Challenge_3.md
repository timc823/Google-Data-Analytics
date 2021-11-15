## Weekly challenge 3

Latest Submission Grade: 100%

&nbsp;

### Question 1

A data analyst is considering using tibbles instead of basic data frames. What are some of the limitations of tibbles? Select all that apply.

* Tibbles can overload a console
* **Tibbles can never create row names**
* **Tibbles won’t automatically change the names of variables**
* **Tibbles can never change the input type of the data**

> Tibbles are useful when working with large datasets because they make printing easier. But tibbles can never change the input type of the data, create row names, or change the names of variables. 

&nbsp;

### Question 2

A data analyst wants a quick summary of the structure of their data frame, including the column names and the number of rows and variables. What function should they use?

* colnames()
* head()
* **str()**
* rename_with()

> The str() function returns a summary of the structure of a dataframe, including column names, the number of rows and variables, and the type of data stored. 

&nbsp;

### Question 3

You are working with the ToothGrowth dataset. You want to use the skim_without_charts() function to get a comprehensive view of the dataset. Write the code chunk that will give you this view. 

**`skim_without_charts(ToothGrowth)`**

```
__ Data Summary _____________________________
                           Values
Name                       ToothGrowth
Number of rows             60
Number of columns          3
_______________________
Column type frequency:
  factor                   1
  numeric                  2
________________________
Group variables            None

__ Variable type: factor ________________________________________________________
  skim_variable n_missing complete_rate ordered n_unique top_counts
1 supp                  0             1 FALSE          2 OJ: 30, VC: 30

__ Variable type: numeric _______________________________________________________
  skim_variable n_missing complete_rate  mean    sd    p0   p25   p50   p75  p100
1 len                   0             1 18.8  7.65    4.2  13.1  19.2  25.3  33.9
2 dose                  0             1  1.17 0.629   0.5   0.5   1     2     2
```

How many rows does the ToothGrowth dataset contain? 

* 50
* 40
* 25
* **60**

> The code chunk **`skim_without_charts(ToothGrowth)`** gives you a comprehensive view of the dataset. Inside the parentheses of the skim_without_charts() function is the name of the dataset you want to view. The code returns a summary with the name of the dataset and the number of rows and columns. It also shows the column types and data types contained in the dataset. The ToothGrowth dataset contains 60 rows.

&nbsp;

### Question 4

A data analyst is working with the penguins dataset. What code chunk does the analyst write to make sure all the column names are unique and consistent and contain only letters, numbers, and underscores? 

* `drop_na(penguins)`
* **`clean_names(penguins)`**
* `rename(penguins)`
* `select(penguins)`


> The code chunk is **`clean_names(penguins)`**. The clean_names() function ensures that there are only characters, numbers, and underscores in the names used in the data frame. 

&nbsp;

### Question 5

A data analyst is working with the penguins data. The variable species includes three penguin species: Adelie, Chinstrap, and Gentoo. The analyst wants to create a data frame that only includes the Adelie species. The analyst receives an error message when they run the following code:

```
penguins %>%
    filter(species <- “Adelie”)
```
How can the analyst change the second line of code to correct the error?

* `filter(“Adelie” <- species)`
* `filter(Adelie == species)`
* `filter(“Adelie”)`
* **`filter(species == “Adelie”)`**

> The code chunk is **`filter(species == “Adelie”)`**. The filter function is used to specify the part of the data to be viewed. Two equal signs in an argument mean “exactly equal to.” Using this operator instead of the assignment operator <- calls only the data about Adelie penguins to the dataset.

&nbsp;

### Question 6

Question 6
You are working with the penguins dataset. You want to use the summarize() and mean() functions to find the mean value for the variable body_mass_g. You write the following code:

```
penguins %>% 
  drop_na() %>% 
    group_by(species) %>%
```

Add the code chunk that lets you find the mean value for the variable body_mass_g.

**`summarize(mean(body_mass_g))`**

```
# A tibble: 3 <U+00D7> 2
    species `mean(body_mass_g)`
      <chr>               <dbl>
1    Adelie            3706.164
2 Chinstrap            3733.088
3    Gentoo            5092.437
```
What is the mean body mass in g for the Adelie species? 

* **3706.164**
* 5092.437
* 4207.433
* 3733.088

> The code chunk **`summarize(mean(body_mass_g))`** lets you find the mean value for the variable body_mass_g. The correct code is **`penguins %>% drop_na() %>% group_by(species) %>% summarize(mean(body_mass_g))`**. The summarize() function displays summary statistics. You can use the summarize() function in combination with other functions -- such as mean(), max(), and min() -- to calculate specific statistics. In this case, you use mean() to calculate the mean value for body mass. The mean body mass for the Adelie species is 3706.164g. 

&nbsp;

### Question 7

A data analyst is working with a data frame called salary_data. They want to create a new column named total_wages that adds together data in the standard_wages and overtime_wages columns. What code chunk lets the analyst create the total_wages column? 

* `mutate(total_wages = standard_wages + overtime_wages)`
* `mutate(salary_data, standard_wages = total_wages + overtime_wages)`
* **`mutate(salary_data, total_wages = standard_wages + overtime_wages)`**
* `mutate(salary_data, total_wages = standard_wages * overtime_wages)`

> The code chunk is **`mutate(salary_data, total_wages = standard_wages + overtime_wages)`**. The analyst can use the mutate() function to create a new column for standard_wages plus overtime_wages called total_wages. The mutate() function can create a new column without affecting any existing columns.

&nbsp;

### Question 8

A data analyst is working with a data frame named customers. It has separate columns for area code (area_code) and phone number (phone_num). The analyst wants to combine the two columns into a single column called phone_number, with the area code and phone number separated by a hyphen. What code chunk lets the analyst create the phone_number column? 

* `unite(customers, area_code, phone_num, sep="-")`
* `unite(customers, "phone_number", area_code, phone_num)`
* `unite(customers, "phone_number", area_code, sep="-")`
* **`unite(customers, "phone_number", area_code, phone_num, sep="-")`**

> The code chunk **`unite(customers, "phone_number", area_code, phone_num, sep="-")`**. lets the analyst create the phone_number column. The unite() function lets the analyst combine the area code and phone number data into a single column. In the parentheses of the function, the analyst writes the name of the data frame, then the name of the new column in quotation marks, followed by the names of the two columns they want to combine. Finally, the argument **`sep="-"`** places a hyphen between the area code and phone number data in the phone_number column. 

&nbsp;

### Question 9

A data analyst writes the following code chunk to return a statistical summary of their dataset:
**`quartet %>% group_by(set) %>% summarize(mean(x), sd(x), mean(y), sd(y), cor(x, y))`**
Which function will return the average value of the y column?

* **mean(y)**
* mean(x)
* cor(x, y)
* sd(x)


> The mean() function will return the average value of a specific variable. In this case, mean(y) will return the average value of y. 

&nbsp;

### Question 10

A data analyst wants to find out how much the predicted outcome and the actual outcome of their data model differ. What function can they use to quickly measure this?

* sd()
* **bias()**
* mean()
* cor()

> The bias() function can be used to calculate the average amount a predicted outcome and actual outcome differ in order to determine if the data model is biased. 
