# Life_expectancy
Prepared and cleaned a large life expectancy dataset (3k+ records), mastering the end-to-end EDA process from data preprocessing to visualization.
One of the most element in end of life judgement is Life expectancy. This research explores the computation of
machine learning regression techniques to predict life expectancy using a dataset of 15 years collected from Kaggle,
comprising demographic, health, and socioeconomic features. The dataset contain information from 193 countries with
multiple variables such as 'Country', 'Year', 'Status' (Developer/Developing), and many numerical indicators (e.g., Adult
Mortality, GDP, and Schooling). Twice Exploratory Data Analysis (EDA) was performed to gain proper insights into
feature distributions, identify outliers, and assess correlations. Missing values were treated using both mean imputation
and kNN imputation([6]), and categorical variables were encoded by label encoding. A rapid model benchmarking
approach is applied using the LazyPredict library was employed to compare multiple regression models, from where
many models were selected for Hyperparamertertunning to enhance their performance. The Regression model which
achieve outstanding performance after doing Hyperparameter Tunning on the test set is XGBRegressor model([4], [5])
also the R2 score of model is 96.87% with minimal RMSE. These results highlight the potential and challenges of
predictive modeling in life expectancy estimation, and underscore the importance of thorough preprocessing and model
validation.
