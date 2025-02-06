---
## Front matter
title: "Отчёт по лабораторной работе №2


Компьютерный практикум по статистическому анализу данных"
subtitle: "Структуры данных"
author: "Выполнил: Чичкина Ольга Константиновна , 


НПИбд-02-21, 1032217621"

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

Основная цель работы — изучить несколько структур данных, реализованных в Julia, 
научиться применять их и операции над ними для решения задач.
 
# Выполнение лабораторной работы

##  Кортежи

Кортеж (Tuple) — структура данных (контейнер) в виде неизменяемой индексируемой 
последовательности элементов какого-либо типа (элементы индексируются с единицы). 

Синтаксис определения кортежа: (element1, element2, ...). 

Примеры кортежей (рис. [-@fig:001]):

![Примеры кортежей](image/1.PNG){ #fig:001 width=100% height=100% }

Примеры операций над кортежами (рис. [-@fig:002]):

![Примеры операций над кортежами](image/2.PNG){ #fig:002 width=100% height=100% }

##  Словари

Словарь — неупорядоченный набор связанных между собой по ключу данных. 

Синтаксис определения словаря: Dict(key1 => value1, key2 => value2, ...). 

Примеры словарей и операций над ними (рис. [-@fig:003]):

![Примеры словарей и операций над ними](image/3.PNG){ #fig:003 width=100% height=100% }

## Множества

Множество, как структура данных в Julia, соответствует множеству, как математическому объекту, 
то есть является неупорядоченной совокупностью элементов какого-либо типа. 
Возможные операции над множествами: объединение, пересечение, разность; принадлежность элемента множеству.

Синтаксис определения множества: Set([itr]) где itr — набор значений, сгенерированных данным итерируемым объектом или пустое 
множество.

Примеры множеств и операций над ними (рис. [-@fig:004] - рис. [-@fig:005]):

![Примеры множеств и операций над ними](image/4.PNG){ #fig:004 width=100% height=100% }

![Примеры множеств и операций над ними](image/5.PNG){ #fig:005 width=100% height=100% }

## Массивы

Массив — коллекция упорядоченных элементов, размещённая в многомерной сетке. Векторы и матрицы являются частными случаями массивов.

Общий синтаксис одномерных массивов: array_name_1 = [element1, element2, ...], array_name_2 = [element1 element2 ...]

Примеры массивов (рис. [-@fig:006] - рис. [-@fig:007]):

![Примеры массивов](image/6.PNG){ #fig:006 width=100% height=100% }

![Примеры массивов](image/7.PNG){ #fig:007 width=100% height=100% }

Примеры массивов, заданных некоторыми функциями через включение (рис. [-@fig:008]):

![Примеры массивов, заданных некоторыми функциями через включение](image/8.PNG){ #fig:008 width=100% height=100% }

Некоторые операции для работы с массивами: (рис. [-@fig:009] - рис. [-@fig:014]):

![Некоторые операции для работы с массивами](image/9.PNG){ #fig:009 width=100% height=100% }

![Некоторые операции для работы с массивами](image/10.PNG){ #fig:010 width=100% height=100% }

![Некоторые операции для работы с массивами](image/11.PNG){ #fig:011 width=100% height=100% }

![Некоторые операции для работы с массивами](image/12.PNG){ #fig:012 width=100% height=100% }

![Некоторые операции для работы с массивами](image/13.PNG){ #fig:013 width=100% height=100% }

![Некоторые операции для работы с массивами](image/14.PNG){ #fig:014 width=100% height=100% }

## Самостоятельная работа

Выполнение заданий №1 и №2 (рис. [-@fig:015]):

![Решение заданий №1 и №2](image/15.PNG){ #fig:015 width=100% height=100% }

Выполнение задания №3 (всех подпунктов) (рис. [-@fig:016] - рис. [-@fig:020]):

![Выполнение подпунктов задания №3](image/16.PNG){ #fig:016 width=100% height=100% }

![Выполнение подпунктов задания №3](image/17.PNG){ #fig:017 width=100% height=100% }

![Выполнение подпунктов задания №3](image/18.PNG){ #fig:018 width=100% height=100% }

![Выполнение подпунктов задания №3](image/19.PNG){ #fig:019 width=100% height=100% }

![Выполнение подпунктов задания №3](image/20.PNG){ #fig:020 width=100% height=100% }

Выполнение заданий №4, №5 и №6 (рис. [-@fig:021]):

![Решение заданий №4, №5 и №6](image/15.PNG){ #fig:021 width=100% height=100% }

# Вывод

В ходе выполнения лабораторной работы были изучены несколько структур данных, реализованных в Julia, 
а также научились применять их и операции над ними для решения задач.

# Список литературы. Библиография

[1] Julia Documentation: https://docs.julialang.org/en/v1/