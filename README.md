# Portofolio
<div align="justify">
Hi, there! My name is William Wibowo Ciptono, people usually call me William. I'm from Indonesia and currently still on the way to finishing my Industrial Engineering degree at Bandung Institute of Technology. In this repository, I'm going to show you some of the projects that I have been working on over the last few months. If you have any interest to collaborating with me or anything, feel free to drop a DM at my linkedin account which can be accessed on <a href="https://www.linkedin.com/in/williamwibowo/">this link</a>. Enjoy!</div>


# Summary
1. **[Hotel Booking Cancelation Prediction with Random Forest Model](https://github.com/lgamal/Hotel-Booking-Cancelation-Prediction-Model)**
2. **[Mas Trendy Discord Bot](https://github.com/lgamal/MasTrendy)**
3. [Titanic - **Machine Learning practice with CatBoost**](https://www.kaggle.com/lgamal/titanic-case)
4. [**Payment Matching** - ID NDSC 2020](https://www.kaggle.com/lgamal/payment-matching/)
5. [**Market Basket** - ID NDSC 2020](https://www.kaggle.com/lgamal/market-basket)

## Hotel Booking Cancelation Prediction Model with Random Forest Model
<div align="justify">
At the pandemic era that emerged in 2020, the hospitality industry has become one of the most affected industries. Based on McKinsey's prediction in one of theirs article that has been posted on June 10, 2020, it was stated that there was more than a 50% decrease in total revenue of the hospitality industry in America (Krishnan, 2020). They also predicted that there will be a 'rebound era' or 'recovery era' that will happen from 2023 to 2024, where all of the revenue will slowly improving to the previous pre-pandemic state. <br/><br/>
By able to predict the hotel booking cancelation, the hospitality industries will be able to manage their budget on marketing better and make the most profit from each order. On the other side, knowing which order will be canceled also helps the hospitality industries to improve their service quality by preventing any conflictual overbook. <br/><br/>
On this project, I have managed to choose the best models which gives a <b>83.56% f1 score accuracy</b> result. Those result are obtained by using <b>random forest</b> model and performing feature selection techniques over the feature engineered predictive variables and also hyperparameter tuning process as the cherry on top. The following is a diagram about the research outline. More info about this project can be accessed on <a href="https://github.com/lgamal/Hotel-Booking-Cancelation-Prediction-Model">this link</a>.
</div>
<div align="center">
<img src="https://github.com/lgamal/Hotel-Booking-Cancelation-Prediction-Model/blob/main/visualisasi%20metode%20penelitian.png" alt="the research outline">
</div>

## Mas Trendy Discord bot
**Mas Trendy** is an Open Source, `Google trend & Google search` powered `Discord Bot`. Equipped with **daily-push-notification** about the current trends based on Google search-engine and **manual-push-notification** to search current trends in each country. This project is written on Python language with help of several packages such as Discord.py, Pytrends, and so on. Feel free to check this project on [this link](https://github.com/lgamal/MasTrendy).

#### Here's some picture of Mas Trendy in action

![Image Mas Trendy 1](/mastrendy_screenshot_1.png)
![Image Mas Trendy 2](/mastrendy_screenshot_2.png)

## Titanic - Machine Learning Prediction/Classification with CatBoost Model
The sinking of the Titanic is one of the most infamous shipwrecks in history. On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew. While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.
In this mini case, which held on **Kaggle.com**, we got to answer **“what sorts of people were more likely to survive?”** using the available passenger data (in total **891** rows of train data & **418** test data set).

To answer that question, I've made a simple machine learning model using the boosting method with the help of `Catboost`(gradient boosting framework lib). To help improve the accuracy score, I also applied some `Data Preparation Technique`(Data cleaning, Filling Missing Value, etc.) and did some `Feature Engineering` such as ("Lowfare" label to identify people who board with less than $50 fare and "Age band" to classified people based on their ages). In this project, I have managed to acquired **78.229% accuracy score**. Feel free to check the notebook on [this link](https://www.kaggle.com/lgamal/titanic-case).

#### Here's some sneak peek of the project result

```Python
g = sns.FacetGrid(train, col="Survived", row="Sex")
g.map(plt.hist,"Fare")
```

![Image Titanic Visualization 1](/titanic/Visualization_1.png)

Feature | Feature Importance Score
--------| ------------------------
Sex|55.060701
SibSp|5.747522
Parch|6.197176
Age|8.180586
Lowfare|1.597320
Pclass_1|6.741240
Pclass_2|2.400222
Pclass_3|11.207736
Embarked_C|0.606663
Embarked_Q|0.592664
Embarked_S|1.668170


## Payment Matching - ID NDSC 2020
This is a Payment Matching case that was contested a few months ago at NDSC(National Data Science Competition) 2020. In this competition, I used `fuzzywuzzy` packages helps to gain the ***Levenshtein score*** from the `buyer name` & `transaction description`. Based on the Levenshtein score, I can finally have some clue about which customer do which transaction. In the end, I submitted a late submission and successfully got a **0.9944 Public Score** & **0.99433 Private Score**. Here's [the link](https://www.kaggle.com/lgamal/payment-matching/) to my Kaggle notebook.

## Market Basket - ID NDSC 2020
On the previous NDSC(National Data Science Competition) 2020 event, there's a market basket analysis case. I grouped `orderid` based on `customerid` to make the matching process more easier. In the end, I submited a late submission and successfully got a **1.0 Public Score** & **1.0 Private Score**. Here's [the link](https://www.kaggle.com/lgamal/market-basket) to my Kaggle notebook.
