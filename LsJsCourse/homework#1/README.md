## Задание:

>Написать рекурсивную функцию с именем `consoleRec`, которая выводит все значения массива на экран
>Функция должна **рекурсивно** выводить элементы массива на экран.
>Запрещено использовать циклы и методы для работы с массивами.
>Функция должна принимать два аргумента: массив и… что-то еще. Что именно - остается на ваше усмотрение. Пример вызова:

```javascript
consoleRec(['я', 'умею', 'писать', 'рекурсивные', 'функции'], ???);
должна вывести на экран:
я
умею
писать
рекурсивные
функции
```

## Моё решение

Код решения вы можете увидеть в файле index.js
Ход моих мыслей: раз нам нельзя использовать методы для работы с массивом, значит нам нужна числовая переменная для вывода значения массива по его индексу как array[index], поэтому вторым параметром мы передаем точку входа 'entryPoint' и после каждой итерации увеличиваем её на единицу и сравнимаем с длинной массива, если точка входа меньше длинны массива, то вызываем следующую итерацию.