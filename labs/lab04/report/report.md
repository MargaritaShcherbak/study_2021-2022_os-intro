---
## Front matter
title: "Отчёт по лабораторной работе №4"
subtitle: "Основы интерфейса взаимодействия
пользователя с системой Unix на уровне командной строки"
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

# **Основы интерфейса взаимодействия пользователя с системой Unix на уровне командной строки** 

## **Цель работы**
Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.


### Из теории: 
В операционной системе типа Linux взаимодействие пользователя с системой обычно
осуществляется с помощью командной строки посредством построчного ввода команд. При этом обычно используется командные интерпретаторы языка shell: /bin/sh;
/bin/csh; /bin/ksh.

Командой в операционной системе называется записанный по специальным правилам текст (возможно с аргументами), представляющий собой указание на выполнение какой-либо функции (или действия) в операционной системе.
Обычно первым словом идёт имя команды, остальной текст — аргументы или опции,
конкретизирующие действие.
Общий формат команд можно представить следующим образом:
<имя_команды><разделитель><аргументы>

## **Ход работы**

1. Определили полное имя своего домашнего каталога(команда pwd).
2. Выполнили следующие действия: (Рис. [-@fig:001])
  - Перешли в каталог /tmp.
  - Вывели на экран содержимое каталога /tmp. Для этого использовали команду ls с различными опциями.
  - Определили, есть ли в каталоге /var/spool подкаталог с именем cron.
  - Перешли в домашний каталог и вывели на экран его содержимое. (cd /home) (ls)
  - Определили, кто является владельцем файлов и подкаталогов? (ls -l)

![Выполнение действий](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-04-28%2022-19-21.png){#fig:001}

3. Выполнили следующие действия:
- В домашнем каталоге создали новый каталог с именем newdir.
- В каталоге ~/newdir создали новый каталог с именем morefun.
- В домашнем каталоге создали одной командой три новых каталога с именами
letters, memos, misk. Затем удалили эти каталоги одной командой.
- Попробовали удалить ранее созданный каталог ~/newdir командой rm. Проверили,
был ли каталог удалён.
- Удалили каталог ~/newdir/morefun из домашнего каталога. Проверили, был ли
каталог удалён. (Рис. [-@fig:002]) 

![Дальнейшее выполнение команд](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-04-28%2022-29-48.png){#fig:002}  

4. С помощью команды man определили, какую опцию команды ls нужно использовать для просмотра содержимого не только указанного каталога, но и подкаталогов,входящих в него.
(Рис. [-@fig:003])  

![Просмотр содержимого каталога и входящих в него подкаталогов](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-04-28%2022-34-02.png){#fig:003 width=70%}


5. С помощью команды man определили набор опций команды ls, позволяющий отсортировать по времени последнего изменения выводимый список содержимого каталога с развёрнутым описанием файлов.(Рис. [-@fig:004] - [-@fig:005] ) 

6. Использовали команду man для просмотра описания следующих команд: cd, pwd, mkdir,
rmdir, rm. 

7. Используя информацию, полученную при помощи команды history, выполнили модификацию и исполнение нескольких команд из буфера команд. 

![Вводим необходимые команды](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-04-28%2022-40-57.png){#fig:004 width=70%}

![Выполнили модификацию и исполнение нескольких команд из буфера обмена](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-04-28%2022-41-42.png){#fig:005 width=70%}

## **Вывод:** 

Таким образом, я приобрела практические навыки взаимодействия пользователя с системой посредством командной строки.