---
## Front matter
title: "ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ №3"
subtitle: "Язык разметки Markdown"
author: "Панченко Денис Дмитриевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
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
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Освоить процедуру оформления отчетов с помощью легковесного языка разметки Markdown.

# Выполнение лабораторной работы

1) Открываем терминал и переходим в каталог курса, сформированный при выполнении лабораторной работы №2. (Рис. 1)

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.001.png)
Рис. 1. Терминал 

2) Обновляем локальный репозиторий, скачав изменения из удаленного репозитория. (Рис. 2) 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.002.png)
Рис. 2. Обновление локального репозитория 

3) Перейдем в каталог с шаблоном отчета по лабораторной работе №3. (Рис. 3) 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.003.png)
Рис. 3. Каталог с шаблоном 

4) Проведем компиляцию шаблона с использованием Makefile. (Рис. 4) А также проверим корректность полученных файлов. (Рис. 5) 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.004.png)
Рис. 4. Компиляция шаблона 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.005.png)
Рис. 5. Полученные файлы 

5) Удаляем полученный файлы с использованием Makefile. (Рис. 6) А также проверим это. (Рис. 7) 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.006.png)
Рис. 6. Удаление файлов 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.007.png)
Рис. 7. Файлы 

6) Откроем файл report.md c помощью текстового редактора gedit. (Рис. 8-9) 
![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.008.png)
Рис. 8. Открытие текстового файла 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.009.jpeg)
Рис. 9. Текстовый файл 

7) Заполняем отчет и скомпилируем его с использованием Makefile. (Рис. 10-11)  Проверяем корректность полученных файлов. (Рис. 12) 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.010.jpeg)
Рис. 10. Отчет 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.011.png)
Рис. 11. Компилируем отчет 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.012.png)
Рис. 12. Файлы 

3) Загружаем файлы на Github. (Рис. 13-14) 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.013.png)
Рис. 13. Загружаем файлы на GitHub 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.014.png)
Рис. 14. Загружаем файлы на GitHub 

Задание для самостоятельной работы. 

1) Создаем отчёт по лабораторной работе №2 в формате Markdown и загружаем его на GitHub. (Рис. 15) 

![](image/Aspose.Words.c520a693-c006-4504-abe8-2a0a7b4297d8.015.jpeg)
Рис. 15. Отчет 

# Вывод

В ходе выполнения данной лабороторной работы я освоил процедуру оформления отчетов с помощью легковесного языка разметки Markdown. 
