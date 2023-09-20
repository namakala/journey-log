---
output: pdf_documents
---

# 2023-09-19

- Do monthly meeting with Prof. Talitha and Assoc. Prof. Frederika Jorg on Tuesday/Thursday
- Bimonthly meeting should involve Prof. Mako
- Umbrella review:
  - Create a flow diagram of data management
  - Describe what kind of study is being discarded
  - Merge Korea with South Korea when cleaning the dataset
  - Merge Arab Saudi with Saudi Arabia
  - Merge Maryland with USA
  - In EDA, arrange the self-report instrument together
  - Subgroup analysis for the `incl_year`
  - Search for metaregression for prevalence
  - Share the paper about prediction interval (from meta) and I2 to Prof. Talitha

# 2023-09-07

- Course to take: https://cursus1.webhosting.rug.nl/gsms/course-information/?tx_seminars_pi1%5BshowUid%5D=1675
- IADB data:
  - Need to perform descriptive statistics
  - Tinker the SQL code from IADB toolbox for 
- Research proposal:
  - Align the research questions with IADB data request protocol:
    - 1: Add the phrase: "In relation with drug's use"
    - 2: Check the data request protocol
    - 3: How does an individual perceive their health in relation with environmental stressors, such as the COVID-19 pandemic?
  - In scoping review: Include the role of medicine to resilience
  - Find a co-author with primary domain in neuropsychiatry or neurpsychology $\to$ Contact dr. Khamelia
  - Simplify the idea about the model

# 2023-07-20

- Contact Prof. Mako regarding monthly or bi-monthly regular meeting $\to$ Output: Brief MoM
- Protocol draft:
  - Table of population estimate: Check the box to include this data
  - Title: Add in adults
  - Overview of literature: Add other study on the effect of pandemic on the use of psychopharmaca $\to$ Tell how many studies have been done, and how they were investigated
  - In methods: Add comparison during the pandemic because different policy might have different impact $\to$ Add to the exploratory question
  - Clarify the research question, create a footnote to explain what a daily epoch is
  - Specify what the pattern implies in the secondary question
  - Specify "the past five years" as 2018-2022
  - Exclude patients whose prescribed duration is less than two weeks
  - Prescription table: Add variable request for the prescriber
  - Rewrite he effect measures $\to$ Clarify the point in a layman term
  - In statistical methods:
    - First paragraph should be the summary of how I plan my analysis
    - Explain how to analyze the differences before and during COVID-19
    - Link each method with the research questions
    - Add references to the graph knowledge embedding
    - Clarify the aggregation on weekly, monthly, and quarterly basis (first paragraph in methods)
    - Specify what $N$ means $\to$ It is the total number of people making medication claim on daily basis
    - In the fourth paragraph
    - Explain how to handle patients with multiple drugs (use examples, as explained in the email)
    - Use subheadings to clarify which paragraph belongs to which ideas:
      - Executive summary (in bullet point)
      - Data management and feature engineering
      - Concurrent medication use as a matrix
      - Data analysis plan
    - Show the formula for eigenvector centrality $\to$ Refers to the R package being used and its function
    - Explain that the node is the medication
    - Last paragraph: Refer subgroup to the "Stratification of data" section
  - Stratification on age:
    - WHO/ILO: 18-25, 25-35, 35-45, 45-55, >56
    - Theory: 18-25, 25-45, 45-55, >56
  - Report: Interim analysis should be discussed and reported to IADB as well
- Discuss with Nynke Bosman regarding the medication and policy in the Netherlands
- Ask Fang about Dutch's guideline on MDD and anxiety disorder $\to$ Use this as a baseline to select the medication
- There's a table describing zip code into socioeconomic status
- Ask Frederick about courses for time-series analysis

# 2023-07-13

- Complete the data request form by next week
- Draft a SQL query for data request
- Proposal revision:
  - Choice of graph metrics $\to$ Include this as a literature review $\to$ Mention in subsection 4.2
  - Last paragraph in 4.2 is redundant, make it more compact
  - Add about the time-series analysis
  - Clarify the overall purpose: Is it to evaluate seasonality (pattern) or trend?
  - Add about the age range: 18-65
  - In the introduction of 4.2, explain why concurrent drug use is important to evaluate
  - Guideline to use when selecting the medication
- Master's course of time-series analysis in Autumn $\to$ In mathematics and economics department:
  - Mathematics: Fitting dynamical model to data
  - Economics: (Needs further searching)

# 2023-07-06:

- Complete the SQL course from IADB, then submit it right away
- Read the book: Going beyond cost-effectiveness by Kaying Kan
- Consider doing:
  - Interrupted time-series analysis
  - Moving average
- List all medications needed  $\to$ Will discuss it later
