# Pi-value-Calculation-Korshikov
 

В моей лабораторной работе реализовано вычисление числа Pi методом Монте-Карло. Ввиду проблем с видеокартой, вычисления проводились в Google Colaboratory. 

С результатами можно ознакомиться в файле results.xlsx. Как мы видим, чем больше точек, тем вцелом точнее вычисляется число Pi(т.е. уменьшается величина ошибки Error rate). Это связано с особенностями реализации самого метода, который подразумевает перебор точек на площади. С этой же реализацией связано колебание в точности (при увеличении количества точек Error rate не всегда уменьшается, а иногда даже увеличивается, в тех ситуациях, когда распределение точек было не слишком удачным). Однако, вцелом наблюдается тенденция к повышению точности и, даже случаи неудачного распределения не так сильно снижают точность вычисления числа Pi как при малом числе точек.


Разрыв в скорости между CPU и GPU также увеличивается по мере увеличения количества точек. Это связано с особенностями работы GPU, так как ему нужно время наподгрузку данных в память, на что уходит какое-то время. Однако, по мере роста числа точек, оно всё слабее влияет на выполняемую операцию.
