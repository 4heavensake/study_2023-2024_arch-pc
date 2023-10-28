---
## Front matter
title: "Отчёт по лабораторной работе №4"
subtitle: "Создание и процесс обработки программ на языке ассемблера NASM"
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

Освоение процедуры компиляции и сборки программ, написанных на ассемблере NASM.

# Задание

Написать программу на Ассемблере с выводом "Hello World!" и своего ФИО

# Выполнение лабораторной работы

## Программа Hello World!

</p>Создайте каталог для работы с программами на языке ассемблера NASM
<p align="center">![Создание каталога](image/Снимок экрана от 2023-10-28 15-26-29.png)
</p>Перейдите в созданный каталог
<p align="center">![Переходим в созданный каталог](image/Снимок экрана от 2023-10-28 15-27-34.png)
</p>Создайте текстовый файл с именем hello.asm
<p align="center">![Создание текстового файла](image/Снимок экрана от 2023-10-28 15-28-33.png)
</p>Откройте этот файл с помощью любого текстового редактора, например, gedit
</p>и введите в него следующий текст:
<p align="center">![Открываем файл с помощью gedit и вводим программу](image/Снимок экрана от 2023-10-28 15-30-57.png)

## Транслятор NASM

</p>Преобразуем текстовый файл в объектный код
<p align="center">![Используем команду nasm](image/Снимок экрана от 2023-10-28 15-31-55.png)
</p>Проверяем правильность выполнения команды
<p align="center">![Используем команду ls](image/Снимок экрана от 2023-10-28 15-32-21.png)

## Расширенный синтаксис командной строки NASM

</p>Компилируем исходный файл
<p align="center">![Преобразуем файл hello.asm в obj.o](image/Снимок экрана от 2023-10-28 15-33-12.png)
</p>Проверяем правильность выполнения команды
<p align="center">![Используем команду ls](image/Снимок экрана от 2023-10-28 15-33-21.png)

## Компоновщик LD
</p>Передаем объектный файл на обработку компоновщику
<p align="center">![Используем команду ld](image/Снимок экрана от 2023-10-28 15-34-13.png)
</p>Проверяем создался ли исполняемый файл
<p align="center">![Используем команду ls](image/Снимок экрана от 2023-10-28 15-34-24.png)
</p>Передаем объектный файл obj.o на обработку компоновщику
<p align="center">![Используем команду ld для создания файла main](image/Снимок экрана от 2023-10-28 15-35-05.png)
</p>Проверяем правильно выполнения команды
<p align="center">![Используем команду ls](image/Снимок экрана от 2023-10-28 15-35-11.png)

## Запуск исполняемого файла

Запускаем выполняемый файл 
<p align="center">![Используем команду ./hello](image/Снимок экрана от 2023-10-28 15-35-27.png)

## Задание для самостоятельной работы

Копируем файл hello.asm
<p align="center">![Используем команду cp](image/Снимок экрана от 2023-10-28 16-26-44.png)
</p>Открываем файл и меняем Hello World на свое имя и фамилию
<p align="center">![Используем gedit и редактируем](image/Снимок экрана от 2023-10-28 15-37-30.png)
</p>Прописываем те же команды, что и с первой программой
<p align="center">![Используем команды для работы файла и запускаем программу](image/Снимок экрана от 2023-10-28 15-42-31.png)
</p>Копируем файлы в локальный репозиторий
<p align="center">![Копируем файлы в каталог lab04](image/Снимок экрана от 2023-10-28 16-30-50.png)
</p>Переходим в каталог лабораторных работ и загружаем файлы на github
<p align="center">![Загружаем файлы](image/Снимок экрана от 2023-10-28 15-45-39.png)

# Выводы

Мы освоили процедуры компиляции и сборки программ, написанных на ассемблере NASM

