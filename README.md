Задача: Написать программу формирования ОПЗ и расчета полученного выражения. Разработать удобный интерфейс ввода исходных данных и вывода результатов. Язык программирования С++. Работу программы проверить на конкретном примере a-(b/c*(d+e)) a=5.6 b=3.2 c=0.9 d=1.7 e=4.8 результат=-17.51

Алгоритм программы: Программа определяет функцию isOperator, которая проверяет, является ли символ оператором (+, -, * или /). Функция performOperation выполняет операцию между двумя операндами, в зависимости от заданного оператора. Функция getOperatorPriority возвращает приоритет оператора. Операторы + и - имеют приоритет 1, а операторы * и / - приоритет 2. Функция evaluateRPN вычисляет значение выражения в обратной польской записи. Она использует стек операндов для выполнения операций. Выражение разделяется на токены (числа и операторы) с помощью istringstream, и каждый токен обрабатывается. Если токен является числом, оно помещается в стек операндов. Если токен является оператором, извлекаются два операнда из стека, выполняется операция, и результат помещается обратно в стек операндов. Функция infixToRPN преобразует инфиксное выражение в обратную польскую запись. Она использует стек операторов для сохранения операторов и их приоритетов. Выражение обрабатывается посимвольно. Если символ является числом, он добавляется в выходную строку rpn. Если символ является оператором, производится сравнение его приоритета с приоритетом операторов в стеке. Если приоритет текущего оператора меньше или равен приоритету оператора в стеке, операторы извлекаются из стека и добавляются в выходную строку. Если символ является открывающей скобкой (, он помещается в стек операторов. Если символ является закрывающей скобкой ), операторы извлекаются из стека и добавляются в выходную строку до тех пор, пока не встретится открывающая скобка. В функции main программа запрашивает у пользователя ввод инфиксного выражения. Затем она преобразует его в ОПЗ с помощью функции infixToRPN и выводит полученное выражение на экран. Затем она вычисляет значение выражения в ОПЗ с помощью функции evaluateRPN и выводит результат.

Ссылка на яндекс диск с примером работы:
