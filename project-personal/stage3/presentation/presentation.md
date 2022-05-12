---
## Front matter
lang: ru-RU
title: "Добавить к сайту достижения"
author: |
        Щербак Маргарита Романовна

institute: |
           RUDN
date: 2022

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

## **Цель работы**
Добавить к сайту: информацию о навыках (Skills),опыте (Experience) и  достижениях (Accomplishments).  
Сделать пост по прошедшей неделе.  
Добавить пост на тему "Язык разметки Markdown".

## **Ход работы:** Перешли в ~/work/blog/content/home  (Рис. [-@fig:001]).
- Открыли skills.md  
- Внесли соответствующие изменения в файл (изменили иконки, описание и названия иконок).   Также у меня добавлен эмоджи в виде земного шара. 

![Меняем skills](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-52-28.png){#fig:001 width=50%}

## В этом же каталоге home открыли файл experience.md и внесли свои изменения (исправили заголовок, локацию, даты, описание и организацию). (Рис. [-@fig:002])

![Меняем experience](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-52-58.png){#fig:002 width=70%} 

## В файле accomplishments.md изменили ссылки на организации, исправили даты, описание, наименование организации, заголовок и тд). (Рис .[-@fig:003])

![Меняем accomplishments](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-53-19.png){#fig:003 width=70%}

## Переходим в ~/work/blog/content/post и создаём там две папки, соответствующие названиям постов: Last_week2 и Markdown.  
Копируем файл из папки getting-started и изменяем информацию в файле аналогично как во втором этапе проекта.  
Добавляем картиночки. (Рис .[-@fig:004] - Рис .[-@fig:005]).

![Добавили картинку к посту о прошедшей неделе](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-50-20.png){#fig:004 width=65%}

## Выполнение

![Добавили картинку к посту про язык разметки](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-50-27.png){#fig:005 width=70%}

## Запускаем терминал, вводим следующие команды:  
- hugo (~/work/blog)  
- cd public
- git add .
- git commit -am "Comment"
- git push origin main (Рис .[-@fig:006]) 

![Загружаем данные на гитхаб](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-08-02.png){#fig:006 width=65%}

## Проверяем страницу. (Рис .[-@fig:007] - Рис .[-@fig:0010]) 

![Обновлённые skills](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-11-19.png){#fig:007 width=90%}

## Experience

![Обновлённый experience](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-11-28.png){#fig:008 width=90%}

## Accomplishments

![Обновлённыe accomplishments](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2020-22-17.png){#fig:009 width=90%}

## посты

![Добавились посты](image/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202022-05-12%2015-11-50.png){#fig:0010 width=90%}


## **Вывод:** 

Таким образом, я добавила к сайту: информацию о навыках (Skills),опыте (Experience) и  достижениях (Accomplishments).  
Сделала пост по прошедшей неделе.  
Добавила пост на тему "Язык разметки Markdown".
