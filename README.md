DSA 210 – Sleep Quality Analysis Using Weather Data
1. Introduction and Objective

Sleep quality is a crucial component of overall physical and mental well-being. Environmental factors, particularly weather conditions such as temperature and humidity, may influence sleep duration and quality. The aim of this project is to analyze the relationship between sleep characteristics and weather conditions using personal sleep data combined with external weather data. Additionally, machine learning methods are applied to predict sleep quality based on environmental variables.

2. Data Description

2.1 Sleep Data
The sleep dataset was calculated manually by the participant using daily sleep summaries. Each observation represents one night of sleep.

The dataset includes the following variables:
- date: Date of the sleep record
- total_sleep_hours: Total duration of sleep in hours
- deep_sleep_hours: Duration of deep sleep
- light_sleep_hours: Duration of light sleep
- num_awakenings: Number of awakenings during the night
- sleep_score: Overall sleep quality score

2.2 Weather Data
Weather data was obtained from Apple Weather for the Pendik region. Daily weather summaries were used to align with the sleep data.

The dataset includes the following variables:
- date: Date of the weather record
- min_temp: Minimum daily temperature
- max_temp: Maximum daily temperature
- avg_temp: Average daily temperature
- humidity: Average daily humidity
- weather_condition: Categorical weather description (e.g., Sunny, Cloudy, Rain)
The sleep and weather datasets were merged using the date variable, resulting in a unified dataset for analysis.

3. Feature Engineering
To support machine learning tasks, additional features were derived from the raw data. A binary classification target variable, good_sleep, was defined as follows:

good_sleep = 1 if total_sleep_hours ≥ 7 and sleep_score ≥ 85
good_sleep = 0 otherwise

This definition incorporates both sleep duration and quality. Additional engineered features include temperature range (max_temp − min_temp), a binary rain indicator derived from weather_condition, and day-of-week information.

4. Exploratory Data Analysis
Exploratory Data Analysis (EDA) was conducted to understand the structure and characteristics of the data. Distributions of sleep metrics were examined using histograms, while temporal patterns were explored through time-series visualizations. Scatter plots and boxplots were used to analyze relationships between weather variables and sleep outcomes. A correlation heatmap was also generated to identify linear associations between numerical variables.

5. Statistical Hypothesis Testing
Several statistical hypothesis tests were conducted to evaluate relationships observed during EDA:

- Mann–Whitney U test was used to compare temperature distributions between good and poor sleep nights.
- Chi-square test was applied to assess the association between rainfall and sleep quality.
- Spearman correlation analysis was used to examine the relationship between humidity and sleep score.

These tests provide statistical evidence supporting or rejecting the proposed hypotheses.

6. Machine Learning Methodology

6.1 Classification
The primary machine learning task was binary classification, where the objective was to predict whether a night resulted in good or poor sleep. Logistic Regression was used as a baseline model, while Random Forest was employed as a more complex non-linear model.

Model performance was evaluated using Accuracy, F1-score, and ROC-AUC metrics. Confusion matrices and ROC curves were generated to visualize classification performance.

6.2 Regression (Additional Analysis)
As an additional analysis, regression models were used to predict continuous sleep outcomes, specifically sleep_score and total_sleep_hours. Linear Regression served as a baseline model, and Random Forest Regressor was used to capture potential non-linear relationships.

Model performance was assessed using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² metrics. Residual and true-versus-predicted plots were examined to evaluate model fit.

7. Results and Discussion
The results indicate that weather variables exhibit measurable associations with sleep quality. Random Forest models consistently outperform linear baselines in both classification and regression tasks, suggesting the presence of non-linear relationships between weather conditions and sleep outcomes. Feature importance analysis highlights temperature-related variables as influential predictors.

8. Reproducibility
All dependencies required to reproduce the analysis are listed in the requirements.txt file. The complete workflow, including EDA, hypothesis testing, and machine learning experiments, can be reproduced by running the provided Jupyter notebook.

9. AI Usage Disclosure
AI-based tools were used for methodological guidance, code structuring, and visualization suggestions. All analysis steps, modeling decisions, and interpretations were reviewed and implemented by the student.

10. Course Information
DSA 210 – Fall 2025
