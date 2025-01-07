---
## Front matter
title: "Отчёт по лабораторной работе 4"
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

Целью работы является освоение процедуры компиляции и сборки программ, написанных на ассемблере NASM.

# Выполнение лабораторной работы

1. Создаю каталог lab04, перехожу в него, создаю файл hello.asm.

![Файл для программы](image/01.png){ #fig:001 width=70%, height=70% }

2. Написал код программы по заданию.

![Программа hello.asm](image/02.png){ #fig:002 width=70%, height=70% }

3. Транслировал файл командой nasm. Получился объектный файл hello.o

4. Транслировал файл командой nasm с дополнительными опциями.Получился файл листинга и объектный файл.

5. Выполнил линковку и получил исполняемый файл.

6. Еще раз выполнил линковку для второго объектного файла и получил новый исполняемый файл.

7. Запустил исполняемые файлы.

![Сборка и запуск программы](image/03.png){ #fig:003 width=70%, height=70% }

8. Изменил сообщение Hello world на свое имя и запустил файл еще раз.

![Программа в файле lab4.asm](image/04.png){ #fig:004 width=70%, height=70% }

![Сборка и проверка программы lab4.asm](image/05.png){ #fig:005 width=70%, height=70% }

# Выводы

Освоили процесс компиляции и сборки программ, написанных на ассемблере nasm.