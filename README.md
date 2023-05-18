## Домашнее задание от 21.04 
### Шаблоны в C++

Вспомнить тему обсуждения можно с помощью [статьи](https://habr.com/ru/articles/599801/) \
А про концепты можно найти [тут](https://habr.com/ru/companies/yandex_praktikum/articles/556816/)

1. Напишите шаблонную функцию, вычисляющую сумму элементов вектора. Проверок на то, что объекты этого типа умеют суммироваться пока можно не добавлять. Результатом работы функции ожидается один объект того же типа -- сумма всех элементов переданного вектора. `T sum(vector<T> a)`

2. Реализовать шаблонное дерево поиска, балансировка не требуется. Логика добавления и поиска аналогична обсужденной ранее, но подходит любая, если в результате получается корректное дерево поиска, соответсвующее всем добавленным элементам.
    * Реализация шаблонного класса одной вершины дерева `Node<T> { T value; Node<T>* next; }` 
    * Реализация шаблонного класса самого дерева. Все вершины должны хранить значения одного типа, но самое дерево должно быть можно создать для разных типов. Требуются методы `void add(T value)` (добавить новых элемент) и `bool find(T value)` (поискать значение в дереве)