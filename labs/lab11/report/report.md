---
## Front matter
title: "Лабораторная работа №11"
subtitle: "Программирование в командном процессоре OC UNIX. Ветвления и циклы"
author: "Рытов Алексей Константинович НФИбд-02-21"
lang: ru-RU


## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc-depth: 2
lof: true # List of figures
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text

---

# Цель работы

Изучить основы программирования в оболочке ОС UNIX. Научится писать более
сложные командные файлы с использованием логических управляющих конструкций
и циклов.

# Выполнение лабораторной работы

1. Используя команды getopts grep, написали командный файл, который анализирует
командную строку с ключами:

– -iinputfile — прочитать данные из указанного файла;

– -ooutputfile — вывести данные в указанный файл;

– -pшаблон — указать шаблон для поиска;

– -C — различать большие и малые буквы;

– -n — выдавать номера строк.

а затем ищет в указанном файле нужные строки, определяемые ключом -p. Затем написали текстовый файл для проверки скрипта(рис 1-4).

![Скрипт 1.sh](image/1.png)

![Текстовый файл 1.txt](image/2.png)

![Запуск скрипта](image/3.png)

![Файл 1.txt после отработки скрипта](image/4.png)

2. Написали на языке Си программу, которая вводит число и определяет, является ли оно больше нуля, меньше нуля или равно нулю. Затем программа завершается с помощью
функции exit(n), передавая информацию в о коде завершения в оболочку. Командный файл должен вызывать эту программу и, проанализировав с помощью команды $?, выдать сообщение о том, какое число было введено(рис. 5-7).

![Программа 2.cpp на языке Си++](image/5.png)

![Скрипт 2.sh](image/6.png)

![Вывод скрипта](image/7.png)

3. Написали командный файл, создающий указанное число файлов, пронумерованных
последовательно от 1 до N. Число файлов,
которые необходимо создать, передаётся в аргументы командной строки. Этот же командный файл должен уметь удалять все созданные им файлы (если они существуют)(рис. 8-10).

![Скрипт 3.sh](image/8.png)

![Запуск скрипта](image/9.png)

![Результат отработки скрипта](image/10.png)

4. Написали командный файл, который с помощью команды tar запаковывает в архив
все файлы в указанной директории. Модифицировать его так, чтобы запаковывались
только те файлы, которые были изменены менее недели тому назад(рис. 11-13).

![Скрипт 4.sh](image/11.png)

![Запуск скрипта](image/12.png)

![Результат отработки скрипта](image/10.png)

# Выводы

Мы изучили основы программирования в оболочке ОС UNIX. Научились писать более
сложные командные файлы с использованием логических управляющих конструкций
и циклов.

# Ответы на контрольные вопросы:

1. Каково предназначение команды getopts?

даёт возможность работать с флагами, которые вводятся при запуске скрипта в консоль

2. Какое отношение метасимволы имеют к генерации имён файлов?

они помогают

3. Какие операторы управления действиями вы знаете?

if, case, while, for

4. Какие операторы используются для прерывания цикла?

continue; break

5. Для чего нужны команды false и true?

true,: - всегда возвращает 0 в качестве кода выхода.
false - всегда возвращает 1 в качестве кода выхода.

6. Что означает строка if test -f man$s/$i.$s, встреченная в командном файле?

проверка существования файла 

7. Объясните различия между конструкциями while и until.