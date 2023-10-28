---
## Front matter
title: "Отчёта по лабораторной работе 3"
subtitle: "дисциплина: Архитектура вычислительных систем"
author: "Тураева Аиша НБИбд-03-23"

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

Установили программы pandoc и TexLive по указаниям в лабораторной работе. 

Провожу компиляцию шаблона с использованием Makefile. 
Для этого использую команду make.
При успешной компиляции должны сгенерироваться файлы report.pdf и
report.docx. 

![Make шаблона](image/01.png){ #fig:001 width=70%, height=70% }

![файл в docx](image/02.png){ #fig:002 width=70%, height=70% }

![файл в pdf](image/03.png){ #fig:003 width=70%, height=70% }

Удаляю полученные файлы с использованием Makefile. Для этого ввожу команду make clean
Проверю, что после этой команды файлы report.pdf и report.docx были удалены.

![Удалены docx и pdf](image/04.png){ #fig:004 width=70%, height=70% }

Открою файл report.md c помощью текстового редактора. 
Внимательно изучите структуру этого файла.

![Шаблон отчета](image/05.png){ #fig:005 width=70%, height=70% }

Заполняю отчет и скомпилирую его с использованием Makefile. 
Проверю корректность полученных файлов.

![Отчет](image/06.png){ #fig:006 width=70%, height=70% }

Таже создаю отчет для лабораторной номер 2.

![Отчет](image/07.png){ #fig:007 width=70%, height=70% }

Загружаю на гитхаб.

![Отчет](image/08.png){ #fig:008 width=70%, height=70% }

# Выводы

Изучили синтаксис языка разметки Markdown, получили отчет из шаблона при помощи Makefile. 
