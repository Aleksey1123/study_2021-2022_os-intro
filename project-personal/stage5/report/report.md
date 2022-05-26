---
## Front matter
title: "Отчёт к индивидуальному проекту №5"
subtitle: "Добавить с сайту все остальные элементы."
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

Добавить с сайту все остальные элементы.

# Задание

-Сделать записи для персональных проектов.
-Сделать пост по прошедшей неделе.
-Добавить пост на тему по выбору.
-Языки научного программирования.

# Ход работы

1. Создали localhost с помощью команды hugo serve.

2. Открыли файл  проекта index.md и написали краткое описание проекта, а также изменили иконку твиттера на иконку гитхаба(рис. 1-2).

![Файл index.md](image/1.png)

![Вид поста на главной странице](image/2.png)

3. Создали папку "4" и файл index.md в ней в папке post. Открыли файл index.md и создали пост на тему Научные языки программирования.(рис. 3-6).

![Добавление данных в index.md](image/3.png)

![Вид поста на главной странице](image/4.png)

![Сам пост(1)](image/5.png)

![Сам пост(2)](image/6.png)

4. Отправили данные на сервер и забилдили сайт(рис. 7).

![Билд и отправка на сервер](image/7.png)

# Выводы

Мы добавили к сайту все остальные элементы.