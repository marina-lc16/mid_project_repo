**EDA and Visualization project**

**DATA SCIENCE JOBS: SALARIES AND TYPE OF WORKS MODELS**


**Introduction 📝:**

In recent years, data science roles are more demanded, so it's important to understand how they are evolving in terms of positioning as job offers and their salaries.

In this analysis, I will take my first Exploratory Data Analysis (EDA) and visualization project using Python and Tableau, where I explored data science jobs titles and salaries between 2020 and 2023. 

The "global salary index" dataset comes from the ai-jobs.net website for roles in the AI, ML, Data Science space based on internal data obtained from surveys and jobs with open salaries.

This dataset is processed and updated on a weekly basis, but I'll take the dataset updated on September 29th, 2023.

Data: The "global salary index" dataset comes from the ai-jobs.net website for roles in the AI, ML, Data Science space based on internal data obtained from surveys and jobs with open salaries and is processed and updated on a weekly basis, but I'll take the dataset updated on September 29th, 2023.

**Hypotheses 💡:**

What I want to find out with this analysis is to extract the following data from my data set:

- Top 3 highest-payed roles for each year and evaluate the changes between 2020-2023 

- Which level of experience has the most representation

- Evaluate the working model followed per year of work

- "Remote\_ratio VS company\_size": The size of the company influences in the overall amount of work done remotely? 

- "Remote\_ratios VS Salary": Which kind of "type of work" has the highest salaries on 2023? has this changed over the years?

- "Remote\_ratios VS location": create a visualization map to view remote ratios by job areas, year, company size and location



**Dataset details 🔎:**

Here we can find the detail of all the data included

https://ai-jobs.net/salaries/download/


work\_year			The year the salary was paid.


experience\_level	The experience level in the job during the year with the following possible values:

**EN**	Entry-level / Junior

**MI**	Mid-level / Intermediate

**SE**	Senior-level / Expert

**EX**	Executive-level / Director


employment\_type		The type of employement for the role:

**PT**	Part-time

**FT**	Full-time

**CT**	Contract

**FL**	Freelance


job\_title			The role worked in during the year.


salary				The total gross salary amount paid.


salary\_currency	The currency of the salary paid as an ISO 4217 currency code.


salary\_in\_usd	The salary in USD (FX rate divided by avg. USD rate of respective year) via statistical data from the BIS and central banks.


employee\_residence	Employee's primary country of residence in during the work year as an ISO 3166 country code.


remote\_ratio	The overall amount of work done remotely, possible values are as follows:

**0**	No remote work (less than 20%)

**50**	Partially remote/hybird

**100**	Fully remote (more than 80%)


company\_location	The country of the employer's main office or contracting branch as an ISO 3166 country code.


company\_size	The average number of people that worked for the company during the year:

**S**	less than 50 employees (small)

**M**	50 to 250 employees (medium)

**L**	more than 250 employees (large)




**Exploratory Data Analysis (EDA) **



**Finding all variables and understanding them 🔎:**

To start my analysis, I was to get an overview of my data set. I exported and read the file on the jupyter notebook and examined its contents: size, columns and rows distributions to see the information it contained, i.e. the distribution of roles(job\_titles) and salaries (in USD) according to company size, experience levels, employee and company location or proportion of remote work ratio.

To do this I used the functions pd.read, head(), shape(), info(), describe() and df.columns and I explored if the dataset had missing values and the unique values for each column.



**Preprocessing: Data cleaning and reduction 🕵️‍♀️:**

Once I got all the overall information I could start working with the data and think about what changes I could make to clean it up, transform it and ensure more meaningful consistency of certain values.

The data set contains two types of variables in the columns, numerical and categorical, and I split them to process the data.

I first cleaned the numerical columns and then the categorical ones.



**Cleaning numerical:**

During the cleaning of the numerical columns, to make a more concrete analysis, the "salary" column was deleted and only the "salary\_in\_usd" column was left to have all the data in the same currency.

In addition, during the analysis of the numerical columns, it highlighted that in the columns "job\_year" and "salary" there is an asymmetry on the left and right, respectively. That means a large difference between the job/salary numbers between 2020 and 2023, probably the data collection probably started at the end of 2020.



**Cleaning categorical:**

The cleaning and reduction of the categorical data was more extensive.

Looking at the values included in each column could be seen that some of them may be confusing.

The columns affected were:

\- "experience\_level"

\- "employment\_type"

\- "employee\_residence"

\- "remote\_ratio"

\- "company\_location"

\- "company\_size"

All coded data were replaced by their actual meaning, and, in addition, the "job\_title" column had a high cardinality, having more than 100 distinct values, so a new column was created grouping the data by "area".

Once the cleaned data were obtained, a new data set was created.



**Data visualization with Tableau 📊:** 

With the new clean dataset could started working with the Data visualization, the process of graphical representation of information and data, by using visual elements like charts, graphs, and maps, and data visualization tools like Python or Tableau that provide an accessible way to see and understand patterns, trends, and outliers in data.



**Results 🚀:**

Nowadays, data science roles are one of the most in-demand and are rapidly growing. 

In this short project (Notebook + Tableau public) I covered the data science field salaries and how the work remote ratio has been changing from 2020 to 2023.

When we look the data and visual graphs from Tableau Public, we can see that:

- The popularity of data science jobs continues
- The majority of the data is based in the **United States** 
- **United States, UK and Canada** are the countries with more representation in the data science sector and has the highest salaries
- The highest-payed jobs are from **Analytics**
- **Senior-level experience** has been growing probably because those who started in 2020 have already reached this level 
- One thing that stands out is how the work **remote ratio has dropped** again after the pandemic although it has grown among smaller companies, possibly related to the cost of having on-site employees (offices, transport…)
- It’s currently striking that the highest salaries correspond to "on-site" employees; it would be necessary to confirm whether this is an error in the data collection or whether it is the reality.

In my opinion, after performing this analysis I believe that getting a role related to data science is a good career option in terms of salary and remote options, but, even so, at the remote work level we should not take this result for granted, since many times a job is indicated as on-site, when it has a remote (hybrid) part, so it is possible that the real data is different.


**Link to GitHub Repository:**

**https://github.com/marina-lc16/mid_project/tree/main**
