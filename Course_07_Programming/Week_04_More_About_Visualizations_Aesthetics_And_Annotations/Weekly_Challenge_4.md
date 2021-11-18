## Weekly challenge 4

Latest Submission Grade: 100%

&nbsp;

### Question 1

Which of the following are benefits of using ggplot2? Select all that apply. 

* Automatically clean data before creating a plot
* **Easily add layers to your plot** 
* **Combine data manipulation and visualization** 
* **Customize the look and feel of your plot** 

> The benefits of using ggplot2 include easily adding layers to your plot, customizing the look and feel of your plot, combining data manipulation and visualization.

&nbsp;

### Question 2

In ggplot2, what symbol do you use to add layers to your plot?

* The equal sign (=)
* The ampersand symbol (&)
* The pipe operator (%>%)
* **The plus sign (+)**

> In ggplot2, you use the plus sign (+) to add layers to your plot.

&nbsp;

### Question 3

A data analyst creates a plot using the following code chunk: 

```
ggplot(data = penguins) + 
    geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g))
```

Which of the following represents a variable in the code chunk? Select all that apply. 

* **`body_mass_g`**
* `x`
* **`flipper_length_mm`**
* `y`

> The two variables in the code are flipper_length_mm and body_mass_g. The two variables are part of the penguins dataset. The aesthetic x maps the variable flipper_length_mm to the x-axis of the plot. The aesthetic y maps the variable body_mass_g to the y-axis of the plot.

&nbsp;

### Question 4

In ggplot2, which of the following aesthetic attributes can you use to map variables to points? Select all that apply. 

**Size**
**Color**
Facet
**Shape**


> In ggplot2, color, shape, and size are aesthetic attributes you can use to map variables to points. Color refers to the color of the points on your plot, shape to the shape of the points, and size to the size of the points. 

&nbsp;

### Question 5

A data analyst is working with the penguins data. The analyst creates a scatterplot with the following code: 

```
ggplot(data = penguins) + 
    geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g,alpha = species))
```

What does the alpha aesthetic do to the appearance of the points on the plot? 

* **Makes some points on the plot more transparent**
* Makes the points on the plot more colorful 
* Makes the points on the plot smaller
* Makes the points on the plot larger 

> The alpha aesthetic makes some points on a plot more transparent, or see-through, than others.

&nbsp;

### Question 6

You are working with the penguins dataset. You create a scatterplot with the following code: 
```
ggplot(data = penguins) +

  geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g))
```
You want to highlight the different penguin species on your plot. Add a code chunk to the second line of code to map the aesthetic shape to the variable species.

`geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g, ...))` 

NOTE: the three dots (...) indicate where to add the code chunk.

` ... = shape = species`

Which penguin species does your visualization display?

* Adelie, Chinstrap, Emperor
* Adelie, Gentoo, Macaroni 
* **Adelie, Chinstrap, Gentoo**
* Emperor, Chinstrap, Gentoo

> You add the code chunk shape = species to the second line of code to map the aesthetic shape to the variable species. The correct code is ggplot(data = penguins) + geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g, shape = species)). Inside the parentheses of the aes() function, after the comma that follows  y = body_mass_g, write the aesthetic (shape), then an equals sign, then the variable (species). The data points for each penguin species now appear in different shapes. 

> Your visualization displays the Adelie, Chinstrap, and Gentoo penguin species.

&nbsp;

### Question 7

A data analyst creates a plot with the following code chunk: 
```
ggplot(data = penguins) + 
  geom_jitter(mapping = aes(x = flipper_length_mm, y = body_mass_g))
```
What does the geom_jitter() function do to the points in the plot?

* Decrease the size of each point in the plot 
* Adds random colors to each point in the plot 
* **Adds a small amount of random noise to each point in the plot** 
* Adds a small amount of random shapes at each point in the plot

> The geom_jitter() function creates a scatterplot and then adds a small amount of random noise to each point in the plot to make the points easier to find.

&nbsp;

### Question 8

You are working with the diamonds dataset. You create a bar chart with the following code:
```
ggplot(data = diamonds) +

  geom_bar(mapping = aes(x = color, fill = cut)) +
```

You want to use the facet_wrap() function to display subsets of your data. Add the code chunk that lets you facet your plot based on the variable color. 

`facet_wrap(~color)`

How many subplots does your visualization show?

* 9
* 6
* 8
* **7**


> You add the code chunk **`facet_wrap(~color)`** to facet your plot based on the variable color. The correct code is **`ggplot(data = diamonds) + geom_bar(mapping = aes(x = color, fill = cut)) + facet_wrap(~color)`**. Inside the parentheses of the facet_wrap() function, write a tilde symbol (~) followed by the name of the variable you want to facet. The facet_wrap() function lets you display subsets of your data.

> Your visualization shows 7 subplots. 

&nbsp;

### Question 9

A data analyst creates a scatterplot. The analyst wants to put a text label on the plot to call out specific data points. What function does the analyst use?

* The ggplot() function 
* **The annotate() function** 
* The geom_smooth() function 
* The facet_grid() function 

> The analyst uses the annotate() function. The annotate() function can put a text label on a plot to call out specific data points. 


&nbsp;

### Question 10

You are working with the penguins dataset. You create a scatterplot with the following lines of code: 
```
ggplot(data = penguins) + 

  geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g)) + 
```

What code chunk do you add to the third line to save your plot as a pdf file with “penguins” as the file name? 

* ggsave(penguins.pdf)
* ggsave(“pdf.penguins”)
* ggsave(=penguins)
* **ggsave(“penguins.pdf”)**

> You add the code chunk **`ggsave(“penguins.pdf”)`** to save your plot as a pdf file with “penguins” as the file name. Inside the parentheses of the ggsave() function, type a quotation mark followed by the file name (penguins), then a period, then the type of file (pdf), then a closing quotation mark. 
