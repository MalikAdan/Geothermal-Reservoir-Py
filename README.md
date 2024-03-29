# MalikAdan: Prediction of temperature using hydrogeochemical concentrations in geothermal reservoirs with machine learning algorithms

Author: Adan Malik, Petroleum Engineer, Pakistan Petroleum Limited. [Bio at the bottom]


## Purpose
In this notebook, we explore the application of machine learning techniques for predicting the temperatures of geothermal reservoirs, utilizing hydrogeochemical data. This study exclusively focuses on a regression-based approach, aiming to forecast the temperature of geothermal reservoirs as a continuous numerical value.

## Methodology
For the regression analysis, following machine learning models are used,  
1. Linear Regression 
2. Ridge Regression
3. Lasso Regression
4. ElasticNet Regression
5. Support Vector Machine (SVM)
6. K-Nearest Neighbors
7. Decision Tree
8. Random Forest Regressor

To enhance the accuracy and reliability of our predictions, the study incorporates data preprocessing methods. This involves normalizing the hydrogeochemical data and implementing outlier detection techniques, which are essential for refining the machine learning models' performance. Additionally, a feature importance analysis is conducted to identify the key hydrogeochemical parameters that most significantly influence geothermal reservoir temperatures. This aspect of the study is crucial for gaining deeper insights into the geothermal processes and for further improving the predictive capabilities of the models.


## Results
1. The observed dataset exhibits a weak correlation between predictor and response variables, leading to suboptimal performance of linear regression models. The high Mean Square Error (MSE) values indicate a significant deviation of the model predictions from the actual data.
2. A set of eight machine learning algorithms was used to analyze the hydrogeochemical dataset. During both training and testing phases, these models achieved moderate levels of accuracy. Notably, the Decision Tree and Random Forest Regression models demonstrated better performance, achieving MSEs of 0.8177 and 0.7881, respectively.
3. A correlation analysis revealed that SiO<sub>2</sub>, Na, and Cl concentrations exhibit a relatively strong positive correlation (exceeding 0.2) with geothermal reservoir temperatures, suggesting their potential as predictive indicators in the models.
4. Feature importance ranking analysis identified SiO<sub>2</sub> (measured in mg/L) as the most critical predictor in base cases of both Decision Tree and Random Forest models.
5. Based on their minimal impact on model performance, Boron (mg/L) and Potassium (K, measured in mg/L) were excluded from the dataset, streamlining the feature set for more efficient model training.
6. The predictive accuracy of the machine learning models is anticipated to improve with the integration of additional predictor variables and an expanded dataset, enhancing the models' ability to capture complex relationships within the data.
7. Hyperparameter tuning yielded significant improvements in model performance. Specifically, the Random Forest model exhibited a 3.5776% reduction in MSE and a 16.1744% increase in R<sup>2</sup> score. For the Decision Tree model, hyperparameter tuning resulted in a 41.6862% improvement in R<sup>2</sup> score and a 8.5836% decrease in MSE.
8. After hyperparameter tuning, the Decision Tree model outperformed the Random Forest model, as evidenced by a 5.271% higher R<sup>2</sup> score, indicating a more accurate fit to the data and superior predictive capability.

## Suggested next steps
In future, a robust cross-validation strategy could be employed to assess the models' generalizability across various datasets. This will ensure that the predictive models would be applicable and reliable in different geothermal contexts.


## References

    Haklidir, M. (2019) NIS-GRT, GitHub, https://github.com/haklidir/NIS-GRT/tree/master
    Pyrcz, M. (2021) PythonNumericalDemos, GeostatsGuy, GitHub, https://github.com/GeostatsGuy
    GeeksforGeeks (2021) How to Standardize Data in a Pandas DataFrame?, https://www.geeksforgeeks.org/how-to-standardize-data-in-a-pandas-dataframe/
    Shetye, A. (2019) Feature Selection with sklearn and Pandas, Medium, https://towardsdatascience.com/feature-selection-with-pandas-e3690ad8504b
    Leung, K. (2021) Random Forest Regressor Code for Condo Rental Prediction, GitHub, https://gist.github.com/kennethleungty/ea3cc1de4c424a63e318f1ba5dff7c6a
    NBShare Notebooks. Decision Tree Regression With Hyper Parameter Tuning, https://www.nbshare.io/notebook/312837011/Decision-Tree-Regression-With-Hyper-Parameter-Tuning-In-Python/

## About me

Hi! I'm Adan Malik, an enthusiastic and dynamic petroleum engineer, weaving data and energy to spark innovation. I'm not just drilling for oil - I'm mining insights.

My academic journey at NED University of Engineering and Technology was a cocktail of rigorous engineering and research zest, culminating in a standout CGPA of 3.88. I didn't just study Petroleum Engineering; I lived it, earning a distinction in my batch. My dissertation? A deep dive into the stress analysis of completion strings for high pressure high temperature (HPHT) gas wells.

Tech-savvy? Absolutely. Python, Prosper, MBAL, Petrel, and a parade of other advanced engineering tools are my playground. I'm also a fan of weaving data narratives through Python for Data Science and have a knack for making Excel and Power BI dance to my tunes.

As I navigate the complexities of energy and its future, my notebook here is more than code – it's a chronicle of my journey in reshaping how we understand and utilize energy resources. Welcome to my digital domain, where petroleum engineering meets programming!

I can be reached at adansajid.sajid26@gmail.com.

P.S. Explore my code, share your thoughts, and let's fuel the future of energy, one line of code at a time.


### Permission Requests

For permission requests, write to the author at adansajid.sajid26@gmail.com.
