[[_TOC_]]

# Задача:
Разработать набор модульных тестов
### Цель:

Научиться писать модульные тесты по TDD, так как модульные тесты является важной частью концепции Time To Market и часто применяется в современных проектах.

Описание/Пошаговая инструкция выполнения домашнего задания:

    Создать проект на gitlab/github.
    Настроить CI, чтобы можно было собирать проект и прогонять тесты.
    Необходимо реализовать операцию нахождения квадратного уравнения. Предположим, что эта операция описывается следующей функцией c поправкой на конкретный язык программирования. В ООП языках эта функция реализуется в виде метода класса.
    solve(double a, double b, double c): double[]
    здесь a, b, c - коэффициенты квадратного уравнения, функция возвращает список корней квадратного уравнения.
    Написать тест, который проверяет, что для уравнения x^2+1 = 0 корней нет (возвращается пустой массив)
    Написать минимальную реализацию функции solve, которая удовлетворяет данному тесту.
    Написать тест, который проверяет, что для уравнения x^2-1 = 0 есть два корня кратности 1 (x1=1, x2=-1)
    Написать минимальную реализацию функции solve, которая удовлетворяет тесту из п.5.
    Написать тест, который проверяет, что для уравнения x^2+2x+1 = 0 есть один корень кратности 2 (x1= x2 = -1).
    Написать минимальную реализацию функции solve, которая удовлетворяет тесту из п.7.
    Написать тест, который проверяет, что коэффициент a не может быть равен 0. В этом случае solve выбрасывает исключение.
    Примечание. Учесть, что a имеет тип double и сравнивать с 0 через == нельзя.
    Написать минимальную реализацию функции solve, которая удовлетворяет тесту из п.9.
    С учетом того, что дискриминант тоже нельзя сравнивать с 0 через знак равенства, подобрать такие коэффициенты квадратного уравнения для случая одного корня кратности два, чтобы дискриминант был отличный от нуля, но меньше заданного эпсилон. Эти коэффициенты должны заменить коэффициенты в тесте из п. 7.
    При необходимости поправить реализацию квадратного уравнения.
    Посмотреть какие еще значения могут принимать числа типа double, кроме числовых и написать тест с их использованием на все коэффициенты. solve должен выбрасывать исключение.
    Написать минимальную реализацию функции solve, которая удовлетворяет тесту из п.13.
    Сделать merge request/pull request и ссылку на него указать при сдаче ДЗ.


## Критерии оценки:

    ДЗ сдана на проверку. 1 балл
    Настроен CI. 1 балл.
    Тест, который проверяет, что для уравнения x^2+1 = 0 корней нет, успешно выполняется. 1 балл.
    Тест, который проверяет, что для уравнения x^2-1 = 0 есть два корня кратности 1, успешно выполняется. 1 балл.
    Тест, который проверяет, что для уравнения есть один корень кратности 2, успешно выполняется.
    1 балл, если дискриминант ровно равен 0,
    2 балла, если дискриминант не ноль, но меньше заданного epsilon.
    Тест, который проверяет, что коэффициент a не может быть равен 0, с учетом, что a - число с плавающей точкой, успешно выполняется. 1 балл.
    Тест, который проверяет, что solve не может принимать значения, отличные от чиcел, успешно выполняется.
    1 балл, если хотя бы один случай рассмотрен,
    2 балла - учтены все случаи.
    Оформлен merge/pull request. 1 балл
    Итого: 10 баллов.
    Задание будет принято, если набрано не менее 8 баллов.


# Конфигурирование:
pip install parameterized

