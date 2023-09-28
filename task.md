---
output: pdf_documents
---

# TBD

Some questions regarding the pooling of the proportions. We can discuss tomorrow.

* Do we really want to pool over all studies? That is, do we think we can find a single estimate of the prevalence of MDD in T2DM that would be relevant worldwide and irrespective of outcome or time.

* Maybe here the proportion as a measure of prevalence differs from an effect measure, where you may reasonably assume it to be independent of setting in principle.

* Maybe when we combine all the 634 studies, this gives us the global average, which of course reflects a lot of heterogeneity (as we may expres by presenting a histogram). We should then ensure not to take more than one proportion from each study. (so it will be less than 634).
* Maybe that is more relevant than taking only the studies that are closest together (to avoid heterogeneity). Since we do expect and understand heterogeneity.


Next, for the subgroups. There we focus at one characteristic at a time.
Do we indeed expect that once we concentrate on country, we can expect to pool? I would be inclined to think so, but as you show, also time, outcome measure and maybe more do matter.
So question: Once you stratify by country: can we combine studies into a setting specific average? Is homogeneity sufficient? If not, does it make sense to select studies based on being no outlier? Or would it be more appropriate to further stratify for factors that will explain heterogeneity, like time of study and outcome measure?

Regarding time of study: I would prefer to use time of measurement when available. Time of individual study then is a proxy. Time of review is a very crude (maybe too crude) proxy.

About the pooling. Another factor that could explain heterogeneity is underlying prevalence of MDD and of T2DM.
Next to outcome measure, that may also be a matter of risk profile of the population (e.g. obesitas).
So could you and Nora also find the expected prevalence (by country/by time), based on published prevalence estimates of MDD and of T2DM (using GBD, WHO, OECD or IHME published numbers, whatever is most clear and consistent); calculate the expected proportion of MDD in T2DM based on such prevalences and then start doing the meta-regression on the remainder (So the additional prevalence of MDD over what you may expect) or maybe on the RR (the crude proportion divided by the expected proportion) or Odds Ratio.

Possibly this latter measure is one that you may expect to be the same irrespective of time or setting more reasonably, since it is more of an effect measure (the effect of T2DM on MDD risk). So then it becomes more reasonable to use established methods of meta-regression packages, which were initially developed for pooling effect measures.

What do you think?

For the analysis of the observed proportions, I think it is mostly the heterogeneity that you need to show in the results: SO how this varies indeed by country (a map would be great), by outcome measure etc.

If you take more than one outcome per study, how could you take account of the dependence these will have? Multilevel analysis an option? Or using clustered standard errors??

# 2023-09-23

- Umbrella review:
  - Might need to redo the analysis
  - To discuss with Katja and Nora:
    - Pros and cons of the current approach
    - Discuss about multiple entries
  - Discuss with Xinyu regarding meta-regression done by the mathematician in RUG:
    - Comparison of methods and packages to conduct metaregression
    - How to handle logit transformation
- IADB data:
  - Recheck the use of persistence toolbox $\to$ Combine parts of the code to my query
  - Change the overlap query into weekly basis
  - Check what we know about concurrent medication uses before and during the pandemic
- Scoping review:
  - Use multiple search to address:
    - Stressors, self perception, and resilience
    - Medication/policy and resilience
    - Resilience and psychological outcomes
  - Check PRISMA guideline on selecting articles for a scoping review
  - Perform bibliometrics analysis to narrow down the search
  - Need to create a clear selection criteria
  - Have a discussion with Frederike Jorg/librarian about the search strategy
  - Check on published articles using scoping review to investigate psychological disorders:
    - https://doi.org/10.1017/S0033291721004177
    - https://doi.org/10.1016/j.pnpbp.2020.110111

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
