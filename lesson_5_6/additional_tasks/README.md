# Additional tasks 5_6 :atom:

Python libraries for Data Science

# List of the tasks

#### Ru

- Загрузите датасет Wine из встроенных датасетов ```sklearn.datasets``` с помощью функции ```load_wine``` в переменную ```data```
- Полученный датасет не является датафреймом. Это структура данных, имеющая ключи аналогично словарю. Просмотрите тип данных этой структуры данных и создайте список ```data_keys```, содержащий ее ключи
- Просмотрите данные, описание и названия признаков в датасете. Описание нужно вывести в виде привычного, аккуратно оформленного текста, без обозначений переноса строки, но с самими переносами и т.д
- Сколько классов содержит целевая переменная датасета? Выведите названия классов.
- На основе данных датасета (они содержатся в двумерном массиве ```Numpy```) и названий признаков создайте датафрейм под названием ```X```
- Выясните размер датафрейма ```X``` и установите, имеются ли в нем пропущенные значения
- Добавьте в датафрейм поле с классами вин в виде чисел, имеющих тип данных ```numpy.int64```. Название поля - ```'target'```
- Постройте матрицу корреляций для всех полей ```X```. Дайте полученному датафрейму название ```X_corr```
- Создайте список ```high_corr``` из признаков, корреляция которых с полем ```target``` по абсолютному значению превышает 0.5 (причем, само поле ```target``` не должно входить в этот список)
- Удалите из датафрейма ```X``` поле с целевой переменной. Для всех признаков, названия которых содержатся в списке ```high_corr```, вычислите квадрат их значений и добавьте в датафрейм ```X``` соответствующие поля с суффиксом '_2', добавленного к первоначальному названию признака. Итоговый датафрейм должен содержать все поля, которые, были в нем изначально, а также поля с признаками из списка ```high_corr```, возведенными в квадрат. Выведите описание полей датафрейма ```X``` с помощью метода ```describe```

#### En

- Download the Wine dataset from the built-in ```sklearn.datasets``` using the ```load_wine``` function to the variable data.
- The dataset received is not a dataframe. It is a data structure that has keys similar to a dictionary. Look at the data type of this data structure and create a list of ```data_keys``` containing its keys
- Look at the data, description and names of the attributes on the data sheet. The description should be displayed as a familiar, neatly arranged text, without line breaks, but with the line breaks themselves, etc.
- How many classes does the target variable in the dataset contain? Print the class names.
- Based on the data from the dataset (contained in the ```Numpy 2D array```) and the names of the attributes, create a dataset frame called ```X```
- Find out the size of the dateframe ```X``` and determine if there are any missing values in it
- Add to the dateframe a field with wine classes in the form of numbers that have the data type ```numpy.int64```. The name of the field is ```'target'```.
- Build a correlation matrix for all ```X``` fields. Give the resulting dataframe the name ```X_corr```
- Create a list of ```high_corr``` features whose correlation with the target field by an absolute value exceeds 0.5 (and the ```target``` field itself should not be included in this list).
- Remove the field with the target variable from dateframe ```X```. For all features whose names are contained in the ```high_corr``` list, calculate a square of their values and add the corresponding fields with the suffix '_2' added to the original feature name to the dateframe ```X```. The resulting dataframe must contain all fields that were originally in it, as well as fields with ```high_corr``` traits in the square. Output a description of the fields in the dateframe ```X``` using the method ```describe```

# Contributing

Pull requests are welcome.

# Source

[Geekbrains](https://geekbrains.ru)
