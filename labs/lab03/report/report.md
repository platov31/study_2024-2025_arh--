---
## Front matter
title: "Отчёт по лабораторной работе №3"
subtitle: "*Дисциплина: Архитектура компьютера*"
author: "Богачев Егор Михайлович НММбд-01-24"

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

Целью работы является освоение процедуры оформления отчетов с помощью легковесного
языка разметки Markdown.

# Задание

1) Техническое обеспечение
2) Установка необходимого ПО
3) Заполнение и компиляция отчёта по лабораторной работе №3
4) Задание для самостоятельной работы

# Выполнение лабораторной работы

1. Открываю терминал.Перехожу в каталог курса сформированный при выполнении лабораторной работы
№2. 

![переход в каталог](image/переход_в_каталог.png){#fig:001 width=70%}

2. Обновляю локальный репозиторий, скачав изменения из удаленного репозитория с помо-
щью команды git pull 

![git pull](image/git_pull.png){#fig:002 width=70%} 

3. Перехожу в каталог с шаблоном отчета по лабораторной работе № 3 

![переход](image/переход.png){#fig:003 width=70%} 

4. Провожу компиляцию шаблона с использованием Makefile. Для этого ввожу команду make. 

![make](image/make.png){#fig:004 width=70%} 

5. После успешной компиляции сгенерировались файлы report.pdf и report.docx.
Открываю и проверяю корректность полученных файлов.

![сгенерированные файлы](image/сгенерированные_файлы.png){#fig:005 width=70%} 

6. Удаляю полученные файлы с использованием Makefile. Для этого ввожу команду make clean.
Проверяю, что после этой команды файлы report.pdf и report.docx были удалены. 

![make clean](image/make_clean.png){#fig:006 width=70%} 

7. Открываю файл report.md c помощью текстового редактора gedit. 

![gedit](image/gedit.png){#fig:007 width=70%} 

8. Загружаю файлы на Github.

![файлы на Git](image/файлы_на_Git.png){#fig:008 width=70%} 


# Выводы

Я освоил процедуры оформления отчетов с помощью легковесного
языка разметки Markdown.


