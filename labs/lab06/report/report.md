---
## Front matter
title: "Отчёт по лабораторной работе №6"
subtitle: "Операционные системы"
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

Приобрести практические навыки взаимодействия пользователя с системой посредством командной строки. 

# Выполнение лабораторной работы

Определим полное имя домашнего каталога. При помощи команды cd перейдем в домашний каталог и увидим, что его название совпадает с именем пользователя. Путь к домашнему каталогу покажем командой pwd (рис. [-@fig:001]).

![Домашний каталог](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/1.png){#fig:001 width=70%}

Перейдем в каталог /tmp с помощью команды cd/tmp. С помощью команды ls выведем содержимое каталога с различными опциями (рис. [-@fig:002]).

![Каталог /tmp](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2.png){#fig:002 width=70%}

С помощью опции -a мы можем увидеть содержимое каталога со скрытыми файлами (рис. [-@fig:003]).

![Опция -a](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/3.png){#fig:003 width=70%}

С помощью опции -f мы сожем увидеть файлы списком (рис. [-@fig:004]).

![Опция -f](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/4.png){#fig:004 width=70%}

С помощью опции -l мы можем увидеть подробное содержимое каталога (рис. [-@fig:005]).

![Опция -l](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/5.png){#fig:005 width=70%}

Перейдем в каталог /var/spool с помощью команды cd. Командой ls проверим наличие каталога cron. Такого каталога нет (рис. [-@fig:006]).

![Каталог /var/spool](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/6.png){#fig:006 width=70%}

Перейдем в домашний каталог, выведем его содержимое, с помощью опции -al определим, кто является владельцем файлов и подкаталогов (рис. [-@fig:007], рис. [-@fig:008]).

![Домашний каталог](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/7.png){#fig:007 width=70%}

![Владелец](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/8.png){#fig:008 width=70%}

В домашнем каталоге создадим каталог newdir. В созданном каталоге создадим новый каталог morefun, одной командой в домашнем каталоге создадим каталоги letters, memos, misk. Командой ls проверим (рис. [-@fig:009]).

![Создание каталогов](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/9.png){#fig:009 width=70%}

Удалим ранее созданные каталоги. Проверим удалились ли каталоги командой ls (рис. [-@fig:010], рис. [-@fig:011]).

![Удаление каталога](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/10.png){#fig:010 width=70%}

![Удаление каталога](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/11.png){#fig:011 width=70%}

С помощью команды man определим использование опций для просмотра не только каталога, но и подкаталога, входящего в него. Также определим опцию, для отсортировки по времени последнего изменения выводимый список содержимого каталога с развернутым описанием файлов (рис. [-@fig:012], рис. [-@fig:013]).

![Команда man](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/12.png){#fig:012 width=70%}

![Опции](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/13.png){#fig:013 width=70%}

С помощью команды man посмотрим описание команд: cd, pwd, mkdir, rmdir, rm (рис. [-@fig:014], рис. [-@fig:015], рис. [-@fig:016], рис. [-@fig:017], рис. [-@fig:018]).

![Описание команды cd](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/14.png){#fig:014 width=70%}

![Описание команды pwd](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/15.png){#fig:015 width=70%}

![Описание команды mkdir](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/16.png){#fig:016 width=70%}

![Описание команды rmdir](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/17.png){#fig:017 width=70%}

![Описание команды rm](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/18.png){#fig:018 width=70%}

Используя информацию, полученную при помощи команды history, выполним модификацию и исполнение нескольких команд из буфера команд (рис. [-@fig:019]).

![Команда history](/home/dakozina/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/19.png){#fig:019 width=70%}

# Выводы

Мы приобрели практические навыки взаимодействия пользователя с системой посредством командной строки

