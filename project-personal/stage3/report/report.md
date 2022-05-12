---
## Front matter
title: "Отчёт по третьему этапу реализации проекта"
subtitle: "Добавить к сайту достижения"
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
Добавить к сайту: информацию о навыках (Skills),опыте (Experience) и  достижениях (Accomplishments).  
Сделать пост по прошедшей неделе.  
Добавить пост на тему "Язык разметки Markdown".

## **Теоретическое введение**

Для реализации сайта используется генератор статических сайтов Hugo.  
Исходя из действий во втором этапе, внесли изменения в файлы skills.md, experience.md, accomplishments.md. Выбрали понравившиеся иконки и эмоджи. Написали два поста с картинками. Загрузили на хостинг Git.

## **Ход работы**

1. Перешли в ~/work/blog/content/home  
Открыли skills.md  
Внесли соответствующие изменения в файл (изменили иконки, описание и названия иконок). Также у меня добавлен эмоджи в виде земного шара. 
(Рис. [-@fig:001])

![Меняем skills](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-52-28.png){#fig:001 width=70%}

2. В этом же каталоге home открыли файл experience.md и внесли свои изменения (исправили заголовок, локацию, даты, описание и организацию).
   (Рис. [-@fig:002])

![Меняем experience](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-52-58.png){#fig:002 width=70%} 

3.  (Рис .[-@fig:003])  
Изменили ссылки на организации, исправили даты, описание, наименование организации, заголовок и тд).

![Меняем accomplishments](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-53-19.png){#fig:003 width=70%} 

4. Переходим в ~/work/blog/content/post и создаём там две папки, соответствующие названиям постов: Last_week2 и Markdown.  
Копируем файл из папки getting-started и изменяем информацию в файле аналогично как во втором этапе проекта.  
Добавляем картиночки. (Рис .[-@fig:004] - Рис .[-@fig:005]).

![Добавили картинку к посту о прошедшей неделе](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-50-20.png){#fig:004 width=70%}

![Добавили картинку к посту про язык разметки](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-50-27.png){#fig:005 width=70%}

5. Запускаем терминал, вводим следующие команды:  
- hugo (~/work/blog)  
- cd public
- git add .
- git commit -am "Comment"
- git push origin main (Рис .[-@fig:006]) 

![Загружаем данные на гитхаб](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-08-02.png){#fig:006 width=70%}

6. Проверяем страницу. (Рис .[-@fig:007] - Рис .[-@fig:0010]) 

![Обновлённые skills](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-11-19.png){#fig:007 width=70%}

![Обновлённый experience](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-11-28.png){#fig:008 width=70%}

![Обновлённыe accomplishments](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2020-22-17.png){#fig:009 width=70%}

![Добавились посты](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-11-50.png){#fig:0010 width=70%}

7. Читаем посты. (Рис .[-@fig:0011] - Рис .[-@fig:0012]) 

![Пост про прошедшую неделю](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-51-22.png){#fig:0011 width=70%}

![Пост про Markdown](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-51-42.png){#fig:0012 width=70%}

## **Вывод:** 

Таким образом, я добавила к сайту: информацию о навыках (Skills),опыте (Experience) и  достижениях (Accomplishments).  
Сделала пост по прошедшей неделе.  
Добавила пост на тему "Язык разметки Markdown".
