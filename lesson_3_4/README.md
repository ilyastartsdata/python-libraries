# Homework #2 :atom:

Homework for the class **'Visualisation of data in Matplotlib'**

Python libraries for Data Science

# List of the tasks

## Task #1

#### Ru

Загрузите модуль pyplot библиотеки matplotlib с псевдонимом plt, а также библиотеку numpy с псевдонимом np.

Примените магическую функцию %matplotlib inline для отображения графиков в Jupyter Notebook и настройки конфигурации ноутбука со значением 'svg' для более четкого отображения графиков.

Создайте список под названием x с числами 1, 2, 3, 4, 5, 6, 7 и список y с числами 3.5, 3.8, 4.2, 4.5, 5, 5.5, 7.

С помощью функции plot постройте график, соединяющий линиями точки с горизонтальными координатами из списка x и вертикальными - из списка y.

Затем в следующей ячейке постройте диаграмму рассеяния (другие названия - диаграмма разброса, scatter plot).

#### En

Download the pyplot module of the matplotlib library with the nickname plt as well as the numpy library with the np alias.

Apply the magic function %matplotlib inline to display the charts in Jupyter Notebook and configure the notebook with a value of 'svg' to display the charts more clearly.

Create a list called x with the numbers 1, 2, 3, 4, 5, 6, 7 and a list of y with the numbers 3.5, 3.8, 4.2, 4.5, 5, 5.5, 7.

Using the plot function, draw a graph connecting the lines of points with horizontal coordinates from the x list and vertical coordinates from the y list.

Then build a scatter plot in the next cell (other names is scatter plot).

## Task #2

#### Ru

С помощью функции linspace из библиотеки Numpy создайте массив t из 51 числа от 0 до 10 включительно.

Создайте массив Numpy под названием f, содержащий косинусы элементов массива t.

Постройте линейную диаграмму, используя массив t для координат по горизонтали,а массив f - для координат по вертикали. Линия графика должна быть зеленого цвета.

Выведите название диаграммы - 'График f(t)'. Также добавьте названия для горизонтальной оси - 'Значения t' и для вертикальной - 'Значения f'.

Ограничьте график по оси x значениями 0.5 и 9.5, а по оси y - значениями -2.5 и 2.5.

#### En

Use the linspace function from the Numpy library to create an array of t from 51 numbers 0 to 10 inclusive.

Create a Numpy array called f that contains the cosines of array t elements.

Build a line chart using array t for horizontal coordinates and array f for vertical coordinates. The line chart should be green.

Print the name of the diagram - 'Chart f(t)'. Also add names for the horizontal axis - 't values' and for the vertical axis - 'f values'.

Limit the graph on the x axis to 0.5 and 9.5, and on the y axis to -2.5 and 2.5.

## Task #3 (Optional)

#### Ru

С помощью функции linspace библиотеки Numpy создайте массив x из 51 числа от -3 до 3 включительно.

Создайте массивы y1, y2, y3, y4 по следующим формулам:

- y1 = x^2
- y2 = 2 * x + 0.5
- y3 = -3 * x - 1.5
- y4 = sin(x)

Используя функцию subplots модуля matplotlib.pyplot, создайте объект matplotlib.figure.Figure с названием fig и массив объектов Axes под названием ax,причем так, чтобы у вас было 4 отдельных графика в сетке, состоящей из двух строк и двух столбцов. 

В каждом графике массив x используется для координат по горизонтали.В левом верхнем графике для координат по вертикали используйте y1,в правом верхнем - y2, в левом нижнем - y3, в правом нижнем - y4.Дайте название графикам: 'График y1', 'График y2' и т.д.

Для графика в левом верхнем углу установите границы по оси x от -5 до 5.
Установите размеры фигуры 8 дюймов по горизонтали и 6 дюймов по вертикали.
Вертикальные и горизонтальные зазоры между графиками должны составлять 0.3.

#### En

Use the Numpy library's linspace function to create an x array of 51 numbers from -3 to 3 inclusive.

Create arrays of y1, y2, y3, y4 using the following formulas:

- y1 = x^2
- y2 = 2 * x + 0.5
- y3 = -3 * x - 1.5
- y4 = sin(x)

Using the subplots function of the matplotlib.pyplot module, create a matplotlib.figure.figure object named fig and an array of Axes objects named ax, so that you have 4 separate charts in a grid consisting of two rows and two columns. 

In each chart, the x array is used for horizontal coordinates. In the upper left chart, use y1 for vertical coordinates, in the upper right chart, use y2, in the lower left chart, use y3, and in the lower right chart, use y4.Give the chart a name: 'y1 chart', 'y2 chart', etc.

For the chart in the upper left corner, set the boundaries on the x axis from -5 to 5.
Set the size of the figure to 8 inches horizontally and 6 inches vertically.
Vertical and horizontal gaps between charts should be 0.3.

## Task #4 (Optional)

#### Ru



#### En



# Contributing

Pull requests are welcome.

# Source

[Geekbrains](https://geekbrains.ru)
