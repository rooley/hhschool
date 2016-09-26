# hhschool

Задача 1 (MagicSequence)

В некоторых числах можно найти последовательности цифр, которые в сумме дают 10. К примеру, в числе 3523014 целых четыре таких последовательности.
352, 523, 5230, 23014

Можно найти и такие замечательные числа, каждая цифра которых входит в по крайней мере одну такую последовательность.
Например, 3523014 является замечательным числом, а 28546 — нет (в нём нет последовательности цифр, дающей в сумме 10 и при этом включающей 5). 

Найдите количество этих замечательных чисел в интервале [1, 2100000] (обе границы — включительно).

Реализация

В конструктор передаются нижняя и верхняя границы, а также сумма последовательности цифр (по условию задачи 10).

Задача 2 (Equation)

Дано равенство, в котором цифры заменены на буквы:
rqr + rrsw = rssx
(Количество различных символов - 5. Последовательность символов произвольная как по длине так и по позиции).

Найдите сколько у него решений, если различным буквам соответствуют различные цифры (ведущих нулей в числе не бывает).

Реализация

В конструктор передаются 3 строки, с заменой символов на a, b, c, d, e. Например для rqr + rrsw = rssx это будут строки aba, aacd, acce.  

Задача 3 (DigitPermutation)

Число 125874 и результат умножения его на 2 — 251748 можно получить друг из друга перестановкой цифр. 

Найдите наименьшее положительное натуральное x такое, что числа 3*x, 6*x можно получить друг из друга перестановкой цифр.

Реализация

В конструктор передаются 2 множителя (в условии 3 и 6). Метод getX() возвращает результат.

Задача 4 (Palindrome)

Если мы возьмем 47, перевернем его и сложим, получится 47 + 74 = 121 — число-палиндром. 

Если взять 349 и проделать над ним эту операцию три раза, то тоже получится палиндром: 
349 + 943 = 1292
1292 + 2921 = 4213
4213 + 3124 = 7337

Найдите количество положительных натуральных чисел меньших 13776 таких, что из них нельзя получить палиндром за 50 или менее применений описанной операции (операция должна быть применена хотя бы один раз).

Реализация

В статический метод getCount() передаётся максимальная граница (в условии 13776).

Задача 5 (Spiral)

Рассмотрим спираль, в которой, начиная с 1 в центре, последовательно расставим числа по часовой стрелке, 
пока не получится спираль 5 на 5 

21 22 23 24 25
20  7  8  9 10
19  6  1  2 11
18  5  4  3 12
17 16 15 14 13
Можно проверить, что сумма всех чисел на диагоналях равна 101. 

Чему будет равна сумма чисел на диагоналях, для спирали размером 1013 на 1013?

Реализация

В статический метод sumOfDiagonals() передаётся размер спирали.