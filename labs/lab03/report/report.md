---
## Front matter
title: "Отчёт по лабораторной работе 3"
subtitle: "Архитектура компьютеров"
author: "Рамиэль Сарханов"

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

## Знакомство с Markdown

Установили программы pandoc и TexLive по указаниям в лабораторной работе. 

Открываю терминал, перехожу в каталог курса сформированный при выполнении лабораторной работы №3:
Обновляю локальный репозиторий, скачав изменения из удаленного репозитория.

Перехожу в каталог с шаблоном отчета по лабораторной работе № 3

Провожу компиляцию шаблона с использованием Makefile. 
Для этого ввожу команду make.
При успешной компиляции должны сгенерироваться файлы report.pdf и
report.docx. Открою их и проверю корректность полученных файлов. (рис. [-@fig:001], [-@fig:002], [-@fig:003])

![Компиляция файлов](image/01.png){ #fig:001 width=70%, height=70% }

![Просмотр docx файла](image/02.png){ #fig:002 width=70%, height=70% }

![Просмотр pdf файла](image/03.png){ #fig:003 width=70%, height=70% }

Удаляю полученный файлы с использованием Makefile. Для этого ввожу команду make clean
Проверю, что после этой команды файлы report.pdf и report.docx были удалены. (рис. [-@fig:004])

![Удаление файлов docx и pdf](image/04.png){ #fig:004 width=70%, height=70% }

Открою файл report.md c помощью любого текстового редактора, например gedit
Внимательно изучаю структуру этого файла. (рис. [-@fig:005])

![Изучаю шаблон отчета](image/05.png){ #fig:005 width=70%, height=70% }

Заполняю отчет и компилирую его с использованием Makefile. 
Проверяю корректность полученных файлов. (рис. [-@fig:006])

![Заполняю свой отчет](image/06.png){ #fig:006 width=70%, height=70% }

Загружаю файлы на Github.

## Выполнение заданий для самостоятельной работы.

Подготовил отчет по лабораторной №2 и разместил его в репозитории.
(рис. [-@fig:007], [-@fig:008])

![Заполняю отчет по лабораторной №2](image/07.png){ #fig:007 width=70%, height=70% }

![Компилирую отчет по лабораторной №2](image/08.png){ #fig:008 width=70%, height=70% }

# Выводы

При выполнении данной лабораторной работы я изучил синтаксис языка 
разметки Markdown, получил отчет из шаблона при помощи Makefile. 

