# Массивы
***

Массивы в системе WebTutor в общем случае требуют объявления:

    // одномерный массив
    var array1 = new Array();

    // двумерный массив
    var array2 = new Array()();




Обращение к элементам массива имеет следующий вид:

    // одномерный массив
    array1[0]

    // двумерный массив
    array2[0][2]

Нумерация членов массива начинается с 0.

Для работы с массивами используются встроенные функции. В системе WebTutor часто встречаются следующие встроенные функции:

**ArrayCount(НаименованиеМассива)** - возвращает количество элементов массива.

**ArrayOptFirstElem(НаименованиеМассива)** - возвращает первый элемент заданного массива.

---

К массивам применима конструкция цикла **for... in**.

---

Примеры:


    var a = new Array();
    a[0] = 5;
    a[1] = 6;
    a[2] = 4;
    a[3] = 7;
    a[4] = 3;
    a[5] = 8;

    // Расчет суммы элементов массива
    summa01 = 0;
    for (i = 1; i < ArrayCount(a); i++)
    {
	      summa01 = summa01 + a[i];
    } 
    alert("Сумма элементов массива равна " + summa01 + "\n" + 
        "Количество элементов массива равно " + ArrayCount(a) + "\n"  + 
        "Первый элемент массива равен " + ArrayOptFirstElem(a));




---

Пример использования оператора **for**:

Скопируйте приведенный код в созданный нами агент **Тестовый агент** на вкладку **"Выполняемый код"** (предыдущий код, введенный ранее на эту вкладку, можно удалить) и запустите агент, нажав на кнопку **Выполнить агент на стороне клиента**.

    a = 0;
    b = 10;
    for (i = 1; i < b; i++)
    {
    	a++;
    }
    alert("Переменная a равна " + a);

---

Результат выполнения агента:

![](for01.PNG)

Изменяйте значения переменных **a** и **b** и понаблюдайте, как это влияет на полученный результат.



 


***
<dd><li> <a href="1_language.md"> Возврат к части 1</a></dd>
<dd><li> <a href="README.md"> Возврат к оглавлению</a></dd>