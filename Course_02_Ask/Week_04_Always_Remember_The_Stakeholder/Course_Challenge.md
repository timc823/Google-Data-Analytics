## Course challenge

Latest Submission Grade: 100%

&nbsp;

## Scenario 1, questions 1-5


### Question 1

You’ve just started a job as a data analyst at a small software company that provides data analytics and business intelligence solutions. Your supervisor asks you to kick off a project with a new client, Athena’s Story, a feminist bookstore. They have four existing locations, and the fifth shop has just opened in your community.

Athena’s Story wants to produce a campaign to generate excitement for an upcoming celebration and introduce the bookstore to the community. They share some data with your team to help make the event as successful as possible.

Your task is to review the assignment and the available data, then present your approach to your supervisor.

[Scenario_1_Email_From_Supervisor](reources/Scenario_1_Email_From_Supervisor.pdf)

Then, review the email, and review the Customer Survey and Historical Sales datasets: 

* You may click the link to create a copy of the dataset: [Customer Survey](resources/CustomerSurvey.csv)
* You may click the link to create a copy of the dataset [Historical Sales](resources/HistoricalSales.csv)

After reading the email, you notice that the acronym WHM appears in multiple places. You look it up online, and the most common result is web host manager. That doesn’t seem right to you, as it doesn’t fit the context of a feminist bookstore. **How do you proceed?**

* Call the client to ask what WHM means and inform them that using acronyms is not a professional business practice.
* Proceed with the project assuming WHM must mean web host manager.
* Schedule a meeting with your supervisor, the client, and another analyst on your team to figure out the meaning.
* **Send your supervisor a polite, concise email, asking them to confirm the meaning of WHM.**

> You should send your supervisor a polite, concise email, asking them to confirm the meaning of WHM.

&nbsp;

### Question 2

Scenario 1 continued
Now that you know WHM stands for Women’s History Month, you continue reviewing the datasets. You notice the [Customer Survey](resources/CustomerSurvey.csv) dataset contains both qualitative and quantitative data. 

**The quantitative data includes information from which columns? Select all that apply.**

* **Column C (Survey Q3: Do you purchase feminist books in honor of WHM, either for yourself or as a gift for someone else?)** 
* **Column A (Survey Q1: Do you plan to celebrate WHM?)**
* **Column D (Survey Q4: If answered "Yes" to Q3, how many books do you typically purchase during March?)**
* Column E (Survey Q5: What do you like most about Athena's Story?)

> The qualitative data includes information from columns B, E, and F.

&nbsp;

### Question 3

Next, you review the customer feedback in column F of the Customer Survey (link to download CSV instead below).
CustomerSurvey - CustomerSurvey.csv

The attribute of column F is, “Survey Q6: What types of books would you like to see more of at Athena's Story?” In order to verify that children’s literature and feminist zines are among the most popular genres, you create a visualization. This will help you clearly identify which genres are most likely to sell well during the Women’s History Month campaign. 

Your visualization looks like this:

![img](img/chart.png)

**The chart you create demonstrates the percentages of each book genre that make up the whole. It’s called an area chart.**

* True
* **False**

> It’s called a pie chart. Pie charts are effective at demonstrating the percentages of a whole, such as the percentage of customers who would be interested in purchasing books of different genres.

&nbsp;

### Question 4

Now that you’ve confirmed that children’s literature and feminist zines are among the most requested book genres, you review the [Historical Sales](resources/HistoricalSales.csv).  

You’re pleased to see that columns D and E have something in common: They both contain data that’s specific to children’s literature and feminist zines. This will provide you with the information you need to make data-inspired decisions. In addition, the children’s literature and feminist zines metrics will help you organize and analyze the data about each genre in order to determine if they’re likely to be profitable.

**Next, you calculate the total sales over 52 weeks for feminist zines. You type =CALCULATE(E2-E53) but get an error. What is the correct syntax?**


* =COUNT(E2:E53)
* =MAX(E2:E53)
* **=SUM(E2:E53)**
* =CALC(E2:E53)

> The correct syntax is =SUM(E2:E53). The SUM function adds the values of a range of cells. E2:E53 is the specified range.

&nbsp;

### Question 5

After familiarizing yourself with the project and available data, you present your approach to your supervisor. You provide a scope of work, which includes important details, a schedule, and information on how you plan to prepare and validate the data. You also share some of your initial results and the pie chart you created. 

In addition, you identify the problem type, or domain, for the data analysis project. You decide that the historical sales data can be used to provide insights into the types of books that will sell best during Women’s History Month this coming year. This will also enable you to determine if Athena’s Story should begin selling more children’s literature and feminist zines.

**Using historical data to make informed decisions about how things may be in the future is an example of discovering connections.**

* True
* **False**

> Using historical data to make informed decisions about how things may be in the future is an example of making predictions.

&nbsp;

## Scenario 2, questions 6-10

### Question 6
[Customer Survey](resources/CustomerSurvey.csv)


You’ve completed this program and are now interviewing for your first junior data analyst position. You’re hoping to be hired by an event planning company, Patel Events Plus. Access the job description below:


[Junior Data Scientist Job Description](resources/Junior_Data_Scientist_Job_Description.pdf)


So far, you’ve successfully completed the first round of interviews with the human resources manager and director of data and strategy. Now, the vice president of data and strategy wants to learn more about your approach to managing projects and clients. Access the email you receive from the human resources director below: 


[Human Resources Director Email](resources/Human_Resources_Director_Email.pdf)

You arrive Thursday at 1:45 PM for your 2 PM interview. Soon, you’re taken into the office of Mila Aronowicz, vice president of data and strategy. After welcoming you, she begins the behavioral interview. 

First, she hands you a copy of Patel Events Plus’s organizational chart. Access the chart below:

[Patel Event Plus Org Chart](resources/Patel_Event_Plus_Org_Chart.pdf)

As you’ve learned in this course, stakeholders are people who invest time, interest, and resources into the projects you’ll be working on as a data analyst. Let’s say you’re working on a project involving data and strategy. **Based on what you find in the organizational chart, if you need information from the primary stakeholder, who can you ask?**


* Chief executive officer
* **Vice president, data and strategy**
* Project manager, analytics
* Director, strategy

> If you need information from the primary stakeholder, you can ask the vice president of data and strategy. 

&nbsp;

### Question 7

Next, the vice president wants to understand your knowledge about asking effective questions. Consider and respond to the following question. Select all that apply.

**Let’s say we just completed a big event for a client and wanted to find out if they were satisfied with their experience. Provide some examples of measurable questions that you could include in the customer feedback survey.**

* Why did you enjoy the event planned by Patel Events Plus?
* **Would you recommend Patel Events Plus to a colleague or friend? Yes or no?**
* **On a scale from 1 to 5, with 1 being not at all likely and 5 being very likely, how likely are you to recommend Patel Events Plus?**
* How would you describe your event experience?

> In the SMART methodology, measurable questions can be quantified and assessed. This might include a 1-to-5 scale or questions with yes-or-no responses.

&nbsp;

### Question 8

Now, the vice president presents a situation having to do with resolving challenges and meeting stakeholder expectations. Consider and respond to the following question.

**You’re working on a rush project, and you discover your dataset is not clean. Even though it has numerous nulls, redundant data, and other issues, the primary stakeholder insists that you move ahead and use it anyway. The project timeline is so tight that there simply isn’t enough time for cleaning. How would you handle that situation?**

* **Communicate the situation to your supervisor and ask for advice on how to handle the situation with the stakeholder.**
* Clean the data as quickly as you can. It’s not perfect, but it’s better than it was before, and this way you can meet the deadline.
* The stakeholder is in charge. It's best to do as they say and use the unclean dataset.
* Contact the stakeholder’s boss to let them know about the issue and ask for help managing the stakeholder’s expectations.


> This situation presents an opportunity to communicate, collaborate, and foster positive working relationships. 

&nbsp;

### Question 9

Your next interview question deals with sharing information with stakeholders. Consider and respond to the following question. 

**Let’s say you’ve designed a dashboard to give stakeholders easy, automatic access to data about an upcoming event. Describe the benefits of using a dashboard.**

* **Dashboards enable stakeholders to interact with the data.** 
* Dashboards are easy to design and understand.
* Dashboards present pre-cleaned, historical data.
* **Dashboards offer live monitoring of incoming data.**


> Dashboards offer live monitoring of incoming data and enable stakeholders to interact with the data.

&nbsp;

### Question 10

Your final behavioral interview question involves using metrics to answer business questions. Your interviewer hands you a copy of [Patel Events Data](resources/PatelEventsData.csv). 

Then, she asks:

Recently, Patel Events Plus purchased a new venue for our events. **If we asked you to calculate the return on investment of this purchase, which metrics would you use?**

* Purchase date
* 2019 events held at new venue (column D)
* **Net profit in 2019 (column F)**
* **Purchase price (column C)**

> Return on investment is made up of two metrics: the net profit over a period of time and the cost of the investment. By comparing these two metrics, you can determine the profitability of the investment.
