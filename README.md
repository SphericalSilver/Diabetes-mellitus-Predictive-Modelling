# Diabetes mellitus Risk Prediction
Profiles of healthy people and diabetic people were analyzed and used to build a predictive model to gauge the diabetes risk index of an untested person.

The [dataset](https://www.kaggle.com/johndasilva/diabetes/downloads/diabetes.zip/1) we worked with was acquired from a hospital in Frankfurt, Germany. It contains a profile of health indicators such as BMI, Age, and Blood Glucose levels of individuals with and without Diabetes.

## How to Run
Download the file and run on Jupyter Notebook.

At the bottom of the file, you'll be required to enter your health indicators, such as your BMI, Blood Glucose levels, Age, etc. The predictive model will return a Diabetes Risk Index and give a short health recommendation based on that.

## Project Goal

The prevalence of Diabetes in Singapore (10.5%) is not only higher than the world average (8.8%), but is also [ever increasing](https://www.healthhub.sg/a-z/diseases-and-conditions/626/diabetes). 

According to the World Health Organization (WHO), apart from prevention, [early diagnosis is one of the most effective ways](https://www.who.int/en/news-room/fact-sheets/detail/diabetes) to minimize the burden caused by diabetes. Our objective here was therefore to train a predictive model using the available data to learn what the profile of a person afflicted with Diabetes looks like. This model would then receive the profile of an untested individual, and based on that person's health indicators, measure the similarity of their profile against that of a person with diabetes, and assign that person a value that represents their predicted risk of having Diabetes.

By better educating individuals on their diabetes risk factor, the disease can be diagnosed and tackled earlier. The predictive model serves as a means to impart (possibly life-saving) health literacy to its users.

## Future Improvements

Some future improvements to improve our model's effectiveness could be:
- Use an error metric other than accuracy score, like f1 score or precision.
- Use domain knowledge (acquired from a Doctor or another more qualified person) to make better choices about feature engineering/selection. The weightage of each health indicator could also be tuned better using domain knowledge.
- Doing the prediction with algorithms like Neural Networks instead of Logistic Regression. 
- Using a larger data-set - ideally one from Singapore.
- Think of a different way to convert predicted Diabetes Probability into Risk Index.
- Deploy the model online as a Web App, possibly using Flask, or RStudios/Shiny. 
- Right now, blood glucose levels might not be properly standardized. We don't know if they represent the average blood glucose level over a week, or whether it was taken at a single point randomly in the day. In the latter case, it would be greatly susceptible to the time of the day it was taken, so factors like whether the person just had a meal might change it substantially. 

### Images

![Prediction Example](https://i.gyazo.com/40c209e5563e2450e0c4150269405c9f.png)
