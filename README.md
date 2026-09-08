# Data Professional Survey Analysis: Power BI Workforce Dashboard
## Executive Summary

This project uses **Power BI** to analyze survey data from data professionals and uncover insights into salaries, job roles, programming language preferences, geographic representation, work-life balance, salary satisfaction, and the perceived difficulty of entering the data field.

The raw survey data contained several data-quality challenges, including inconsistent text responses, customized “Other” entries, and salary ranges stored as text. I used **Power Query** to clean and transform the dataset, convert salary ranges into numeric values, and prepare the data for analysis and visualization.

The completed dashboard highlights several key findings: **Data Scientists had the highest average salary among the surveyed job titles, Python was the most popular programming language, and respondents reported greater satisfaction with work-life balance than with salary.**

This project demonstrates an end-to-end Power BI workflow, from data preparation and transformation to interactive dashboard development and business-focused insight generation.

## Business Problem

Survey data can provide valuable insights into workforce and career trends, but raw survey responses are often difficult to analyze. Inconsistent text fields, salary ranges, and varying response formats can make it challenging to identify meaningful patterns.

For **students, career changers, recruiters, and business stakeholders**, understanding trends among data professionals can provide useful information about salary expectations, in-demand technical skills, job roles, and barriers to entering the data field.

This project addresses the following business questions:

* Which data-related job titles have the highest average salary?
* Which programming languages are most popular among data professionals?
* Which countries are most represented in the survey?
* How satisfied are respondents with their salary and work-life balance?
* How difficult do respondents perceive entering the data field to be?

## Tools & Technologies

* **Power BI**
* **Power Query**
* **DAX**

## Dataset

The project uses a publicly available survey dataset covering data professionals. The dataset includes information on:

* Job title
* Salary range
* Favorite programming language
* Country
* Work-life balance
* Salary satisfaction
* Perceived difficulty of entering the data field

The raw dataset is not included in the repository. Instead, the project focuses on demonstrating the **data cleaning, transformation, analysis, and visualization workflow in Power BI**.

## Methodology

### 1. Data Import

The survey dataset was imported into Power BI. Rather than loading the raw data directly into the model, I selected **Transform Data** to open Power Query and prepare the dataset before developing the dashboard.

### 2. Data Cleaning & Transformation

The dataset required several transformations to make it suitable for analysis. Using Power Query, I:

* Removed unnecessary columns.
* Standardized job title values, particularly responses categorized as “Other.”
* Cleaned programming language responses and removed unnecessary custom text.
* Split columns using delimiters to isolate relevant responses.
* Standardized country and industry fields to reduce inconsistencies.
* Duplicated the original salary column before transformation.
* Split salary ranges into separate numeric values.
* Removed characters such as `k`, `-`, and `+` from salary values.
* Converted open-ended salary responses into numeric estimates.
* Changed salary fields from text to whole-number data types.
* Created a custom column to calculate average salary from salary ranges.
* Updated data types to ensure compatibility with analysis and visualizations.

### 3. Dashboard Development

After preparing the dataset, I developed an interactive Power BI dashboard to communicate the survey findings.

The dashboard includes:

* **KPI cards** displaying the total number of survey respondents and average respondent age.
* **Bar chart** comparing average salary across job titles.
* **Column chart** showing favorite programming languages.
* **Treemap** displaying the geographic distribution of respondents.
* **Gauge charts** measuring satisfaction with work-life balance and salary.
* **Donut chart** showing respondents’ perceptions of the difficulty of entering the data field.

### 4. Dashboard Design

The dashboard was designed with a focus on readability, consistency, and user interaction.

Key design improvements included:

* Renaming chart titles and axis labels for greater clarity.
* Applying a consistent visual theme rather than relying on the default Power BI layout.
* Adjusting colors to improve category recognition.
* Organizing and resizing visuals to create a clean dashboard structure.
* Using the country treemap as an interactive filter, allowing users to explore results by location.

## Power BI Skills Demonstrated

This project demonstrates practical experience with:

* Data cleaning and transformation using Power Query
* Removing unnecessary columns
* Splitting columns by delimiter
* Replacing and standardizing values
* Data type conversion
* Creating custom columns
* Transforming text-based salary ranges into numeric values
* KPI dashboard development
* Creating bar, column, treemap, gauge, and donut charts
* Interactive filtering
* Dashboard formatting and layout design
* Business-focused data storytelling

## Dashboard Screenshot
<img width="1315" height="742" alt="Screenshot 2026-08-28 152417" src="https://github.com/user-attachments/assets/1ebd48a6-2173-4b5e-82d7-934b381755c9" />


## Key Findings & Practical Implications

The analysis produced several notable findings:

* The survey included **630 respondents**, with an average age of **29.87**.
* **Data Scientists** had the highest average salary among the surveyed job titles, indicating stronger earning potential within this particular sample.
* **Python** was the most popular programming language, highlighting its importance for individuals pursuing or developing careers in data-related roles.
* The **United States and India** represented major groups within the survey, which may influence the overall salary and career trends observed.
* Respondents reported greater satisfaction with **work-life balance than salary**, suggesting that compensation may be a more significant area of concern.
* Some respondents reported that **breaking into the data field was difficult**, highlighting potential barriers for people entering data-related careers.

## Limitations

The analysis is based solely on the available survey dataset, so the findings should not be considered representative of the entire global data professional population.

Several responses contained inconsistent or customized text, particularly within “Other” categories. Although these responses were cleaned using Power Query, some categories may remain broad or simplified.

Additionally, salaries were originally reported as ranges rather than exact values. The average salary metric was therefore calculated using estimated midpoint values. As a result, salary figures should be interpreted as **approximate comparisons rather than precise salary measurements**.

## Future Improvements

With additional time and data, I would extend the project by:

* Adding more detailed country-level salary and workforce analysis.
* Creating dedicated dashboard pages for salary, skills, and career satisfaction.
* Adding slicers for job title, country, industry, and experience level.
* Comparing salary satisfaction against estimated salary levels.
* Analyzing programming language preferences across different job titles.
* Developing more advanced DAX measures for deeper analysis.

## What I Learned

This project allowed me to practice the complete **Power BI analytics workflow**, from transforming raw survey data to building an interactive dashboard and communicating actionable insights.

I gained hands-on experience cleaning inconsistent survey responses, converting salary ranges into usable numeric measures, creating interactive visualizations, and structuring a dashboard around business questions.

Most importantly, the project helped me strengthen my ability to translate technical data-analysis work into **clear, business-focused insights**—an important skill for data analyst and business intelligence roles.
