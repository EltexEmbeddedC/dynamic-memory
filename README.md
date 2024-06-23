# Структуры

## Сборка и запуск

1. Необходимо перейти в корневую директорию и выполнить команду для сборки проекта

```
make
```

2. Исполняемый файл появятся в папке ```bin```

3. Для удаления объектных и исполняемых файлов необходимо выполнить команду

```
make clean
```

## Задание

Написать программу абонентский справочник. Список абонентов представляет собой статический массив (100 элементов) из структур следующего в вида:

```c
struct abonent {
    char name[10];
    char second_name[10];
    char tel[10];
};
```

При запуске на экран выводится текстовое меню:

```
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
```

Пользователю предлагается ввести пункт меня с клавиатуры. Добавление абонента в массив реализуется простым заполнением свободной структуры, при выходе за 100 абонентов уведомить пользователя о переполнении справочника и не позволять больше добавлять абонентов. При удалении структура заполняется нулями. При поиске пользователь вводит с клавиатуры имя абонентов и на экран выводится список всех абонентов с таким же именем. Программа продолжает выполняться пока пользователь не введет пункт 5.

## Тестирование

### Проведем тестирование основных функций программы:

```
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
1
Введите имя: abc
Введите фамилию: aaaaa
Введите номер телефона: 12345
Абонент добавлен.
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
1
Введите имя: def
Введите фамилию: bbbbbb
Введите номер телефона: 55555
Абонент добавлен.
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
1
Введите имя: ghi
Введите фамилию: cccccc
Введите номер телефона: 876543
Абонент добавлен.
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
4
Имя: abc, Фамилия: aaaaa, Телефон: 12345
Имя: def, Фамилия: bbbbbb, Телефон: 55555
Имя: ghi, Фамилия: cccccc, Телефон: 876543
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
2
Введите имя абонента для удаления: def
Абонент удален.
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
4
Имя: abc, Фамилия: aaaaa, Телефон: 12345
Имя: ghi, Фамилия: cccccc, Телефон: 876543
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
1
Введите имя: jkl
Введите фамилию: ggg
Введите номер телефона: 5432
Абонент добавлен.
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
4
Имя: abc, Фамилия: aaaaa, Телефон: 12345
Имя: jkl, Фамилия: ggg, Телефон: 5432
Имя: ghi, Фамилия: cccccc, Телефон: 876543
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
1
Введите имя: abc
Введите фамилию: csvr
Введите номер телефона: 456
Абонент добавлен.
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
4
Имя: abc, Фамилия: aaaaa, Телефон: 12345
Имя: jkl, Фамилия: ggg, Телефон: 5432
Имя: ghi, Фамилия: cccccc, Телефон: 876543
Имя: abc, Фамилия: csvr, Телефон: 456
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
3
Введите имя для поиска: abc
Имя: abc, Фамилия: aaaaa, Телефон: 12345
Имя: abc, Фамилия: csvr, Телефон: 456
1) Добавить абонента
2) Удалить абонента
3) Поиск абонентов по имени
4) Вывод всех записей
5) Выход
5
Выходим...
```
