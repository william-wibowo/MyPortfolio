Hi! My name is William Wibowo Ciptono, people usually call me William. In this repository, I will show you some projects that I have done over the last few months.  
Please enjoy!


# Summary
1. **[Mas Trendy Discord Bot](https://github.com/lgamal/MasTrendy)**
2. [Titanic - **Machine Learning practice with CatBoost**](https://www.kaggle.com/lgamal/titanic-case)
3. [**Payment Matching** - ID NDSC 2020](https://www.kaggle.com/lgamal/payment-matching/)
4. [**Market Basket** - ID NDSC 2020](https://www.kaggle.com/lgamal/market-basket)


## Mas Trendy Discord bot
**Mas Trendy** is an Open Source, `Google trend & Google search` powered `Discord Bot`. Equipped with **daily-push-notification** about the current trends based on Google search-engine and **manual-push-notification** to search current trends in each country. This project is written on Python language with help of several packages such as Discord.py, Pytrends, and so on. Feel free to check this project on [this link](https://github.com/lgamal/MasTrendy).

#### Here's some picture of Mas Trendy in action

![Image Mas Trendy 1](/mastrendy_screenshot_1.png)
![Image Mas Trendy 2](/mastrendy_screenshot_2.png)

## Titanic - Machine Learning practice with CatBoost
The sinking of the Titanic is one of the most infamous shipwrecks in history. On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew. While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.
In this mini case, which held on **Kaggle.com**, we got to answer **“what sorts of people were more likely to survive?”** using the available passenger data (in total **891** rows of train data & **418** test data set).

To answer that question, I've made a simple machine learning model using the boosting method with the help of `Catboost`(gradient boosting framework lib). To help improve the accuracy score, I also applied some `Data Preparation Technique`(Data cleaning, Filling Missing Value, etc.) and did some `Feature Engineering`. In this project, I have managed to acquired **77.9% accuracy score**. Feel free to check the notebook on [this link](https://www.kaggle.com/lgamal/titanic-case).

#### Here's some sneak peek of the project result

```Python
g = sns.FacetGrid(train, col="Survived", row="Sex")
g.map(plt.hist,"Fare")
```

![Image Titanic Visualization 1](/titanic/Visualization_1.png)

Feature | Feature Importance Score
--------| ------------------------
Pclass|18.179660
Sex|61.078684
SibSp|4.288450
Parch|1.915523
Age|5.854512
Embarked|5.109940
Lowfare|3.573231


## Payment Matching - ID NDSC 2020
This is a Payment Matching case that was contested a few months ago at NDSC(National Data Science Competition) 2020. In this competition, I used `fuzzywuzzy` packages helps to gain the ***Levenshtein score*** from the `buyer name` & `transaction description`. Based on the Levenshtein score, I can finally have some clue about which customer do which transaction. In the end, I submitted a late submission and successfully got a **0.9944 Public Score** & **0.99433 Private Score**. Here's [the link](https://www.kaggle.com/lgamal/payment-matching/) to my Kaggle notebook.

## Market Basket - ID NDSC 2020
On the previous NDSC(National Data Science Competition) 2020 event, there's a market basket analysis case. I grouped `orderid` based on `customerid` to make the matching process more easier. In the end, I submited a late submission and successfully got a **1.0 Public Score** & **1.0 Private Score**. Here's [the link](https://www.kaggle.com/lgamal/market-basket) to my Kaggle notebook.
