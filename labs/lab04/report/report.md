---
## Front matter
title: "ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ №4"
subtitle: "Создание и процесс обработки программ на языке ассемблера NASM"
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

Освоить процедуры компиляции и сборки программ, написанных на ассемблере NASM.

# Выполнение лабораторной работы

1) Создайте каталог для работы с программами на языке ассемблера NASM. (Рис. 1)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.001.png)
Рис. 1. Терминал

2) Переходим в созданный каталог. (Рис. 2)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.002.png)
Рис. 2. Каталог

3) Создаем текстовый файл с именем hello.asm. (Рис. 3)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.003.png)
Рис. 3. Создание файла

4) Открываем созданный файл и вводим в него предложенный текст. (Рис. 4)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.004.png)
Рис. 4. Ввод текста

**4.3.2. Транслятор NASM**

5) Компилируем приведённый выше текст программы «Hello World». (Рис. 5)
А также проверим это. (Рис. 6)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.005.png)
Рис. 5. Компиляция программы

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.006.png)
Рис. 6. Проверка

**4.3.3. Расширенный синтаксис командной строки NASM**

6) Скомпилирует исходный файл hello.asm в obj.o. (Рис. 7)
А также проверим это. (Рис. 8)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.007.png)
Рис. 7. Компиляция файла

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.008.png)
Рис. 8. Проверка

**4.4. Компоновщик LD**

7) Объектный файл передаем на обработку компоновщику. (Рис. 9) 
А также проверим это. (Рис. 10)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.009.png)
Рис. 9. Передача файла

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.010.png)
Рис. 10. Проверка

8) Выполняем предложенную команду: ld -m elf\_i386 obj.o -o main. (Рис. 11)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.011.png)
Рис. 11. Компиляция файла

Исполняемый файл имеет имя: **obj.o**
Объектный файл: **main**

**4.4.1. Запуск исполняемого файла**

9) Запустим на выполнение созданный исполняемый файл. (Рис. 12)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.012.png)
Рис. 12. Запуск файла

**Задание для самостоятельной работы.**

1) Создаем копию файла hello.asm с именем lab4.asm. (Рис. 13)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.013.png)
Рис. 13. Копия файла

2) Вносим изменения в текст программы в файле lab4.asm. (Рис. 14)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.014.png)
Рис. 14. Изменения

3) Оттранслируем полученный текст программы lab4.asm в объектный файл, выполним компоновку объектного файла и запустим получившийся исполняемый файл. (Рис. 15)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.015.png)
Рис. 15. Действия с файлом

4) Скопируем файлы hello.asm и lab5.asm в наш локальный репозиторий. (Рис. 16)
И загружаем файлы на Github. (Рис. 17-18)

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.016.png)
Рис. 16. Действия с файлами

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.017.png)
Рис. 17. Загрузка файлов на GitHub

![](image/Aspose.Words.880d177b-9580-4b97-8a75-3490a886fe51.018.png)
Рис. 18. GitHub 

# Вывод

В ходе выполнения данной лабороторной работы я освоил процедуры компиляции и сборки программ, написанных на ассемблере NASM.
