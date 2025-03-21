---
## Front matter
title: "Отчет по 2-му этапу проекта"
subtitle: "Сайт научного работника"
author: "Козина Дарья Александровна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Добавить к сайту данные о себе, сделать пост о прошедшей неделе и на тему по выбору.

# Выполнение работы

Добавим на сайт свою фотографию, напишем свои имя и фамилию (рис. [-@fig:001], рис. [-@fig:002]).

![Изменение файла](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/1.png){#fig:001 width=70%}

![Результат на сайте](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/2.png){#fig:002 width=70%}

Добавим информацию о своей роли (работник, студент и т.д.) (рис. [-@fig:003], рис. [-@fig:004]).

![Изменение файла](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/3.png){#fig:003 width=70%}

![Результат на сайте](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/4.png){#fig:004 width=70%}

Добавим свои интересы и свое образование (рис. [-@fig:005], рис. [-@fig:006]).

![Изменение файла](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/5.png){#fig:005 width=70%}

![Результат на сайте](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/6.png){#fig:006 width=70%}

Добавим краткое описание себя (рис. [-@fig:007], рис. [-@fig:008]).

![Изменение файла](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/7.png){#fig:007 width=70%}

![Результат на сайте](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/8.png){#fig:008 width=70%}

Напишем пост о прошедшей неделе (рис. [-@fig:009], рис. [-@fig:010]).

![Изменение файла](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/9.png){#fig:009 width=70%}

![Результат на сайте](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/10.png){#fig:010 width=70%}

Напишем пост на тему по выбору, я выбрала тему "Непрерывная интеграция и непрерывное развертывание (CI/CD)" (рис. [-@fig:011], рис. [-@fig:012]).

![Изменение файла](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/11.png){#fig:011 width=70%}

![Результат на сайте](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/project-personal/stage2/report/image/12.png){#fig:012 width=70%}

# Выводы

Добавили к сайту данные о себе, сделали пост о прошедшей неделе и на тему по выбору.


