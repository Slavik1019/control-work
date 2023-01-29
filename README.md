# Задача: #
 Написать программу, которая из имеющегося массива строк формирует новый массив из строк, длина которых меньше, либо равна 3 символам. Первоначальный массив можно ввести с клавиатуры, либо задать на старте выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

 ## Примеры: ##

  [“Hello”, “2”, “world”, “:-)”] → [“2”, “:-)”] [“1234”, “1567”, “-2”, “computer science”] → [“-2”] [“Russia”, “Denmark”, “Kazan”] → []

  ### Текстовое описание решения: ###

  Программа принимает на вход количество элементов массива. Пользователь вводит массив с клаиватуры. Далее задаем массив arr1 размером size.Задаем переменную i (индекс элемента).Создаем переменную count (счетчик элементов подходящих под условие). Выводим полученный массив arr2. Вводим переменную maxSymbols (максимально допустимое количество символов в элементе). По условию maxSymbols = 3. Вводим элементы массива начиная с первого arr1[0], до тех пор, пока индекс [i] меньше длины массива size, прибавляя по одному. Каждый элемент массива проверяем по условию: длинна элемента arr[i] <= maxSymbols. Если условие соблюдено, увеличиваем count на один. Если нет - переходим к проверке следующего элемента массива arr1[i+1]. Заполняем новый массив arr2 в пределах цикла. Для этого повторно проводим проверку каждого элемента массива, чтобы длина элемента arr1[i] была больше или равна 3. Если условие соблюдено, элементу arr2[j] присваиваем соответствующее значение элемента arr1[i]. Записываем его в массив arr2. Если нет, переходим к проверке следующего элемента arr1[i+1]. Выводим полученный массив arr2.