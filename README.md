Задача(a): Ввести массив из п целых чисел из заданного диапазона. Создать хеш-
таблицу из М элементов. Осуществить поиск элемента в хеш-таблице. Вы-
вести на экран исходный массив, хеш-таблицу и результат поиска. n=12  Диапазон значений=27000-58000  M=15  Схема хеширования c линейной адресацией

Алгоритм программы: Программа объявляет константы HASH_TABLE_SIZE, MIN_RANGE и MAX_RANGE, определяющие размер хеш-таблицы и диапазон значений ключей.
Функция hashFunction определяет хеш-функцию, которая принимает ключ и возвращает индекс в хеш-таблице.
В функции main программа запрашивает у пользователя количество элементов массива (n) и считывает элементы массива.
Создается пустая хеш-таблица с помощью вектора hashTable. Изначально все ячейки таблицы заполняются значением -1.
Для каждого элемента массива, попадающего в заданный диапазон (MIN_RANGE и MAX_RANGE), вычисляется хеш-значение с помощью хеш-функции. Затем производится поиск свободной ячейки в хеш-таблице с помощью линейного пробирования. Если найдена свободная ячейка, элемент добавляется в таблицу.
Программа выводит исходный массив и содержимое хеш-таблицы на экран.
Затем программа запрашивает у пользователя ключ для поиска и выполняет поиск этого ключа в хеш-таблице. При поиске используется хеш-функция и линейное пробирование до тех пор, пока не будет найден элемент с искомым ключом или не будет найдена свободная ячейка.
По результатам поиска программа выводит соответствующее сообщение.

Ссылка на яндекс диск с примером работы: https://disk.yandex.ru/i/jGMIrSDaH1r7HQ

Задача(б): Объявить и ввести массив структур из п элементов. Создать хеш-
таблицу из М элементов. Осуществить поиск элемента по ключу в хеш-
таблице. Вывести на экран исходный массив, хеш-таблицу и все поля найденной структуры. 
n=7  Поля структуры:фамилия, количество очков, занятое место  Ключевое поле:Занятое место  M=15  Схема хеширования c двойным хешированием

Алгоритм программы(б): Программа объявляет структуру Data, которая представляет информацию о студенте: фамилию (surname), количество очков (points) и занятое место (place).
Определяется константа TABLE_SIZE, которая определяет размер хеш-таблицы.
Создается класс HashTable, который содержит приватное поле table типа vector<Data> для хранения данных.
В классе HashTable определяются две хеш-функции: hash1(key) и hash2(key), которые используются для вычисления индекса в хеш-таблице.
В конструкторе класса HashTable происходит инициализация таблицы с помощью метода resize(TABLE_SIZE), чтобы создать вектор заданного размера.
Метод insert(data) вставляет данные в хеш-таблицу. Он вычисляет начальный индекс с помощью hash1(data.place) и шаг с помощью hash2(data.place), затем применяет линейное пробирование, чтобы найти свободную ячейку и вставить данные.
Метод search(key) выполняет поиск элемента по ключу в хеш-таблице. Он использует ту же логику вычисления индекса и шага, а затем применяет линейное пробирование до тех пор, пока не будет найден элемент с заданным ключом или не будет найдена свободная ячейка. Если элемент не найден, возвращается указатель nullptr, иначе возвращается указатель на найденный элемент.
Метод print() выводит содержимое хеш-таблицы на экран.
В функции main пользователь вводит данные о студентах (фамилия, количество очков, занятое место) и создается хеш-таблица.
Программа выводит исходный массив данных о студентах и содержимое хеш-таблицы.
Пользователь вводит ключ для поиска, и выполняется поиск элемента в хеш-таблице с помощью метода search(key). Результат поиска выводится на экран.

Ссылка на яндекс диск с примером работы(б): https://disk.yandex.ru/i/Wd1sLSOxw-PMCQ
