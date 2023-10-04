

EDA and Visualizations project
DATA SCIENCE JOBS: SALARIES AND TYPE OF WORKS MODELS


Introduction:

In recent years, data science roles are more demanded, so it's important to understand how they are evolving in terms of positioning as job offers and their salaries.

In this analysis, I will take my first Exploratory Data Analysis (EDA) and visualization project using Python, where I explored data science salaries between 2020 and 2023. 

The "global salary index" dataset comes from the ai-jobs.net website for roles in the AI, ML, Data Science space based on internal data obtanided from surveys and jobs with open salaries.

This dataset is processed and updated on a weekly basis but I'll take the dataset updated on September 29th, 2023.

Libraries used:

Pandas
NumPy
Seaborn
Matplotlib
Pycountry
Pycountry-convert

Data: The "global salary index" dataset comes from the ai-jobs.net website for roles in the AI, ML, Data Science space based on internal data obtanided from surveys and jobs with open salaries and is processed and updated on a weekly basis, but, I'll take the dataset updated on September 29th, 2023.

Hypotheses:

- Top 3 highest-payed roles, and evaluate the changes between 2020-2023 
(groupby role, agg salary, )

- Which level of experience has the most representation?

- "Remote_ratios":
Evaluate the working model followed per year of work

		- "Remote_ratio VS company_size": The size of the company influences in the overall amount of work done remotely? - compare company sizes and % of roles in each "remote_ratio"

		- "Remote_ratios VS Salary": which kind of "type of work" has the highest salaries on 2023? has this changed over the years?
		(median per cada remote_ratio---box plot)

		- "Remote_ratios VS countries and residence": Where are most of the full_remote workers? Is there any country that stands out in particular?


Dataset details:

















Data preprocessing:

First steps:
To start my analysis I was to get an overview of my data set. To do this, I exported the file and examined its contents: size, columns and rows distributions to see the information it contained, i.e. the distribution of roles(job_titles) and salaries (in USD) according to company size, experience levels, employee and company location or proportion of remote work ratio.

To do this I used the functions pd.read, head(), shape(), info(), describe() and df.columns. Finally I explored if the dataset had missing values and the unique values for each column.

Once I got all the overall information I could start working with the data and think about what changes I could make to clean it up, transform it and ensure more meaningful consistency of certain values.

Exploratory Data Analalysis (EDA):
The dataset contains two types of variables, numericals and categoricals and and we proceeded to divide them to process the data.






Data visualization:
Once we have the new clean dataset we can start working with the Data visualization, the process of graphical representation of information and data, by using visual elements like charts, graphs, and maps, and data visualization tools like Python or Tableau that provide an accessible way to see and understand patternd, trends, and outliers in data.





__________________________

Results:



Conclusions: