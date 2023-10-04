EDA and Visualization project

**DATA SCIENCE JOBS: SALARIES AND TYPE OF WORKS MODELS**


**Introduction:**

In recent years, data science roles are more demanded, so it's important to understand how they are evolving in terms of positioning as job offers and their salaries.

In this analysis, I will take my first Exploratory Data Analysis (EDA) and visualization project using Python and Tableau, where I explored data science jobs titles and salaries between 2020 and 2023. 

The "global salary index" dataset comes from the ai-jobs.net website for roles in the AI, ML, Data Science space based on internal data obtanided from surveys and jobs with open salaries.

This dataset is processed and updated on a weekly basis but I'll take the dataset updated on September 29th, 2023.

**Libraries used:**

Pandas

NumPy

Seaborn

Matplotlib

Pycountry

Pycountry-convert

Data: The "global salary index" dataset comes from the ai-jobs.net website for roles in the AI, ML, Data Science space based on internal data obtanided from surveys and jobs with open salaries and is processed and updated on a weekly basis, but, I'll take the dataset updated on September 29th, 2023.

**Hypotheses:**

What I want to find out with this analysis is to extract the following data from my data set:


- Top 3 highest-payed roles for each year and evaluate the changes between 2020-2023 

- Which level of experience has the most representation

- Evaluate the working model followed per year of work

- "Remote\_ratio VS company\_size": The size of the company influences in the overall amount of work done remotely? 

- "Remote\_ratios VS Salary": Which kind of "type of work" has the highest salaries on 2023? has this changed over the years?

- "Remote\_ratios VS location": Where are located the companies with most of the full\_remote workers? Is there any country that stands out in particular?


**Dataset details:**

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


**Data preprocessing:**

To start my analysis I was to get an overview of my data set. To do this, I exported the file and examined its contents: size, columns and rows distributions to see the information it contained, i.e. the distribution of roles(job\_titles) and salaries (in USD) according to company size, experience levels, employee and company location or proportion of remote work ratio.

To do this I used the functions pd.read, head(), shape(), info(), describe() and df.columns. Finally I explored if the dataset had missing values and the unique values for each column.

Once I got all the overall information I could start working with the data and think about what changes I could make to clean it up, transform it and ensure more meaningful consistency of certain values.

**Exploratory Data Analalysis (EDA):**

The dataset contains two types of variables, numericals and categoricals and and we proceeded to divide them to process the data.






**Data visualization:**

Once we have the new clean dataset we can start working with the Data visualization, the process of graphical representation of information and data, by using visual elements like charts, graphs, and maps, and data visualization tools like Python or Tableau that provide an accessible way to see and understand patternd, trends, and outliers in data.

**Results:**
