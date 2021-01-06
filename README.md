# Bonch_Project_Java
Theme: Калькулятор выражений
<h2>Discipline</h2>
<li>Технологии и методы программирования a.k.a. Разработка защищённых приложений</li>

<h2>Project Goal</h2>
<li>Реализовать калькулятор, вычисляющий выражение в заданном контексте.</li>
<li>Освоить средства создания UML диаграмм на Java</li>

<h2>Description</h2>
Поскольку калькулятор поддерживает простейшие операции:
<li>Сложение  + </li>
<li>Вычитание - </li>
<li>Умножение * </li>
<li>Деление   / </li>
<li>Расстановка открывающей ( скобок и закрывающей ) скобок 
</li>
</br>
Было решено рассмотреть возможные варианты решения поставленной задачи:</br>
1. Располагать операции в виде Бинарного дерева, ресурсоемко и сложно! </br>
2. Разбивать выражение на токены. </br>
Был выбран второй вариант.</br>

</br>

Также при выполнении задачи был открыт следующий термин: 
<blockquote>
Обратная польская нотация — форма записи математических и логических выражений, </br>
в которой операнды расположены перед знаками операций. 
</blockquote>

<h3>Логика программы</h3> 
Мы посимвольно пробегаемся по всему выражению, каждому символу соответствует определенный приоритет:
<li>Умножение «*» или Деление «/»	 	приоритет 3	</li>
<li>Сложение «+» или Вычитание «–» 	приоритет 2 </li>
<li>Открывающая скобка «(» 			приоритет 1     </li>
<li>Числа «0…9» 				приоритет 0             </li>
<li>Закрывающая скобка «)»			приоритет  -1   </li>

<h3>Программа выполняется с некоторыми оговорками:</h3> 
<li>если нам встречается число, то мы выводим его в строку вывода;</li>
<li>если встречается математический знак, то мы кладем его в стек, 
при этом проверяя стек на пустоту, если стек не пустой, 
то нужно достать все знаки из него до тех пор, пока приоритет последующего знака не будет меньше текущего;</li>

<h3>По прохождению программы у нас имеется два набора данных:</h3>
Строке вывода, в которой находятся набор переданных чисел
Стек с математическими операциями
Полученные два набора данных преобразуются в обратную польскую нотацию, из которой и получается итоговый ответ по следующей логике:
	<li>если нам встречается число, то оно передается в стек</li>
	<li>если нам встречается математическая операция, то берутся последние два элемента в стеке и над ними выполняется соответствующее преобразование, которое записывается в стек;</li>

<h6>Я не хотел сдавать экзамен</h6>
<h6>Поэтому сделал следующий проект</h6>
