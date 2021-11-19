## Course challenge

Latest Submission Grade: 100%

&nbsp;

## Scenario 1, questions 1-7

### Question 1

As part of the data science team at Gourmet Analytics, you use data analytics to advise companies in the food industry. You clean, organize, and visualize data to arrive at insights that will benefit your clients. As a member of a collaborative team, sharing your analysis with others is an important part of your job. 

Your current client is Chocolate and Tea, an up-and-coming chain of cafes. 

![img](img/chocolate_and_tea.jpg)

The eatery combines an extensive menu of fine teas with chocolate bars from around the world. Their diverse selection includes everything from plantain milk chocolate, to tangerine white chocolate, to dark chocolate with pistachio and fig. The encyclopedic list of chocolate bars is the basis of Chocolate and Tea’s brand appeal. Chocolate bar sales are the main driver of revenue. 

Chocolate and Tea aims to serve chocolate bars that are highly rated by professional critics. They also continually adjust the menu to make sure it reflects the global diversity of chocolate production. The management team regularly updates the chocolate bar list in order to align with the latest ratings and to ensure that the list contains bars from a variety of countries. 

They’ve asked you to collect and analyze data on the latest chocolate ratings. In particular, they’d like to know which countries produce the highest-rated bars of super dark chocolate (a high percentage of cocoa). This data will help them create their next chocolate bar menu. 

Your team has received a dataset that features the latest ratings for thousands of chocolates from around the world. Click [here](https://www.kaggle.com/rtatman/chocolate-bar-ratings) to access the dataset. Given the data and the nature of the work you will do for your client, your team agrees to use R for this project. 

**A teammate asks you about the benefits of using R for the project. You mention that R can quickly process lots of data and create high quality data visualizations. What is another benefit of using R for the project?**

* Define a problem and ask the right questions 
* Automatically clean data 
* Choose a topic for analysis 
* **Easily reproduce and share an analysis**


> Another benefit of using R for the project is R’s ability to create high-quality data visualizations. 

&nbsp;

### Question 2

Before you begin working with your data, you need to import it and save it as a data frame. To get started, you open your RStudio workspace and load the tidyverse library. You upload a .csv file containing the data to RStudio and store it in a project folder named flavors_of_cacao.csv. 

**You use the read_csv() function to import the data from the .csv file. Assume that the name of the data frame is chocolate_df and the .csv file is in the working directory. What code chunk lets you create the data frame?**

* **chocolate_df <-read_csv("flavors_of_cacao.csv")**
* chocolate_df  <- "flavors_of_cacao.csv"(read_csv)
* read_csv("flavors_of_cacao.csv") + chocolate_df
* chocolate_df + read_csv("flavors_of_cacao.csv")

> The code chunk `chocolate_df <- read_csv("flavors_of_cacao.csv")` lets you create the data frame. In this code chunk:
> * `chocolate_df` is the name of the data frame that will store the data. 
> * `<-` is the assignment operator to assign values to the data frame. 
> * `read_csv()` is the function that will import the data to the data frame. 
> * `"flavors_of_cacao.csv"` is the file name that read.csv() function takes for its argument. 

&nbsp;

### Question 3

Now that you’ve created a data frame, you want to find out more about how the data is organized. The data frame has hundreds of rows and lots of columns. 

**Assume the name of your data frame is flavors_df. What code chunk lets you review the structure of the data frame?**


* **`str(flavors_df)`**
* `select(flavors_df)`
* `filter(flavors_df)`
* `summarize(flavors_df)`

> You write the code chunk **`str(flavors_df)`**. In this code chunk:
> * **`str()`** is the function that will return the structure of the data frame, and give you high-level information like the column names and the type of data contained in those columns.
> * **`flavors_df`** is the name of the data frame that the str() function takes for its argument.

&nbsp;

### Question 4

Next, you begin to clean your data. When you check out the column headings in your data frame you notice that the first column is named Company...Maker.if.known. (Note: The period after known is part of the variable name.) For the sake of clarity and consistency, you decide to rename this column Maker (without a period at the end).

**Assume the first part of your code chunk is:**

**`flavors_df %>%`**

**What code chunk do you add to change the column name?**

* `rename(Company...Maker.if.known %<% Maker)`
* **`rename(Maker = Company...Maker.if.known.)`**
* `rename(Company...Maker.if.known. = Maker)`
* `rename(Maker %<% Company...Maker.if.known.)`

> You write the code chunk **`rename(Maker = Company...Maker.if.known.)`**. 
> In this code chunk: 
> * **`rename()`** is the function that will change the name of your column. 
> * Inside the parentheses of the function, write the new name **`(Maker)`**, then an equal sign, then the name you want to change **`(Company...Maker.if.known.)`**.

&nbsp;

### Question 5

After previewing and cleaning your data, you determine what variables are most relevant to your analysis. Your main focus is on Rating, Cocoa.Percent, and Company.Location. You decide to use a function to create a new data frame with only these three variables.

**Assume the first part of your code is:**

**`trimmed_flavors_df <- flavors_df %>%`**

**Add the code chunk that lets you select the three variables.**

```
select(Rating, Cocoa.Percent, Company.Location)
head(trimmed_flavors_df)
```

What company appears in row 1 of your tibble?

* Rogue
* Videri
* **A. Morin**
* Soma
  

> You add the code chunk **`select(Rating, Cocoa.Percent, Company)`** to select the three variables. The correct code is **`trimmed_flavors_df <- flavors_df %>% select(Rating, Cocoa.Percent, Company)`**. In this code chunk:
> * The select() function lets you select specific variables for your new data frame. 
> * select() takes the names of the variables you want to choose as its argument: Rating, Cocoa.Percent, Company.
> 
> The company A. Morin appears in row 1 of your tibble. 

&nbsp;

### Question 6

Next, you select the basic statistics that can help your team better understand the ratings system in your data. 

**Assume the first part of your code is:**

**`trimmed_flavors_df %>%`**

**You want to use the summarize() and mean() functions to find the mean rating for your data. Add the code chunk that lets you find the mean value for the variable Rating.**

```
summarize(mean(Rating))
```

What is the mean rating? 

* 4.701337
* **3.185933**
* 3.995445
* 4.230765


> You add the code chunk **`summarize(mean(Rating))`** to find the mean value for the variable Rating. The correct code is **`trimmed_flavors_df %>% summarize(mean(Rating))`**. In this code chunk:
> * The summarize() function lets you display summary statistics. You can use the summarize() function in combination with other functions such as mean(), sd(), and max() to calculate specific statistics. 
> * In this case, you use mean() to calculate the mean value for the variable Rating. 
> 
> The mean rating is 3.185933.

&nbsp;

### Question 7

After completing your analysis of the rating system, you determine that any rating equal to or greater than 3.9 can be considered a high rating. You also know that Chocolate and Tea considers any bar that contains at least 75% cocoa to be super dark chocolate. You decide to use code to find out which chocolate bars meet these two conditions. 

**Assume the first part of your code is:**

**`best_trimmed_flavors <- trimmed_flavors_df %>%`**

**You want to apply the filter() function to the variables Cocoa.Percent and Rating. Add the code chunk that lets you filter the data frame for chocolate bars that contain at least 70% cocoa and have a rating of at least 3.5 points.**

```
filter(Cocoa.Percent >= 75, Rating >= 3.5)
```

What rating appears in row 1 of your tibble? 

* **3.50**
* 4.00
* 3.75
* 4.25


> The code chunk **`filter(Cocoa.Percent >= 70, Rating >= 3.5)`** lets you filter the data frame for chocolate bars that contain at least 70% cocoa and have a rating of at least 3.5 points. The correct code is **`best_trimmed_flavors_df <- trimmed_flavors_df %>% filter(Cocoa.Percent >= 70, Rating >= 3.5)`**. In this code chunk: 
> * The filter() function lets you filter your data frame based on specific criteria. 
> * Cocoa.Percent and Rating refer to the variables you want to filter. 
> * The >= operator signifies “greater than or equal to.” 
> * The new data frame will show all the values of Cocoa.Percent greater than or equal to 70, and all the values of Rating greater than or equal to 3.5.  
>
> The rating 3.50 appears in row 1 of your tibble.

&nbsp;
<hr>
&nbsp;

## Scenario 2, questions 8-13

### Question 8

Now that you’ve cleaned and organized your data, you’re ready to create some useful data visualizations. Your team assigns you the task of creating a series of visualizations based on requests from the Chocolate and Tea management team. You decide to use ggplot2 to create your visuals. 

**Assume the first line of your code is:**

**`ggplot(data = best_trimmed_flavors_df) +`**

**You want to use the geom_bar() function to create a bar chart. Add the code chunk that lets you create a bar chart with the variable Company on the x-axis.**

```
geom_bar(aes(x=Company)) 
```

How many bars does your bar chart display? 

* **8**
* 6
* 4
* 10

> You add the code chunk **`geom_bar(mapping = aes(x = Company))`** to create a bar chart with the variable Company on the x-axis. The correct code is **`ggplot(data = best_trimmed_flavors_df) + geom_bar(mapping = aes(x = Company))`**. In this code chunk:
> * geom_bar() is the geom function that uses bars to create a bar chart. 
> * Inside the parentheses of the aes() function, the code **`x = Company`** maps the x aesthetic to the variable Company. 
> * Company will appear on the x-axis of the plot. 
> * By default, R will put a count of the variable Company on the y-axis. 
>
> Your bar chart displays 8 bars.
 
&nbsp;

### Question 9

Your bar chart reveals the locations that produce the highest rated chocolate bars. To get a better idea of the specific rating for each location, you’d like to highlight each bar.

**Assume that you are working with the following code:**
```
ggplot(data = best_trimmed_flavors_df) +

  geom_bar(mapping = aes(x = Company.Location))
```
**Add a code chunk to the second line of code to map the aesthetic fill to the variable Rating.**

**NOTE: the three dots (...) indicate where to add the code chunk.**

```
geom_bar(mapping = aes(x = Company.Location, fill= Rating))
```

**According to your bar chart, which two company locations produce the highest rated chocolate bars?**


* Scotland and U.S.A.
* Amsterdam and France
* **Canada and France**
* Scotland and Canada


> You add the code chunk **`fill = Rating`** to the second line of code to map the aesthetic fill to the variable Rating. The correct code is **`ggplot(data = best_trimmed_flavors_df) + geom_bar(mapping = aes(x = Company.Location, fill = Rating))`**. In this code chunk: 
> * Inside the parentheses of the aes() function, after the comma that follows x = Company.Location, write the aesthetic (fill), then an equals sign, then the variable (Rating).
> * The specific rating of each location will appear as a specific color inside each bar of your bar chart.
>
> On your visualization, the legend titled "Rating" shows the color coding for the variable Rating. Lighter blues correspond to higher ratings and darker blues correspond to lower ratings.
>
> According to your bar chart, the two company locations that produce the highest rated chocolate bars are Canada and France. 


&nbsp;

### Question 10

A teammate creates a new plot based on the chocolate bar data. The teammate asks you to make some revisions to their code. 

**Assume your teammate shares the following code chunk:**
```
ggplot(data = best_trimmed_flavors_df) +

     geom_bar(mapping = aes(x = Rating)) +
```
**What code chunk do you add to the third line to create wrap around facets of the variable Rating?** 


* `facet_wrap(Rating)`
* `facet(~Rating)`
* `facet_wrap(Rating~)`
* **`facet_wrap(~Rating)`**


> You write the code chunk facet_wrap**`(~Rating)`**. In this code chunk: 
> * **`facet_wrap()`** is the function that lets you create wrap around facets of a variable.
> * Inside the parentheses of the **`facet_wrap()`** function, type a tilde symbol (~) followed by the name of the variable **`(Rating)`**. 

&nbsp;

### Question 11

Your team has created some basic visualizations to explore different aspects of the chocolate bar data. You’ve volunteered to add titles to the plots. You begin with a scatterplot. 

**Assume the first part of your code chunk is:**
```
ggplot(data = trimmed_flavors_df) +

     geom_point(mapping = aes(x = Cocoa.Percent, y = Rating)) +
```
**What code chunk do you add to the third line to add the title Best Chocolates to your plot?**

* `labs(title <- "Best Chocolates")`
* **`labs(title = “Best Chocolates”)`**
* `labs("Best Chocolates")`
* `labs("Best Chocolates" = title)`


> You write the code chunk **`labs(title = “Best Chocolates”)`**. In this code chunk: 
> * **`labs()`** is the function that lets you add a title to your plot. 
> * In the parentheses of the **`labs()`** function, write the word title, then an equals sign, then the specific text of the title in quotation marks **`(“Best Chocolates”)`**. 

&nbsp;

### Question 12

Next, you create a new scatterplot to explore the relationship between different variables. You want to save your plot so you can access it later on. You know that the ggsave() function defaults to saving the last plot that you displayed in RStudio, so you’re ready to write the code to save your scatterplot.  

**Assume your first two lines of code are:**
```
ggplot(data = trimmed_flavors_df) +

  geom_point(mapping = aes(x = Cocoa.Percent, y = Rating)) +
```
**What code chunk do you add to the third line to save your plot as a pdf file with “chocolate” as the file name?**

* `ggsave(chocolate.pdf)`
* `ggsave("pdf.chocolate")`
* **`ggsave("chocolate.pdf")`** 
* `ggsave("chocolate.png")`

> You add the code chunk **`ggsave("chocolate.pdf")`** to save your plot as a pdf file with "chocolate" as the file name. In this code chunk: 
> * Inside the parentheses of the ggsave() function, type a quotation mark followed by the file name (chocolate), then a period, then the type of file format (pdf), then a closing quotation mark.

&nbsp;

### Question 13

As a final step in the analysis process, you create a report to document and share your work. Before you share your work with the management team at Chocolate and Tea, you are going to meet with your team and get feedback. Your team wants the documentation to include all your code and display all your visualizations. 

**You decide to create an R Markdown notebook to document your work. What are your reasons for choosing an R Markdown notebook? Select all that apply.**

* **It displays your data visualizations**
* **It allows users to run your code** 
* **It lets you record and share every step of your analysis**
* It automatically creates a website to show your work 

> You choose an R Markdown notebook to document your work because it lets you record and share every step of your analysis. The notebook allows users to run your code and also displays your data visualizations. 
