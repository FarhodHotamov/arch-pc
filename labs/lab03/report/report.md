---
## Front matter
title: "Отчёт по лабораторной работе 3"
subtitle: "Архитектура компьютеров"
author: "Хотамов Фарход Хусейнович"

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

Целью работы является освоение процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Выполнение лабораторной работы

Инсталлировал приложения pandoc и TexLive, следуя инструкциям из лабораторного задания.

Переместился в директорию, созданную в ходе третьей лабораторной работы, и оттуда в папку с образцом отчёта для этой же работы.

Выполнил сборку образца, используя Makefile, путем введения команды make.

Создание PDF-файла потребовало нескольких попыток и установки дополнительных шрифтов.

![Make шаблона](image/01.png){ #fig:001 width=70%, height=70% }

После успешной сборки должны были создаться файлы report.pdf и report.docx, которые я проверил.

![файл в docx](image/02.png){ #fig:002 width=70%, height=70% }

![файл в pdf](image/03.png){ #fig:003 width=70%, height=70% }

С помощью Makefile удалил сгенерированные файлы, применив команду make clean, и убедился в их удалении.

![Удалены docx и pdf](image/04.png){ #fig:004 width=70%, height=70% }

Открыл файл report.md в текстовом редакторе, например, в gedit, и подробно ознакомился с его структурой.

![Шаблон отчета](image/05.png){ #fig:005 width=70%, height=70% }

Заполнил отчет, следуя указаниям.

![Заполним шаблон для отчета](image/06.png){ #fig:006 width=70%, height=70% }

Также подготовил отчет для второй лабораторной работы, как было указано.

![Заполним шаблон для отчета](image/07.png){ #fig:007 width=70%, height=70% } 

# Выводы

Изучили синтаксис языка разметки Markdown, получили отчет из шаблона при помощи Makefile. 