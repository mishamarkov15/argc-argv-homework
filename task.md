# Задание 1. Утилита cat
Нужно реализовать утилиту, с помощью которой можно просмотреть содержимое файла. Сама утилита имеет набор параметров, которые необходимо поддержать.

Параметры:
- `-n` - вывести только первые `n` строк в файле.
- `-l` - вывести только последние `l` строк в файле.

Использование:
`cat [-n num | -l num] file`

Все параметры, кроме `file`, опциональны. Поведения утилиты без параметров -- просто вывод содержимого файла `file` на экран.

Параметры `-n` и `-l` взаимозаменяемы. Указать можно либо только `-n`, либо только `-l`, либо вообще их не указывать.

Примеры работы:

<details>
<summary>Без доп. аргументов</summary>

```text
   $cat input.txt
   hello, world!
   Today is Good day.
   
   I'm unbelievable super-man.
   Today is Thursday.
   Ultra gucci cat!
   8 999-222-39-22
```

</details>

<details>
<summary>С параметром -n</summary>

```text
   $cat -n 4 input.txt
   hello, world!
   Today is Good day.
   
   I'm unbelievable super-man.
```

</details>

<details>
<summary>С параметром -l</summary>

```text
   $cat -l 2 input.txt
   Ultra gucci cat!
   8 999-222-39-22
```

</details>