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

Импортируйте библиотеку Pandas и дайте ей псевдоним pd. 

Создайте датафрейм authors со столбцами author_id и author_name, в которых соответственно содержатся данные: [1, 2, 3] и ['Тургенев', 'Чехов', 'Островский'].

Затем создайте датафрейм book cо столбцами author_id, book_title и price, в которых соответственно содержатся данные: 
[1, 1, 1, 2, 2, 3, 3], ['Отцы и дети', 'Рудин', 'Дворянское гнездо', 'Толстый и тонкий', 'Дама с собачкой', 'Гроза', 'Таланты и поклонники'], [450, 300, 350, 500, 450, 370, 290].

#### En

Import the Pandas library and give it the nickname pd. 

Create a dateframe with the author_id and author_name columns, which contain the data respectively: [1, 2, 3] and ['Turgenev', 'Chekhov', 'Ostrovsky'].

Then create a dateframe book with the author_id, book_title and price columns, which contain the data respectively: 
[1, 1, 1, 2, 2, 3, 3], ['Fathers and Children', 'Rudin', 'Noble Nest', 'Fat and Thin', 'Lady with a Dog', 'Thunderstorm', 'Talents and Admirers'], [450, 300, 350, 500, 450, 370, 290].

## Task 2

#### Ru

Получите датафрейм authors_price, соединив датафреймы authors и books по полю author_id.

#### En

Get the authors_price dataframe by linking the authors and books data frames to the author_id field.

## Task 3

#### Ru

Создайте датафрейм top5, в котором содержатся строки из authors_price с пятью самыми дорогими книгами.

#### En

Create a top5 dataframe containing the lines from authors_price with the five most expensive books.

## Task #4

#### Ru

Создайте датафрейм authors_stat на основе информации из authors_price. В датафрейме authors_stat должны быть четыре столбца: author_name, min_price, max_price и mean_price, в которых должны содержаться соответственно имя автора,минимальная, максимальная и средняя цена на книги этого автора.

#### En

Create a dataframe authors_stat based on information from authors_price. The authors_stat dateframe should have four columns: author_name, min_price, max_price and mean_price, which should contain, respectively, the name of the author, the minimum, maximum and average price of the books of this author.

## Task #5 (Optional)

#### Ru

Создайте новый столбец в датафрейме authors_price под названием cover, в нем будут располагаться данные о том, какая обложка у данной книги - твердая или мягкая. В этот столбец поместите данные из следующего списка:
['твердая', 'мягкая', 'мягкая', 'твердая', 'твердая', 'мягкая', 'мягкая'].
Просмотрите документацию по функции pd.pivot_table с помощью вопросительного знака.Для каждого автора посчитайте суммарную стоимость книг в твердой и мягкой обложке. Используйте для этого функцию pd.pivot_table. При этом столбцы должны называться "твердая" и "мягкая", а индексами должны быть фамилии авторов. Пропущенные значения стоимостей заполните нулями, при необходимости загрузите библиотеку Numpy.
Назовите полученный датасет book_info и сохраните его в формат pickle под названием "book_info.pkl". Затем загрузите из этого файла датафрейм и назовите его book_info2. Удостоверьтесь, что датафреймы book_info и book_info2 идентичны.

#### En

Create a new column in the authors_price dataframe called cover, which will contain information about whether the cover of a given book is hard or soft. Place data from the following list in this column:
['hard', 'soft', 'soft', 'hard', 'hard', 'soft'].
Review the documentation for the pd.pivot_table function with the question mark. For each author, calculate the total value of hard and softcover books. Use the pd.pivot_table function for this. The columns should be called "hard" and "soft", and the indexes should be the names of the authors. Fill in the missing cost values with zeros and download the Numpy library if necessary.
Name the book_info dataset you have received and save it in the pickle format called "book_info.pkl". Then download the dataset from this file and name it book_info2. Make sure that the dateframes book_info and book_info2 are identical.

# Contributing

Pull requests are welcome.

# Source

[Geekbrains](https://geekbrains.ru)
