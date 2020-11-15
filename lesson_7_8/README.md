# Homework #7_8 :atom:

Homework for the class **'Training without a teacher'**

Python libraries for Data Science

# List of the tasks

## Task #1

#### Ru

Импортируйте библиотеки ```pandas``` и ```numpy```.

Загрузите "Boston House Prices dataset" из встроенных наборов данных библиотеки ```sklearn```. Создайте датафреймы ```X``` и ```y``` из этих данных.

Разбейте эти датафреймы на тренировочные (```X_train```, ```y_train```) и тестовые (```X_test```, ```y_test```) с помощью функции ```train_test_split``` так, чтобы размер тестовой выборки составлял 30% от всех данных, при этом аргумент ```random_state``` должен быть равен 42.

Создайте модель линейной регрессии под названием ```lr``` с помощью класса ```LinearRegression``` из модуля ```sklearn.linear_model```.

Обучите модель на тренировочных данных (используйте все признаки) и сделайте предсказание на тестовых.

Вычислите R2 полученных предказаний с помощью ```r2_score``` из модуля ```sklearn.metrics```.

#### En

Import ```pandas``` and ```numpy``` libraries.

Download the "Boston House Prices dataset" from the built-in data sets of ```sklearn``` library. Create ```X``` and ```y``` dataframes from these data.

Break down these dataframes into training (```X_train```, ```y_train```) and test (```X_test```, ```y_test```) dataframes using the ```train_test_split``` function so that the test sample size is 30% of all data and the ```random_state``` argument should be 42.

Create a linear regression model called ```lr``` using the ```LinearRegression``` class from the ```sklearn.linear_model module```.

Teach the model on training data (use all features) and make a prediction on test data.

Calculate R2 of the predictions received with ```r2_score``` from the module ```sklearn.metrics```.

## Task #2

#### Ru

Создайте модель под названием ```model``` с помощью ```RandomForestRegressor``` из модуля ```sklearn.ensemble```.

Сделайте агрумент ```n_estimators``` равным 1000, ```max_depth``` должен быть равен 12 и ```random_state``` сделайте равным 42.

Обучите модель на тренировочных данных аналогично тому, как вы обучали модель ```LinearRegression```, но при этом в метод ```fit``` вместо датафрейма ```y_train``` поставьте ```y_train.values[:, 0]```, чтобы получить из датафрейма одномерный массив ```Numpy```, так как для класса ```RandomForestRegressor``` в данном методе для аргумента ```y``` предпочтительно применение массивов вместо датафрейма.

Сделайте предсказание на тестовых данных и посчитайте R2. Сравните с результатом из предыдущего задания.

Напишите в комментариях к коду, какая модель в данном случае работает лучше.

#### En

Create a model called ```model``` with ```RandomForestRegressor``` from the ```sklearn.ensemble``` module.

Make the agent ```n_estimators``` equal to 1000, ```max_depth``` should be equal to 12 and ```random_state should``` be equal to 42.

Teach the model on training data in the same way as you taught the ```LinearRegression``` model, but in the fit method set ```y_train.values[:, 0]``` to get a one-dimensional array ```Numpy``` from the dataframe, because for the ```RandomForestRegressor``` class in this method, arrays are preferred instead of dataframes for the ```y``` argument.

Make a prediction on test data and calculate R2. Compare it with the result from the previous job.

Write in the comments to the code which model works best in this case.

## Task #3 (Optional)

#### Ru

Вызовите документацию для класса ```RandomForestRegressor```, найдите информацию об атрибуте ```feature_importances_```.

С помощью этого атрибута найдите сумму всех показателей важности, установите, какие два признака показывают наибольшую важность.

#### En

Call up documentation for the ```RandomForestRegressor``` class, find information about the attribute ```feature_importances_```.

Use this attribute to find the sum of all importance indicators, set which two indicators show the highest importance.

# Contributing

Pull requests are welcome.

# Source

[Geekbrains](https://geekbrains.ru)
