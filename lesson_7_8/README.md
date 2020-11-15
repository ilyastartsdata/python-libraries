# Homework #7_8 :atom:

Homework for the class **'Training without a teacher'**

Python libraries for Data Science

# List of the tasks

## Task #1

#### Ru

Импортируйте библиотеки ```pandas```, ```numpy``` и ```matplotlib```.

Загрузите "Boston House Prices dataset" из встроенных наборов данных библиотеки ```sklearn```.

Создайте датафреймы ```X``` и ```y``` из этих данных.

Разбейте эти датафреймы на тренировочные (```X_train```, ```y_train```) и тестовые (```X_test```, ```y_test```) с помощью функции ```train_test_split``` так, чтобы размер тестовой выборки составлял 20% от всех данных, при этом аргумент ```random_state``` должен быть равен 42.

Масштабируйте данные с помощью ```StandardScaler```.

Постройте модель TSNE на тренировочный данных с параметрами: ```n_components = 2, learning_rate = 250, random_state = 42```.

Постройте диаграмму рассеяния на этих данных.

#### En

Import libraries ```pandas```, ```numpy``` and ```matplotlib```.

Download the "Boston House Prices dataset" from the built-in library data sets ```sklearn```.

Create the dataset ```X``` and ```y``` from these data sets.

Break down these dataset into training (```X_train```, ```y_train```) and test (```X_test```, ```y_test```) data frames using the function ```train_test_split``` so that the test sample size is 20% of all data and the argument ```random_state``` should be 42.

Scale the data with ```StandardScaler```.

Build the TSNE model on training data with parameters: ```n_components = 2, learning_rate = 250, random_state = 42```.

Build a scatter plot on this data.

## Task #2

#### Ru

С помощью ```KMeans``` разбейте данные из тренировочного набора на 3 кластера, используйте все признаки из датафрейма ```X_train```.

Параметр ```max_iter``` должен быть равен 100, ```random_state``` сделайте равным 42.

Постройте еще раз диаграмму рассеяния на данных, полученных с помощью ```TSNE```, и раскрасьте точки из разных кластеров разными цветами.

Вычислите средние значения ```price``` и ```CRIM``` в разных кластерах.

#### En

Use ```KMeans``` to break down the data from the training kit into 3 clusters, use all features from the dataframe ```X_train```.

The parameter ```max_iter``` should be 100, ```random_state``` make it 42.

Draw the scatter plot again on the data from ```TSNE``` and colour the points from the different clusters.

Calculate the average values of ```price``` and ```CRIM``` in the different clusters.

## Task #3 (Optional)

#### Ru

Примените модель ```KMeans```, построенную в предыдущем задании, к данным из тестового набора.

Вычислите средние значения ```price``` и ```CRIM``` в разных кластерах на тестовых данных.

#### En

Apply the ```KMeans``` model built in the previous task to data from the test set.

Calculate average ```price``` and ```CRIM``` values in different clusters on the test data.

# Contributing

Pull requests are welcome.

# Source

[Geekbrains](https://geekbrains.ru)
