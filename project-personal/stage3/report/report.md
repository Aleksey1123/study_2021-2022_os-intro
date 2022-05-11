---
## Front matter
title: "Отчёт к индивидуальному проекту №3"
subtitle: "Добавить к сайту достижения."
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

Добавить к сайту достижения.

# Задание

Список достижений.</br>
-Добавить информацию о навыках (Skills).</br>
-Добавить информацию об опыте (Experience).</br>
-Добавить информацию о достижениях (Accomplishments).</br>
-Сделать пост по прошедшей неделе.</br>
-Добавить пост на тему по выбору:</br>
1) Легковесные языки разметки.</br>
2) Языки разметки. LaTeX.</br>
3) Язык разметки Markdown.

# Ход работы

1. Создали localhost с помощью команды hugo serve(рис. 1).

![Создание localhost](image/1.png)

2. Загрузили иконки для нашего сайта из интернета и закинули их в папку icons(рис. 2).

![Папка icons](image/2.png)

3. Открыли файл skills.md и добавили свои данные(рис. 3-4).

![Файл skills.md](image/3.png)

![Раздел навыки после изменения](image/4.png)

4. Открыли файл experience.md и добавили свои данные(рис. 5-6).

![Файл experience.md](image/5.png)

![Раздел опыт после изменения](image/6.png)

5. Открыли файл accomplishments.md и добавили свои данные(рис. 7-8).

![Файл accomplishments.md](image/7.png)

![Раздел достижения после изменения](image/8.png)

6. Создали папку "2" и файл index.md в ней в папке post. Открыли файл index.md и создали пост на тему Язык разметки Markdown(рис. 9-11).

![Добавление данных в index.md](image/9.png)

![Вид поста на главной странице](image/10.png)

![Сам пост](image/11.png)

7. Отправили данные на сервер и забилдили сайт(рис. 12).

![Билд и отправка на сервер](image/12.png)

# Выводы

Мы добавили к сайту свои достижения, а также написали пост на тему 'Язык разметки Markdown'.