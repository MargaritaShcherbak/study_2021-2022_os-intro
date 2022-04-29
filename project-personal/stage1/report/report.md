---
## Front matter
title: "Отчёт по первому этапу реализации проекта"
subtitle: "Размещение на Github pages заготовки для персонального сайта."
author: "Щербак Маргарита Романовна"

## Generic otions
lang: ru-RU


## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
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

# **Размещение на Github pages заготовки для персонального сайта.** 

## **Цель работы**
Создать заготовку для персонального сайта научного работника.

## **Ход работы**

1. Установили необходимое программное обеспечение. 
Устанавливаемая в системе версия hugo меньше необходимой,поэтому следует установить программу вручную. 
Cкачали архив с репозитория, далее распаковали его. https://github.com/gohugoio/hugo/releases
(Рис. [-@fig:001])

![Установка ПО](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-04-29%2021-45-05.png){#fig:001 width=70%}

2. Скачали шаблон темы сайта. И клонировали его. (Рис. [-@fig:002] - Рис. [-@fig:003])

![Создаём репозиторий с темой сайта по шаблону](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202022-04-29%20214658.png){#fig:002 width=70%}   

![Клонируем шаблон темы сайта](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202022-04-29%20221434.png){#fig:003 width=70%}

3. Выполняем необходимые команды и получаем ссылку на шаблон сайта.Переходим по этой ссылке. (Рис .[-@fig:004] - Рис .[-@fig:005])

![Ссылка на шаблон сайта](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202022-04-29%20222605.png){#fig:004 width=70%}

![Шаблон сайта](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202022-04-29%20222443.png){#fig:005 width=70%}

4. Удалили зелёное предупреждение, чтобы сайт видели не только мы, но и другие пользователи (сontent/home/demo.md) и получили белый фон сайта.(Рис. [-@fig:006]) 

![Смена фона сайта. Удаление предупреждения](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202022-04-29%20223757.png){#fig:006 width=70%}

5. Разместили сайт на хостинге git. Cоздали ещё один репозиторий. (Рис .[-@fig:007] - Рис .[-@fig:008])

![Создание репозитория](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202022-04-29%20224930.png){#fig:007 width=70%}

![Выполнение команд](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202022-04-29%20225222%20(%D0%BA%D0%BE%D0%BF%D0%B8%D1%8F).png){#fig:008 width=70%}

6. Привязали к каталогу public наш репозиторий. Синхронизируем файлы с репозиторием. (Рис .[-@fig:009])

![Убеждаемся, что каталог подключён к репозиторию](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202022-04-29%20230702.png){#fig:009 width=70%}

7. Проверяем правильность выполненных действий. Обновляем репозиторий. Видим, что добавились файлы. 
Скопировали ссылку на наш новый сайт и перешли по ней. (Рис .[-@fig:0010] - Рис .[-@fig:0011])

![Обновили репозиторий. Добавились файлы](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-04-29%2023-10-49.png){#fig:0010 width=70%}

![Заготовка сайта готова!](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-04-29%2023-11-33.png){#fig:0011 width=70%}

## **Вывод:** 

Таким образом, я создала заготовку для персонального сайта научного работника.