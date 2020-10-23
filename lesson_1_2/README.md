# Homework #1 :atom:

Homework for the class **'Calculations with Numpy. Working with data in Pandas'**

Python libraries for Data Science

# List of the tasks

> Calculations with Numpy

## Task #1

#### Ru

Импортируйте библиотеку Numpy и дайте ей псевдоним np.

Создайте массив Numpy под названием a размером 5x2, то есть состоящий из 5 строк и 2 столбцов. 

Первый столбец должен содержать числа 1, 2, 3, 3, 1, а второй - числа 6, 8, 11, 10, 7. Будем считать, что каждый столбец - это признак, а строка - наблюдение. 

Затем найдите среднее значение по каждому признаку, используя метод mean массива Numpy. 
Результат запишите в массив mean_a, в нем должно быть 2 элемента.

#### En

Import the Numpy library and give it an alias np.

Create a Numpy array called a 5x2, i.e. consisting of 5 rows and 2 columns. 

The first column should contain numbers 1, 2, 3, 1 and the second column should contain numbers 6, 8, 11, 10, 7. We will assume that each column is a sign and a row is an observation. 

Then find the average for each feature using the Numpy array mean method. 
Write the result into the mean_a array and there should be 2 elements.

## Task #2

#### Ru

Вычислите массив a_centered, отняв от значений массива “а” средние значения соответствующих признаков, содержащиеся в массиве mean_a. 
Вычисление должно производиться в одно действие. Получившийся массив должен иметь размер 5x2.

#### En

Calculate the array a_centered by taking the average values of the relevant attributes contained in the mean_a array from the values of the array "a". 
The calculation must be done in one action. The resulting array must be 5x2 in size.

## Task #3

#### Ru

Найдите скалярное произведение столбцов массива a_centered. В результате должна получиться величина a_centered_sp. 
Затем поделите a_centered_sp на N-1, где N - число наблюдений.

#### En

Find the scalar work of the columns in the a_centered array. This should result in the value a_centered_sp. 
Then divide a_centered_sp by N-1, where N is the number of observations.

## Task #4 (Optional)

#### Ru

Число, которое мы получили в конце задания 3 является ковариацией двух признаков, содержащихся в массиве “а”. 
В задании 3 мы делили сумму произведений центрированных признаков на N-1, а не на N, поэтому полученная нами величина является несмещенной оценкой ковариации.

В этом задании проверьте получившееся число, вычислив ковариацию еще одним способом - с помощью функции np.cov. 
В качестве аргумента m функция np.cov должна принимать транспонированный массив “a”. 
В получившейся ковариационной матрице (массив Numpy размером 2x2) искомое значение ковариации будет равно элементу в строке с индексом 0 и столбце с индексом 1.

#### En

The number that we received at the end of assignment 3 is the covariance of the two features contained in the array "a". 
In Assignment 3, we divided the sum of the works of centered features into N-1 rather than N, so the value we obtained is an unbiased covariance estimate.

In this task, check the resulting number by calculating covariance in another way - using the np.cov function. 
The np.cov function should accept the transposed array "a" as an argument m. 
In the resulting covariance matrix (2x2 Numpy array), the covariance value sought will be equal to the element in the row with index 0 and column with index 1.

> Working with data in Pandas

## Task 1

#### Ru


#### En

# Contributing

Pull requests are welcome.

# Source

[Geekbrains](https://geekbrains.ru)
