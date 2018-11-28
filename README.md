# SIBUR Data Science Competition (2018-11)




## Description
**SIBUR** is one of the top players on petrochemical and chemical market in Russia and CIS.

Roughly 140 commands have participated in online stage.

[Competition](https://sibur.ai-community.com/competitions/1/uploads/1) is about predicting 5 different values.
![](https://sibur.ai-community.com/files/uploads/2ef76efd4806be7bd2542fece5179271.png)

**Task** is to predict time-series (coking level of catalyst).

## Pipeline
1) Preprocessing (```ffill```, ```mean```, removing outliers)
2) Feature generation (```shift``` ,```rolling```, ```std```, ```ewm```, ```products``` and etc.)
3) Creation of diversified data models
4) Cross-validation: ```TimeSeriesSplit(3)```
5) Base models: ```sklearn.ensemble.GradientBoostingRegressor```
6) Hyperparameter optimization: ```GridSearchCV```
7) Blending

**Public score**: 0.4421

**Private score**: 0.4198 (top 13)


