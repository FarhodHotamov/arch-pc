---
## Front matter
title: "Отчёт по лабораторной работе 2"
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

Целью работы является изучить идеологию и применение средств контроля версий. Приобрести практические навыки по работе с системой git.

# Выполнение лабораторной работы

Прежде чем начать работать с репозиторием, мне нужно настроить Git на своем компьютере. Для этого я создаю своего пользователя в системе Git и задаю параметры, такие как имя и email, чтобы мои действия были правильно подписаны.

![настроил Git](image/01.png){ #fig:001 width=70%, height=70% }

После этого генерирую SSH-ключи. Они нужны, чтобы GitHub мог меня идентифицировать при взаимодействии с репозиториями. Сохраняю их на своем компьютере и добавляю публичный ключ в свой профиль на GitHub, чтобы наладить связь.

![SSH-ключ](image/02.png){ #fig:002 width=70%, height=70% }

![импорт SSH-ключа](image/03.png){ #fig:003 width=70%, height=70% }

Затем нахожу репозиторий-шаблон, который соответствует моим задачам, и делаю из него копию, чтобы работать со своим проектом.

![Создаю репозиторий из шаблона](image/04.png){ #fig:004 width=70%, height=70% }

Теперь создаю рабочую директорию на компьютере, где буду хранить файлы проекта. В этой директории клонирую репозиторий с GitHub, чтобы можно было работать с файлами локально. 

![Клонирование репозитория](image/05.png){ #fig:005 width=70%, height=70% }

![Создание папок для курса](image/06.png){ #fig:006 width=70%, height=70% }

Когда структура готова, я добавляю все изменения в локальный репозиторий, а затем отправляю их на GitHub с помощью команды push.

![Отправка на гитхаб](image/07.png){ #fig:007 width=70%, height=70% } 

Загружаю отчёты по выполненным работам в соответствующие папки на GitHub, обновляя репозиторий по мере необходимости.

![Отправка на гитхаб](image/08.png){ #fig:008 width=70%, height=70% } 

![Проверяю репозиторий](image/09.png){ #fig:009 width=70%, height=70% } 

# Выводы

В ходе выполнения работы изучили работу с GitHub.