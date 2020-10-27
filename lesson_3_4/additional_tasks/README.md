# Additional tasks :atom:

Python libraries for Data Science

# List of the tasks

#### Ru

- Создать одномерный массив Numpy под названием a из 12 последовательных целых чисел чисел от 12 до 24 невключительно
- Создать 5 двумерных массивов разной формы из массива a. Не использовать в аргументах метода reshape число -1.
- Создать 5 двумерных массивов разной формы из массива a. Использовать в аргументах метода reshape число -1 (в трех примерах - для обозначения числа столбцов, в двух - для строк).
- Можно ли массив Numpy, состоящий из одного столбца и 12 строк, назвать одномерным?
- Cоздать массив из 3 строк и 4 столбцов, состоящий из случайных чисел с плавающей запятой из нормального распределения со средним, равным 0 и среднеквадратичным отклонением, равным 1.0. Получить из этого массива одномерный массив с таким же атрибутом size, как и исходный массив.
- Создать массив a, состоящий из целых чисел, убывающих от 20 до 0 невключительно с интервалом 2.
- Создать массив b, состоящий из 1 строки и 10 столбцов: целых чисел, убывающих от 20 до 1 невключительно с интервалом 2. В чем разница между массивами a и b?
- Вертикально соединить массивы a и b. a - двумерный массив из нулей, число строк которого больше 1 и на 1 меньше, чем число строк двумерного массива b, состоящего из единиц. Итоговый массив v должен иметь атрибут size, равный 10.
- Создать одномерный массив а, состоящий из последовательности целых чисел от 0 до 12. Поменять форму этого массива, чтобы получилась матрица A (двумерный массив Numpy), состоящая из 4 строк и 3 столбцов. Получить матрицу At путем транспонирования матрицы A. Получить матрицу B, умножив матрицу A на матрицу At с помощью матричного умножения. Какой размер имеет матрица B? Получится ли вычислить обратную матрицу для матрицы B и почему?
- Инициализируйте генератор случайных числе с помощью объекта seed, равного 42.
- Создайте одномерный массив c, составленный из последовательности 16-ти случайных равномерно распределенных целых чисел от 0 до 16 невключительно. 
- Поменяйте его форму так, чтобы получилась квадратная матрица C. Получите матрицу D, поэлементно прибавив матрицу B из предыдущего вопроса к матрице C, умноженной на 10. Вычислите определитель, ранг и обратную матрицу D_inv для D.
- Приравняйте к нулю отрицательные числа в матрице D_inv, а положительные - к единице. Убедитесь, что в матрице D_inv остались только нули и единицы. С помощью функции numpy.where, используя матрицу D_inv в качестве маски, а матрицы B и C - в качестве источников данных, получите матрицу E размером 4x4.  Элементы матрицы E, для которых соответствующий элемент матрицы D_inv равен 1, должны быть равны соответствующему элементу матрицы B, а элементы матрицы E, для которых соответствующий элемент матрицы D_inv равен 0, должны быть равны соответствующему элементу матрицы C.

#### En

- Create a one-dimensional Numpy array called a of 12 consecutive integers from 12 to 24.
- Create 5 2D arrays of different shapes from array a. Do not use -1 in reshape method arguments.
- Create 5 two-dimensional arrays of different shapes from array a. Use -1 in reshape method arguments (in three examples - for the number of columns, in two - for rows).
- Can a Numpy array consisting of one column and 12 rows be called a one-dimensional array?
- Create an array of 3 rows and 4 columns consisting of random floating point numbers from a normal distribution with an average deviation of 0 and a standard deviation of 1.0. Get a one-dimensional array from this array with the same size attribute as the original array.
- Create an array a consisting of integers decreasing from 20 to 0 at intervals of 2.
- Create array b consisting of 1 row and 10 columns: integers decreasing from 20 to 1 non inclusively at intervals of 2. What is the difference between arrays a and b?
- Vertically connect arrays a and b. a - a two-dimensional array of zeros with the number of rows greater than 1 and 1 less than the number of rows in a two-dimensional array b consisting of units. The resulting array v must have a size attribute of 10.
- Create a one-dimensional array a consisting of a sequence of integers from 0 to 12. Change the shape of this array to create a matrix A (two-dimensional array Numpy) consisting of 4 rows and 3 columns. Get Matrix At by transposing Matrix A. Obtain matrix B by multiplying matrix A by matrix At. What size does Matrix B have? Will it be possible to calculate the inverse matrix for matrix B and why?
- Initialize a random number generator with a seed object of 42.
- Create a one-dimensional array of c made up of a sequence of 16 random evenly distributed integers from 0 to 16. 
- Change its shape so that a square matrix C is created. Get matrix D by elementally adding matrix B from the previous question to matrix C multiplied by 10. Calculate determinant, rank and inverse matrix D_inv for D.
- Equate the negative numbers in matrix D_inv and the positive numbers in matrix D_inv with one. Make sure that only zeros and units are left in the D_inv matrix. Using the function numpy.where, using matrix D_inv as a mask and matrices B and C as data sources, obtain matrix E with a size of 4x4.  The elements of matrix E, for which the corresponding element of matrix D_inv is 1, must be equal to the corresponding element of matrix B and the elements of matrix E, for which the corresponding element of matrix D_inv is 0, must be equal to the corresponding element of matrix C.

# Contributing

Pull requests are welcome.

# Source

[Geekbrains](https://geekbrains.ru)
