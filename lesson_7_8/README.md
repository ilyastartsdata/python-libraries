# Homework #7_8 :atom:

Homework for the class **'Training with a teacher'**

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

## Task #4 (Optional)

#### Ru

В этом задании мы будем работать с датасетом, с которым мы уже знакомы по домашнему заданию по библиотеке ```Matplotlib```, это датасет Credit Card Fraud Detection.

Для этого датасета мы будем решать задачу классификации - будем определять,какие из транзакциции по кредитной карте являются мошенническими. Данный датасет сильно несбалансирован (так как случаи мошенничества относительно редки),так что применение метрики ```accuracy``` не принесет пользы и не поможет выбрать лучшую модель.

Мы будем вычислять ```AUC```, то есть площадь под кривой ROC.

- Импортируйте из соответствующих модулей ```RandomForestClassifier```, ```GridSearchCV``` и ```train_test_split```.
- Загрузите датасет creditcard.csv и создайте датафрейм ```df```.
- С помощью метода ```value_counts``` с аргументом ```normalize = True``` убедитесь в том, что выборка несбалансирована. Используя метод ```info```, проверьте, все ли столбцы содержат числовые данные и нет ли в них пропусков. Примените следующую настройку, чтобы можно было просматривать все столбцы датафрейма (```pd.options.display.max_columns = 100```).
- Просмотрите первые 10 строк датафрейма ```df```.
- Создайте датафрейм ```X``` из датафрейма ```df```, исключив столбец ```Class```.
- Создайте объект ```Series``` под названием ```y``` из столбца ```Class```.
- Разбейте ```X``` и ```y``` на тренировочный и тестовый наборы данных при помощи функции ```train_test_split```, используя аргументы: ```test_size = 0.3```, ```random_state = 100```, ```stratify = y```.

У вас должны получиться объекты ```X_train```, ```X_test```, ```y_train``` и ```y_test```.

Просмотрите информацию о их форме.

Для поиска по сетке параметров задайте такие параметры:
  - ```parameters = [{'n_estimators': [10, 15]```,
  - ```'max_features': np.arange(3, 5)```,
  - ```'max_depth': np.arange(4, 7)}]```

Создайте модель ```GridSearchCV``` со следующими аргументами:
- ```estimator = RandomForestClassifier(random_state = 100)```,
- ```param_grid = parameters```,
- ```scoring = 'roc_auc'```,
- ```cv=3```.

Обучите модель на тренировочном наборе данных (может занять несколько минут).

Просмотрите параметры лучшей модели с помощью атрибута ```best_params_```.

Предскажите вероятности классов с помощью полученнной модели и метода ```predict_proba```.

Из полученного результата (массив ```Numpy```) выберите столбец с индексом 1 (вероятность класса 1) и запишите в массив ```y_pred_proba```.

Из модуля ```sklearn.metrics``` импортируйте метрику ```roc_auc_score```.

Вычислите ```AUC``` на тестовых данных и сравните с результатом,полученным на тренировочных данных, используя в качестве аргументовмассивы ```y_test``` и ```y_pred_proba```.

#### En

In this task we will be working with the dataset, which we are already familiar with from the ```Matplotlib``` library homework, the Credit Card Fraud Detection dataset.

For this dataset, we will solve the task of classification - we will determine which credit card transactions are fraudulent. This dataset is highly unbalanced (as fraud cases are relatively rare), so the use of the ```accuracy``` metric will not be helpful and will not help us choose the best model.

We will calculate the ```AUC```, which is the area under the ROC curve.

- Import from the corresponding modules ```RandomForestClassifier```, ```GridSearchCV``` and ```train_test_split```.
- Download the dataset creditcard.csv and create the dataframe ```df```.
- Using the ```value_counts``` method with the ```normalize = True``` argument, make sure that the sample is unbalanced. Using the ```info``` method, check that all columns contain numerical data and that there are no omissions. Apply the following setting so that you can view all columns of the dateframe (```pd.options.display.max_columns = 100```).
- Look through the first 10 rows of the dateframe ```df```.
- Create the dateframe ```X``` from the dateframe ```df``` by deleting the column ```Class```.
- Create a ```Series``` object called ```y``` from the ```Class``` column.
- Break down ```X``` and ```y``` into training and test datasets using the ```train_test_split``` function, using arguments: ```test_size = 0.3```, ```random_state = 100```, ```stratify = y```.

You should get objects ```X_train```, ```X_test```, ```y_train``` and ```y_test```.

Take a look at their form.

To search the grid of parameters, set these parameters:
  - ```parameters = [{'n_estimators': [10, 15]```,
  - ```'max_features': np.arange(3, 5)```,
  - ```'max_depth': np.arange(4, 7)}]```.

Create a ```GridSearchCV``` model with the following arguments:
- ```estimator = RandomForestClassifier(random_state = 100)```,
- ```param_grid = parameters```,
- ```scoring = 'roc_auc'```,
- ```cv = 3```.

Train the model on a training data set (may take several minutes).

View the parameters of the best model using the attribute ```best_params_```.

Predict class probabilities using the resulting model and ```predict_proba``` method.

From the result obtained (```Numpy``` array), select the column with index 1 (class 1 probability) and write into the ```y_pred_proba``` array.

From the ```sklearn.metrics``` module, import the ```roc_auc_score``` metric.

Calculate the ```AUC``` on the test data and compare it with the result obtained on the training data using the arrays ```y_test``` and ```y_pred_proba``` as arguments.

# Contributing

Pull requests are welcome.

# Source

[Geekbrains](https://geekbrains.ru)
