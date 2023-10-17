---
## Front matter
title: "Шаблон отчёта по лабораторной работе"
subtitle: "2"
author: "Разанацуа Сара Естэлл , НКАбд-05-23"

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

- Целью работы является изучить идеологию и применение средств контроля версий.
Приобрести практические навыки по работе с системой git.

# Задание

а. Настройка GitHub.
б. Базовая настройка git.
в. Создание SSH ключа.
г. Создание рабочего пространства.
д. Сознание репозитория курса на основе шаблона.
е. Настройка каталога курса.

# Выполнение лабораторной работы

а. Настройка GitHub.
Создаю учётную запись на сайте GitHub и заполнила основные данные учётной записи.

б. Базовая настройка git.
Открываю терминал и ввожу следующие команды, указав имя и gmail владельца
репозитория:

Настраиваю utf-8 в выводе сообщений git и задаю имя начальной ветки (будем
называть её master):


в. Создание SSH ключа.
Для последующей идентификации пользователя на сервере репозиториев необходимо
сгенерировать пару ключей (приватный и открытый): ssh-keygen -C "Имя Фамилия ".
Ключи сохраняться в каталоге ~/.ssh/.

Далее необходимо загрузить сгнетённый открытый ключ. Для этого зайти на сайт http:
//github.org/ под своей учётной записью и перейти в меню Setting . После этого выбрать
в боковом меню SSH and GPG keys и нажать кнопку New SSH key . Скопирую из
локальной консоли ключ в буфер обмена.






(рис. @fig:001).

![Название рисунка](image/placeimg_800_600_tech.jpg){#fig:001 width=70%}

# Выводы

Здесь кратко описываются итоги проделанной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::
