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



SLEEP DATA

date	total_sleep_hours	deep_sleep_hours	light_sleep_hours	num_awakenings	sleep_score
2025-11-01	7.6	1.5	6.1	2	88
2025-11-02	6.9	1.2	5.7	3	82
2025-11-03	8.1	1.8	6.3	1	91
2025-11-04	7.4	1.4	6.0	2	86
2025-11-05	6.2	1.0	5.2	3	78
2025-11-06	7.9	1.7	6.2	2	90
2025-11-07	8.3	2.0	6.3	1	94
2025-11-08	7.1	1.3	5.8	2	84
2025-11-09	6.5	1.1	5.4	3	80
2025-11-10	7.8	1.6	6.2	2	89
2025-11-11	6.8	1.2	5.6	3	81
2025-11-12	7.2	1.3	5.9	2	85
2025-11-13	8.0	1.9	6.1	1	92
2025-11-14	6.4	1.1	5.3	3	79
2025-11-15	7.7	1.6	6.1	2	88
2025-11-16	8.4	2.1	6.3	1	95
2025-11-17	6.6	1.0	5.6	3	80
2025-11-18	7.3	1.4	5.9	2	87
2025-11-19	8.2	1.9	6.3	1	93
2025-11-20	6.7	1.1	5.6	3	81
2025-11-21	7.5	1.5	6.0	2	88
2025-11-22	5.9	0.9	5.0	4	72
2025-11-23	6.1	1.0	5.1	3	75
2025-11-24	7.4	1.3	6.1	2	86
2025-11-25	8.6	2.0	6.6	1	95
2025-11-26	6.3	1.1	5.2	3	78
2025-11-27	7.2	1.4	5.8	2	85
2025-11-28	8.1	1.8	6.3	1	92
2025-11-29	7.0	1.2	5.8	2	83
2025-11-30	6.8	1.1	5.7	3	80<img width="504" height="654" alt="image" src="https://github.com/user-attachments/assets/1a999e6d-a348-4eed-b035-ada57b6110e8" />



EXTERNAL DATA PENDIK

date	min_temp	max_temp	avg_temp	humidity	weather_condition
2025-11-01	13	21	17.0	72	Sunny
2025-11-02	12	20	16.0	70	Partly Cloudy
2025-11-03	11	19	15.0	68	Cloudy
2025-11-04	10	18	14.0	75	Rain
2025-11-05	10	17	13.5	78	Rain
2025-11-06	9	17	13.0	80	Cloudy
2025-11-07	9	18	13.5	82	Sunny
2025-11-08	8	17	12.5	85	Rain
2025-11-09	8	16	12.0	83	Rain
2025-11-10	9	17	13.0	79	Cloudy
2025-11-11	10	18	14.0	77	Partly Cloudy
2025-11-12	11	19	15.0	76	Sunny
2025-11-13	12	20	16.0	74	Sunny
2025-11-14	11	19	15.0	73	Cloudy
2025-11-15	10	18	14.0	72	Partly Cloudy
2025-11-16	9	17	13.0	75	Rain
2025-11-17	8	16	12.0	78	Rain
2025-11-18	8	15	11.5	80	Cloudy
2025-11-19	7	14	10.5	82	Rain
2025-11-20	7	14	10.5	84	Rain
2025-11-21	6	13	9.5	86	Cloudy
2025-11-22	7	14	10.5	83	Rain
2025-11-23	8	15	11.5	81	Partly Cloudy
2025-11-24	9	16	12.5	79	Sunny
2025-11-25	10	17	13.5	77	Sunny
2025-11-26	9	16	12.5	78	Cloudy
2025-11-27	8	15	11.5	80	Rain
2025-11-28	8	15	11.5	82	Rain
2025-11-29	9	16	12.5	81	Partly Cloudy
2025-11-30	10	17	13.5	79	Sunny<img width="382" height="654" alt="image" src="https://github.com/user-attachments/assets/fa7bb110-7252-4dce-aa9e-fa5775efd890" />




