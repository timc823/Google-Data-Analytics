## Course challenge

Latest Submission Grade: 100%

&nbsp;

## Scenario 1, questions 1-5

### Question 1

You are a data analyst at a small analytics company. Your company is hosting a project kick-off meeting with a new client, Meer-Kitty Interior Design. The agenda includes reviewing their goals for the year, answering any questions, and discussing their available data. 

Before the meeting you review the About Us tab on their website and their business plan, linked below:

[Meer_Kitty Interior Design About Us Page.pdf](files/Meer_Kitty_Interior_Design_About_Us_Page.pdf)

[Meer_Kitty Interior Design Business Plan.pdf](files/Meer_Kitty_Interior_Design_Business_Plan.pdf)

Meer-Kitty Interior Design has two goals. They want to expand their online audience, which means getting their company and brand known by as many people as possible. They also want to launch a line of high-quality indoor paint to be sold in-store and online. You decide to consider the data about indoor paint first. 

You may click the link to create a copy of the dataset: Kitty Survey Feedback. Please refer to the Meer-Kitty survey feedback tab.

[Kitty Survey Feedback - Meer_Kitty survey feedback.csv](files/Kitty_Survey_Feedback_Meer_Kitty_Survey_Feedback.csv)

You are pleased to find that the available data is aligned to the business objective. However, you do some research about confidence level for this type of survey and learn that you need at least 120 unique responses for the survey results to be useful. Therefore, the dataset has two limitations: First, there are only 40 responses; second, a Meer-Kitty superfan, User 588, completed the survey 11 times. 

**As the survey has too few responses and numerous duplicates that are skewing results, you decide to repeat the survey in order to create a new, improved dataset. What is your first step?**

* Find a survey tool that only allows someone to complete the survey once.
* **Talk with stakeholders, explain the new timeline, and ask for approval.** 
* Delete all of the data from the current, skewed survey.
* Write new, improved survey questions.

> Before repeating the survey, it’s necessary to talk with stakeholders, explain the new timeline, and ask for approval. 

&nbsp;

### Question 2

During the meeting, you also learn that Meer-Kitty videos are hosted on their website. For each product offered, there is an accompanying video for customers to learn more. So, more views for a video suggests greater consumer interest. 

Your goal is to identify which videos are most popular, so Meer-Kitty knows what topics to explore in the future. Unfortunately, Meer-Kitty has just three months of data available because they only recently launched the videos on their site. 

**Without enough data to identify long-term trends about the video subjects that people prefer, what are your available options? Select all that apply.**

* Ask to wait for more data and provide Meer-Kitty with an updated timeline.
* Talk with Meer-Kitty stakeholders and ask to adjust the objective. 
* Watch the videos and use your gut instinct to identify which are most successful.
* Move ahead with the data you have to determine the top video subjects.

> Without enough data to identify long-term trends, one option is to talk with stakeholders and ask to adjust the objective. You could also ask to wait for more data and provide an updated timeline.

&nbsp;

### Question 3

Now that you’ve identified some limitations with Meer-Kitty’s data, you want to communicate your concerns to stakeholders. In addition to insufficient video trend data, your main concern with the indoor paint survey is that the data isn’t representative of the population as a whole. 

**Clearly, one particular respondent, the superfan, is overrepresented. What does this situation describe?**


* Statistical significance
* Margin of error
* Confidence level
* **Sampling bias**

> This situation describes sampling bias. Sampling bias occurs when a sample isn’t representative of the population as a whole.

&nbsp;

### Question 4

The stakeholders understand your concerns and agree to repeat the indoor paint survey. In a few weeks, you have a much better dataset with more than 150 responses and no duplicates. 

[Kitty Survey Feedback - New Meer-Kitty survey feedback.csv](files/Kitty-Survey-Feedback---New-Meer-Kitty-survey-feedback.csv)

You notice that questions 4 and 5 are dependent on the respondent’s answer to question 3. So, you need to determine how many people answered Yes to question 3, then compare that to responses to questions 4 and 5. That way, you will know if questions 4 and 5 have any nulls.

**You decide to use a spreadsheet tool that changes how cells appear when they contain the word Yes. When using this tool, what is the word Yes?**

* **The value in a conditional formatting rule**
* The value in a VLOOKUP statement
* The value in a CONCATENATE range
* The value in the COUNTA range

> To change how cells appear when they meet a certain value, use conditional formatting. 

&nbsp;

### Question 5

You have finished cleaning the data to ensure it is complete, correct, and relevant to the problem you’re trying to solve. Then, you complete the verification and reporting processes to share the details of your data-cleaning effort with your team. 

Your team notes one aspect of data cleaning that would help improve the dataset. They point out that the new survey also has a new question in Column G: “What are your favorite indoor paint colors?” This was a free-response question, so respondents typed in their answers. Some people included multiple different colors of paint. In order to determine which colors are most popular, it will be necessary to put each color in its own cell.

**You decide to use a spreadsheet function to divide the text strings in Column G around the commas and put each fragment into a new, separate cell. You are using the SPLIT function.**

* **True**
* False

> To divide the text strings in Column G around the commas and put each fragment into a new, separate cell, you use SPLIT. SPLIT is a spreadsheet function that divides text around a specified character and puts each fragment into a new, separate cell.

&nbsp;

## Scenario 2, questions 6-10

### Question 6

You’ve completed this program and are interviewing for a junior data scientist position. The job is at B.Spoke Market Research, a company that analyzes market conditions using customer surveys and other research methods. The detailed job description can be found below:

[C4 B.Spoke Market Research Job Description.pdf](files/C4_B.Spoke_Market_Research_Job_Description.pdf)

So far, you’ve had a phone interview with a recruiter and you’ve secured a second interview with the B.Spoke team. The recruiter’s email can be found below:

[C4 S2 Email from Recruiter.pdf](files/C4_S2_Email_From_Recruiter.pdf)

You arrive 15 minutes early for your interview. Soon, you are escorted into a conference room, where you meet Jodie Choi, the data science lead. After welcoming you, the behavioral interview begins. 

For your first question, your interviewer wants to learn about your experience with spreadsheets. She says: Sometimes the team needs data that is stored in different spreadsheets. So, we use a spreadsheet function to find the information we need.

**There is a spreadsheet function that searches for a value in the first column of a given range and returns the value of a specified cell in the row in which it is found. It is called SEARCH.**

* True
* **False**

> The VLOOKUP function searches for a certain value in a column to return a corresponding piece of information.

&nbsp;

### Question 7

Next, your interviewer wants to know more about your understanding of tools that work in both spreadsheets and SQL queries. She explains that the data her team receives from customer surveys sometimes has many duplicate entries. 

**She says: Spreadsheets have a great tool for that called remove duplicates. But when writing a SQL query, what command should you include in your SELECT statement to remove duplicates?**

* DISCRETE
* DIVERSE
* **DISTINCT**
* DIFFERENT

> To remove duplicates in a SQL query, include DISTINCT in your SELECT statement.

&nbsp;

### Question 8

Now, your interviewer explains that the data team usually works with very large amounts of customer survey data. After receiving the data, they import it into a SQL table. But sometimes, the new dataset imports incorrectly and they need to change the format. 

**She asks: Is there a command or function that converts data in a SQL table from one datatype to another? You respond: Yes, it’s the CAST function.**

* True
* False

> The CAST function is used to convert data in a SQL table from one datatype to another. 

&nbsp;

### Question 9

Next, your interviewer explains that one of their clients is an online retailer that needs to create product numbers for a vast inventory. Her team does this by combining the text strings for product number, manufacturing date, and color. 

**She asks: If you encountered a situation where you wanted to add strings together to create new text strings, which SQL function would you use?**

* COMBINE
* CREATE
* COALESCE
* **CONCAT**

> To add strings together to create new text strings, use the CONCAT function.

&nbsp;

### Question 10

For your final question, your interviewer explains that her team often comes across data with extra spaces. 

**She asks: Which function would enable you to eliminate those extra spaces? You respond: To eliminate extra spaces for consistency, use the TRIM function.**

* **True**
* False

> To eliminate extra spaces for consistency, use the TRIM function. 
