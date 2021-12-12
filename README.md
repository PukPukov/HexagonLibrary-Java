* HexagonLibrary
** Описание
Универсальная библиотека для создания гексагональных сеток и работы с ними. 
** Преимущества
- Осевая система координат
- Деление гексагона на примитивные компоненты для реализации любых задач
- Широчайшее API
- Набор базовых методов для работы с сетками шестиугольников (Перевод пиксельных координат в осевые, нахождение соседей шестиугольника, нахождение координат вершин шестиугольника...)
- Набор дополнительных методов (Создание регионов, работа с массивами гексагонов, кодирование гексагона...)
** Примеры кода
#+BEGIN_SRC java
// Создание гексагональной сетки. Ориентация, начало координат, размер гексагона, настройки Morton64 (в большинстве случаев менять не надо)
HexagonalGrid grid = new HexagonalGrid(Orientation.FLAT, new Point(0, 0), new Point(20, 10), new Morton64(2, 32));

// Получение гексагона по пиксельным координатам
Hexagon hexagon = grid.getHexagon(new Point(50, 50));
#+END_SRC
