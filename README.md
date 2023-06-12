Задача: Реализовать предыдущую задачу для списка, имеющегоорганизацию однонаправленного (двунаправленного) кольца.
Алгоритм программы: Программа определяет две структуры: Grade (Оценка) и Student (Студент). Структура Grade представляет оценку студента, а структура Student представляет студента с его личной информацией, группой и оценками.
Программа объявляет различные функции для разных операций: addStudent (добавление студента) для добавления нового студента, delStudent (удаление студента) для удаления студентов с плохой успеваемостью, sortingStudents (сортировка студентов) для сортировки студентов по фамилиям или группам, seeStudents (просмотр студентов) для отображения информации о всех студентах и changeStudent (изменение информации о студенте) для изменения информации о конкретном студенте.
В функции main программа отображает меню с вариантами операций и запрашивает ввод пользователя с помощью функции _getch (функция из библиотеки <conio.h>).
В зависимости от выбора пользователя программа вызывает соответствующие функции для выполнения желаемых операций.
Программа использует динамическое выделение памяти для создания новых объектов студентов и оценок при добавлении студентов и соответствующим образом изменяет структуру связанного списка.
Программа использует комбинацию циклов, условных операторов и указателей для манипуляции и отображения данных о студентах.
Ссылка на яндекс диск с примером работы: https://disk.yandex.ru/i/3AY5ms5TKUM2Wg
