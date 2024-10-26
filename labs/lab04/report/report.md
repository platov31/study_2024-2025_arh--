---
## Front matter
title: "Отчёт по лабораторной работе 4"
subtitle: "Дисциплина: Архитектура компьютера"
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

1. Создаю каталог `lab04`, перехожу в него и создаю файл `hello.asm`, в котором будет находиться код программы.

![Файл для программы](image/01.png){ #fig:001 width=70%, height=70% }

2. Написал код программы в файле `hello.asm` в соответствии с заданием.

![Программа hello.asm](image/02.png){ #fig:002 width=70%, height=70% }

3. Транслировал файл с помощью команды `nasm`, в результате чего был получен объектный файл `hello.o`.

4. Выполнил трансляцию с использованием `nasm` и дополнительных опций, что позволило создать файл листинга и объектный файл.

5. Произвел линковку, в результате которой был получен исполняемый файл.

6. Снова выполнил линковку для второго объектного файла и создал новый исполняемый файл.

7. Запустил созданные исполняемые файлы для проверки их работоспособности.

![Сборка и запуск программы](image/03.png){ #fig:003 width=70%, height=70% }

8. Изменил сообщение "Hello, world!" на свое имя в программе и снова запустил файл, чтобы увидеть изменения.

![Программа в файле lab4.asm](image/04.png){ #fig:004 width=70%, height=70% }

![Сборка и проверка программы lab4.asm](image/05.png){ #fig:005 width=70%, height=70% }

# Выводы

Освоили процесс компиляции и сборки программ, написанных на ассемблере nasm.