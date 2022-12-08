---
## Front matter
title: "ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ №5"
subtitle: "Основы работы с Midnight Commander. Структура программы на языке ассемблера NASM"
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

Приобрести практические навыки работы в Midnight Commander. Освоить инструкции языка ассемблера mov и int.

# Выполнение лабораторной работы

1) Открываем Midnight Commander. (Рис. 1-2)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.001.png)
Рис. 1. Вызов Midnight Commander

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.002.png)
Рис. 2. Midnight Commander

2) Переходим в каталог ~/work/archpc. (Рис. 3)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.003.png)
Рис. 3. Каталог

3) Создаем папку lab05. (Рис. 4)
И переходим в созданный каталог. (Рис. 5)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.004.png)
Рис. 4. Создание каталога

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.005.png)
Рис. 5. Каталог

4) Создаем файл lab5-1.asm. (Рис. 6)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.006.png)
Рис. 6. Создание файла

5) Открываем файл lab6-1.asm для редактирования. (Рис. 7)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.007.png)
Рис. 7. Открытие файла

6) Вводим текст программы, сохраняем изменения и закрываем файл. (Рис. 8)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.008.png)
Рис. 8. Программа

7) Открываем файл lab5-1.asm для просмотра. Убеждаемся, что файл содержит текст программы. (Рис. 9)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.009.png)
Рис. 9. Программа

8) Оттранслируем текст программы lab5-1.asm в объектный файл. Выполним компоновку объектного файла и запустим получившийся исполняемый файл. (Рис. 10)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.010.png)
Рис. 10. Запуск файла

**5.3.1. Подключение внешнего файла in\_out.asm**

9) Скачаем файл in\_out.asm со страницы курса в ТУИС. (Рис. 11) 

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.011.png)
Рис. 11. Загрузка файла

10) Скопируем файл in\_out.asm в каталог с файлом lab5-1.asm. (Рис. 12) 

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.012.png)
Рис. 12. Копирование файла

11) Создаем копию файла lab5-1.asm с именем lab5-2.asm. (Рис. 13)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.013.png)
Рис. 13. Копия файла

12) Исправим текст программы в файле lab5-2.asm. (Рис. 14)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.014.png)
Рис. 14. Текст программы

13) Создаем исполняемый файл и проверяем его работу. (Рис. 15)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.015.png)
Рис. 15. Запуск файла

14) Заменяем подпрограмму sprintLF на sprint в файле lab5-2.asm. (Рис. 16)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.016.png)
Рис. 16. Изменения

15) Создаем исполняемый файл и проверяем его работу. (Рис. 17)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.017.png)
Рис. 17. Запуск файла

Разница в том, что подпрограмма sprintLF переводит сообщение на следующую строку, а sprint данного действия не делает.

**Задание для самостоятельной работы.**

1) Создаем копию файла lab5-1.asm. (Рис. 18)
Вносим изменения в программу. (Рис. 19)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.018.png)
Рис. 18. Создание копии

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.019.png)
Рис. 19. Изменения

2) Получаем исполняемый файл и проверяем его работу. (Рис. 20)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.020.png)
Рис. 20. Запуск файла

3) Создаем копию файла lab5-2.asm. (Рис. 21)
Вносим изменения в программу. (Рис. 22)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.021.png)
Рис. 21. Создание копии

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.022.png)
Рис. 22. Изменения

4) Получаем исполняемый файл и проверяем его работу. (Рис. 23)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.023.png)
Рис. 23. Запуск файла

# Вывод

В ходе выполнения данной лабороторной работы я приобрел практические навыки работы в Midnight Commander и освоил инструкции языка ассемблера mov и int.
