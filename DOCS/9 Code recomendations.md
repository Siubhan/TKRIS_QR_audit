<!--
Разработка рекомендаций по кодированию
Ориентируясь на материал лекции 7 разработать перечень запретов, рекомендаций и требований (по 2-3) для оформления
исходных кодов проекта. Снабдить их краткими примерами. Дополнить документ кратким (5-10 пунктов) чек-листом для
проверки корректности кода. Разместить документ в репозитории GitHub.
-->

# Рекомендации по кодированию

В основе рекомендаций — руководство по оформлению кода на Python [PEP-8](https://peps.python.org/pep-0008/). Все
правила [PEP-8](https://peps.python.org/pep-0008/) должны соблюдаться в проекте. Ниже перечислены самые важные
рекомендации и требования по оформлению кода.

## Рекомендации и требования к оформлению кода

1. snake_case для всех имён, кроме констант и классов.

```python
your_name = my_var
get_name()
init.py
my_app.py
```

2. SCREAMING_SNAKE_CASE для констант.

```python
PI = 3.1415
MY_PI = 3.14
```

3. UpperCamelCase для имён классов.

```python
class MyClass


class DataFrame
```

4. Во всех именах ключевое слово должно быть существительным, за исключением имён функций и методов.

```python
name
words
best_sum
```

5. Имена функций и методов должны начинаться с глагола.

```python
get_name()
set_name()
sort()
is_number()
```

6. Функции отделяются друг от друга двумя пустыми строками.

```python
def get_name():
    pass


def set_name():
    pass

```

7. Методы отделяются друг от друга одной пустой строкой.

```python
class MyClass:
    def get_name():
        pass

    def set_name():
        pass

```

8. В выражениях не должны участвовать неименованные константы (magic numbers).

```python
side_1 = 5
side_2 = 20
square = side_1 * side_2
```

## Чек-лист для проверки корректности кода

<label><input type="checkbox">
snake_case для всех имён, кроме констант и классов.
</label><br>
<label><input type="checkbox">
SCREAMING_SNAKE_CASE для констант.
</label><br>
<label><input type="checkbox">
UpperCamelCase для имён классов.
</label><br>
<label><input type="checkbox">
Во всех именах ключевое слово — существительное, кроме функций и методов.
</label><br>
<label><input type="checkbox">
Имена функций и методов начинаются с глагола.
</label><br>
<label><input type="checkbox">
Функции отделены друг от друга двумя пустыми строками.
</label><br>
<label><input type="checkbox">
Методы отделены друг от друга одной пустой строкой.
</label><br>