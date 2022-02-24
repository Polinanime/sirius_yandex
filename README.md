# Уроки Настоящего цикл №6

Все решения написаны инвалидно и грязно, за что заранее прошу прощения.  
Решения для каждого задания хранятся в соответствующих директориях, а сами задания в файлах `TASK.md`

## Задание 1. Исправить опечатки

### Решения

#### Решение первое (first_solution.py)

По расстоянию Левинштейна сравнивал каждую возможную пару слов, ничего особенного - **91.5 баллов** (из 100)

#### Решение второе (second_solution.py)

В первом решении пришлось написать алгоритм для последовательного исправления ошибок в слове, чтобы получить нужное.
Поэтому решил сравнивать каждую пару слов именно по этой функции вместо Левинштейна - итого **96.97**.

### Комментарий

Больше по этой таске ничего не делал. Возможно, если немного улучшить функцию исправления, то больше баллов будет

## Задание 2. Нормализация названий университетов

### Решения

#### Решение первое (first_solution.py)

Банально по Левинштейну сравнивал и зашло на ура, а именно 94 балла

#### Решение второе (second_solution.py)

Тут жесть какую-то придумал:

* создаем *алфавит* из всех уникальных слов в названиях университетов
* преобразуем весь словарь в векторы (математические) на основе этого самого алфавита
* идем по запросам (входные данные), разбиваем на слова и для каждого ищем ближайшее из алфавита
* преобразуем на основе прошлого пункта в векторы каждый запрос
* рассматриваем каждую возможную пару векторов **запрос - верное название** и по косинусу ищем самое близкое верное
  название

Казалось бы, гениально и вообще прекрасно, но 96.85 баллов(

### Комментарий
Тут абсолютно хз, что можно улучшить. Чувство, будто все с нуля надо писать