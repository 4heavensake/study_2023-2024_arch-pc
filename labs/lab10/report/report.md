---
## Front matter
title: "Отчёт по лабораторной работе №10"
subtitle: "Работа с файлами средствами Nasm."
author: "Югай Александр Витальевич"

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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Приобрести навыки написания программ для работы с файлам, научиться управлять доступом к 
файлам.


# Выполнение лабораторной работы

Создаем каталог для программ ЛБ10, и в нем создаем файлы
<p align="center">![Создаем каталог с помощью команды mkdir и файлы с помощью команды touch](image/Снимок экрана от 2023-12-14 20-40-05.png)
<p>Открываем файл в Midnight Commander и заполняем его в соответствии с листингом 10.1 
<p align="center">![Заполняем файл](image/Снимок экрана от 2023-12-14 20-41-43.png)
<p>Создаем исполняемый файл и запускаем его 
<p align="center">![Запускаем файл и проверяем его работу](image/Снимок экрана от 2023-12-14 21-00-23.png)
<p>Изменяем права доступа к файлу, запретив его выполнение. Пробуем запустить файл
<p align="center">![Используем команду chmod для установки нужных прав, после этого пытаемся запустить файл](image/Снимок экрана от 2023-12-14 20-46-44.png)
<p>Выдало: отказано в доступе. Значит мы поставили правильный запрет на выполнение.
<p>Изменяем права доступа к файлу с исходным текстом программы, добавив права на исполнение. 
<p>Пробуем запустить файл
<p align="center">![Используем команду chmod для установки нужных прав, после этого пытаемся запустить файл](image/Снимок экрана от 2023-12-14 20-48-29.png)
<p>lab10-1.asm является файлом с исходным кодом программы на языке ассемблера, искусственно 
добавление права на исполнение не даст ожидаемого результата. Такие файлы нужно 
компилировать или ассемблировать в машинный код, а затем выполнять.
<p>Вариант-3
<p>Предоставляем права доступа к 2ум файлам, согласно варианту 20 в символьном и двоичном виде, 
затем проверяем работу команд.
<p align="center">![Используем команду chmod для установки нужных прав, после этого проверяем правильность выполнения командой ls -l](image/Снимок экрана от 2023-12-14 20-56-01.png)

## Задание для самостоятельной работы

Создаем новый файл
<p align="center">![Создаем файл командой touch](image/Снимок экрана от 2023-12-14 20-56-18.png)
<p>Пишем программу, которая выполнит представленный список действий
<p align="center">![Пишем программу в nano](image/Снимок экрана от 2023-12-14 20-58-08.png)
<p>Создаем исполняевый файл и запускаем его, после этого проверяем создался ли новый файл, затем 
смотрим, как он заполнен
<p align="center">![Проверяем работу программы](image/Снимок экрана от 2023-12-14 21-01-49.png)

# Выводы

Мы научились писать программы для работы с файлам и научились предоставлять права доступа к 
файлам.

