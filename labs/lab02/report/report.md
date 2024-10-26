---
## Front matter
title: "Отчёт по лабораторной работе 2"
subtitle: "Архитектура компьютера"
author: "Матевосян Оганес НБИбд-03-24"

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

Изучить идеологию и применение систем контроля версий, приобрести практические навыки по работе с системой Git.

# Порядок выполнения лабораторной работы

## Базовая настройка git

Сначала сделаю предварительную конфигурацию git. Открываю терминал и ввожу следующие команды, указав имя и email владельца репозитория:
(рис. [-@fig:001]) (рис. [-@fig:002])

![Базовая настройка git](image/01.jpg){ #fig:001 width=70%, height=70% }

![Базовая настройка git](image/02.jpg){ #fig:002 width=70%, height=70% }

Настраиваю utf-8 в выводе сообщений git
рис. [-@fig:003])

![Базовая настройка git](image/03.jpg){ #fig:003 width=70%, height=70% }

Задаю имя начальной ветки (будем называть её master)
рис. [-@fig:004])

![Базовая настройка git](image/04.jpg){ #fig:004 width=70%, height=70% }

Ввожу параметр autocrlf и параметр safecrlf
рис. [-@fig:005])

![Базовая настройка git](image/05.jpg){ #fig:005 width=70%, height=70% }

## Создание SSH ключа


Для последующей идентификации пользователя на сервере репозиториев необходимо сгенерировать пару ключей (приватный и открытый).
(рис. [-@fig:006]) (рис. [-@fig:007])

![Создание SSH ключа](image/06.jpg){ #fig:006 width=70%, height=70% }

![Создание SSH ключа](image/07.jpg){ #fig:007 width=70%, height=70% }

После генерации ключа, загружаю открытый ключ, скопировав из локальной консоли в буфер обмена. Вставляю ключ в появившееся на сайте поле и указываю для ключа имя (Title). 
(рис. [-@fig:008])

![Создание SSH ключа](image/08.jpg){ #fig:008 width=70%, height=70% }

## Создание рабочего пространства и репозитория курса на основе шаблона

Открываю терминал и создаю каталог для предмета «Архитектура компьютеров».
(рис. [-@fig:009])

![создаю каталог](image/09.jpg){ #fig:009 width=70%, height=70% }

Задаю имя репозитория и создаю репозиторий. Открываю терминал и захожу в каталог курса. Клонирую созданный репозиторий.
(рис. [-@fig:010]) (рис. [-@fig:011])

![Клонирую репозиторий](image/10.jpg){ #fig:010 width=70%, height=70% }

![Клонирую репозиторий](image/11.jpg){ #fig:011 width=70%, height=70% }

## Настройка каталога курса


Перехожу в каталог курса
(рис. [-@fig:012])

![Настройка каталога курса](image/12.jpg){ #fig:012 width=70%, height=70% }

Удаляю лишние файлы и создаю необходимые каталоги
(рис. [-@fig:013])

![Настройка каталога курса](image/13.jpg){ #fig:013 width=70%, height=70% }

Отправляю файлы на сервер.
(рис. [-@fig:014]) (рис. [-@fig:015])

![Отправляю файлы на сервер](image/14.jpg){ #fig:014 width=70%, height=70% }

![Отправляю файлы на сервер](image/15.jpg){ #fig:015 width=70%, height=70% }

Проверяю правильность создания иерархии рабочего пространства в локальном репозитории и на странице github

![Отправляю файлы на сервер](image/16.jpg){ #fig:016 width=70%, height=70% }

# Выводы

В ходе выполнения лабораторной работы я получил практические навыки работы с системой контроля версий Git. Я освоил основные команды, настроил рабочее пространство и репозиторий, а также успешно загрузил результаты на GitHub.
