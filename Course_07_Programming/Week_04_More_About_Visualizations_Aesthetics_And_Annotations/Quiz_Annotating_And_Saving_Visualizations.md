## L4 Annotating and saving visualizations

&nbsp;

### Question 1

Which of the following are benefits of adding labels and annotations to your plot? Select all that apply. 

* **Indicating the main purpose of your plot** 
* **Helping stakeholders quickly understand your plot**
* **Highlighting important data in your plot**
* Choosing a geom for your plot 

&nbsp;

### Question 2

A data analyst is creating a plot for a presentation to stakeholders. The analyst wants to add a title, subtitle, and caption to the plot to help communicate important information. What function could the analyst use? 

* The geom_bar() function
* The facet_wrap() function
* The geom_point() function
* **The labs() function**

> The analyst could use the labs() function to add a title, subtitle, and caption to the plot.

&nbsp;

### Question 3

What function can you use to put a text label inside the grid of your plot to call out specific data points? 

* **The annotate() function**
* The labs() function
* The aes() function 
* The facet_wrap() function

> You can use the annotate() function to put a text label inside the grid of your plot to call out specific data points.

&nbsp;

### Question 4

You are working with the penguins dataset. You create a scatterplot with the following code:

```
ggplot(data = penguins) + 

geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g)) +
```

You want to use the labs() function to add the title “Penguins” to your plot. Add the code chunk that lets you add the title "Penguins" to your plot.

**`labs(title = “Penguins”)`**

Where does your visualization display the title?

* The lower right
* **The upper left**
* The lower left
* The upper right

> You add the code chunk labs(title = “Penguins”) to add the title "Penguins" to your plot. Inside the parentheses of the labs() function, write the word title, then an equals sign, then the specific text of the title in quotation marks. The labs() function lets you add labels to your plot. 

> Your visualization displays the title in the upper left. 
