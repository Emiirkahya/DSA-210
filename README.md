# DSA-210

Project Title: Sleep Quality Prediction and External Factor Correlation Analysis


1.
Motivation and Project Goal 
The primary motivation for this project is to use scientific methodologies to investigate the effect of technology and environmental factors on individual sleep quality, using personal data. Since sleep hygiene is a critical indicator for health and productivity, it is important to understand which external factors positively or negatively influence sleep quality.


The core objectives of the project are:

To create a personal sleep data set and enrich it with an external, secondary data set.

To use exploratory data analysis (EDA) and visualizations to reveal the relationships between sleep and external factors.

To identify key variables affecting sleep quality and implement appropriate machine learning (ML) techniques to build a sleep quality prediction model.


2.
Primary Data Set (Own Data)  Personal Sleep Data (Sleep Duration, Deep/Light Sleep Ratios, Number of Awakenings)   [DATA COLLECTION TOOL/APP - E.g.: Smartwatch (Garmin/Apple Watch) or Sleep Tracking App data]

Enrichment Data Set (Public Data)   [EXTERNAL DATA SET NAME - E.g.: Local Weather Records / Caffeine Intake / Daily Step Count]   [SOURCE - E.g.: Public Weather API (OpenWeatherMap) / Self-Reported Daily Logs / Smartwatch Fitness Data]



3.
Data Collection and Enrichment Plan 
The project will perform a multivariate analysis by combining the Primary Data Set with the Enrichment Data Set.

Data Collection: Primary sleep data will be collected regularly [STARTING FROM DATE]. The enrichment data (e.g., weather data) will be acquired for the same dates, either via API or manually.

Enrichment (Correlation): The two data sets will be merged based on the common day/date variable. This will allow us to examine the effects of [EXTERNAL VARIABLE] (e.g., nighttime temperature) on sleep quality metrics.


Goal: The enriched data set will enable the creation of a more robust sleep quality prediction model that accounts for external environmental or behavioral factors, not just sleep habits.


4.
Methodology and Analysis Plan 
The project will follow the full data science pipeline through the following milestones:


Data Preparation and EDA (Due November 28): 

Identification and handling of missing values and outliers in the combined data set.

Application of Exploratory Data Analysis (EDA) to visualize the distribution of sleep metrics and their basic correlations with external variables.

Execution of hypothesis tests on relevant variables (E.g., "Higher nighttime temperature is correlated with shorter Deep Sleep duration.").


Machine Learning Implementation (Due January 02): 

A Target Variable (e.g., Sleep Quality Score or similar metric) will be defined.


Model: An appropriate [TYPE OF ML MODEL - E.g.: Regression (Linear/Random Forest) or Classification (Logistic/SVM)] model will be implemented to predict or classify sleep quality.


Findings and Presentation: The model's performance will be evaluated, and insights regarding the factors most influencing sleep quality will be presented.



5.
Deliverables 

GitHub Repository: The repository must contain all code, documentation, and a requirements.txt file for dependencies.


Report/Presentation: Project findings will be communicated through one of the preferred formats (classic article-type report, video, or webpage).



Code Requirement: All code must be written in Python, be well-documented, and include a README.md with instructions to reproduce the analysis.
