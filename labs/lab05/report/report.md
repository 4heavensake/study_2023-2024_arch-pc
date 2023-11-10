---
## Front matter
title: "Отчет по лабораторной работе №5"
subtitle: "Основы работы с Midnight Commander (mc)"
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

Приобретение практических навыков работы в Midnight Commander. Освоение инструкций
языка ассемблера mov и int.

# Задание

Написать 2 программы по примеру и внести изменения по их условию 

# Выполнение лабораторной работы

## Порядок выполнения лабораторной работы

Откройте Midnight Commander
<p align="center">![Открываем mc](image/Снимок экрана от 2023-11-11 00-16-44.png)
<p>Переходим в каталог, созданный при выполнении 4 лабораторной работы 
<p align="center">![Переходим в каталог](image/Снимок экрана от 2023-11-11 00-18-26.png)
<p>Создаем каталог lab05
<p align="center">![Создаем каталог функциональной клавишей F7](image/Снимок экрана от 2023-11-11 00-20-58.png)
<p>Создаем файл lab5-1.asm
<p align="center">![Создаем файл командой touch](image/Снимок экрана от 2023-11-11 00-21-02.png)
<p>Открываем файл для редактирования и заполняем его по листингу
<p align="center">![Открываем файл функциональной клавишей, заполняем и сохраняем](image/Снимок экрана от 2023-11-11 00-26-00.png)
<p>Открываем файл для просмотра
<p align="center">![Просматриваем файл для проверки](image/Снимок экрана от 2023-11-11 00-26-32.png)
<p>Транслируем текст программы и запускаем исполняемый файл
<p align="center">![Проверяем как работает программа](image/Снимок экрана от 2023-11-11 00-28-28.png)
<p>Скачиваем файл с туиса
<p align="center">![Скачиваем файл](image/Снимок экрана от 2023-11-11 00-29-50.png)
<p>Копируем в нужную директорию
<p align="center">![Копируем скаченный файл](image/Снимок экрана от 2023-11-11 00-32-05.png)
<p>Создаем копию файла lab5-1.asm и проверяем
<p align="center">![Создаем копию файла и проверяем](image/Снимок экрана от 2023-11-11 00-33-32.png)
<p>Открываем файл и заполняем в соответствии с листингом 
<p align="center">![Заполняем файл](image/Снимок экрана от 2023-11-11 00-38-03.png)
<p>Транслируем и запускаем файл
<p align="center">![Проверяем работу программы](image/Снимок экрана от 2023-11-11 00-41-04.png)
<p>Снова открываем файл и меняем sprintLF на sprint
<p align="center">![Редактируем файл](image/Снимок экрана от 2023-11-11 00-41-58.png)
<p>Транслируем файл и запускаем
<p align="center">![Проверяем работу файла и сравниваем с прошлой](image/Снимок экрана от 2023-11-11 00-42-51.png)
<p>Замечаем, что sprint выводит текст в той же строке, а spintLF, выводит с новой

### Задание для самостоятельной работы
<p>Создаем копию файла lab5-1.asm и называем его также
<p align="center">![Создаем копию файла lab5-1.asm](image/Снимок экрана от 2023-11-11 01-24-02.png)
<p>Редактируем файл, чтобы введенный текст выводился в консоль
<p align="center">![Редактируем файл](image/Снимок экрана от 2023-11-11 00-53-03.png)
<p>Транслируем файл и запускаем программу
<p align="center">![Проверяем правильность написания программы](image/Снимок экрана от 2023-11-11 00-54-05.png)
<p>Создаем копию файла lab5-2.asm и называем его также
<p align="center">![Создаем копию файла lab5-2.asm](image/Снимок экрана от 2023-11-11 00-54-51.png)
<p>Редактируем файл, чтобы введенный текст, выводился в консоль
<p align="center">![Редактируем файл](image/Снимок экрана от 2023-11-11 00-58-27.png)
<p>Транслируем файл и запускаем программу
<p align="center">![Проверяем правильность написания программы](image/Снимок экрана от 2023-11-11 00-59-14.png)

# Выводы

Мы приобрели навыки работы с Midnight Commander и освоили инструкции mov и int


