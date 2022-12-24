---
## Front matter
title: "ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ №6"
subtitle: "Арифметические операции в NASM."
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

Освоить арифметические инструкции языка ассемблера NASM.

# Выполнение лабораторной работы

1) Создаем каталог для программ лабораторной работы № 6, переходим в него и создаем файл lab6-1.asm. (Рис. 1)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.001.png)
Рис. 1. Создание каталога с файлом

2) Рассмотрим примеры программ вывода символьных и численных значений. Программы будут выводить значения записанные в регистр eax. (Рис. 2)
Создаем исполняемый файл и запускаем его. (Рис. 3)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.002.png)
Рис. 2. Текст программы

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.003.png)
Рис. 3. Запуск файла

3) Далее изменяем текст программы и вместо символов, записываем в регистры числа. Исправляем текст программы. (Рис. 4)
Создаем исполняемый файл и запускаем его. (Рис. 5)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.004.png)
Рис. 4. Текст программы

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.005.png)
Рис. 5. Запуск файла

4) Создаем файл lab6-2.asm в каталоге ~/work/arch-pc/lab06 и вводим в него текст программы. (Рис. 6-7)
Создаем исполняемый файл и запускаем его. (Рис. 8)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.006.png)
Рис. 6. Создание файла

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.007.png)
Рис. 7. Текст программы

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.008.png)
Рис. 8. Запуск файла

5) Аналогично предыдущему примеру изменяем символы на числа. (Рис. 9)
Создаем исполняемый файл и запускаем его. (Рис. 10)
Заменяем функцию iprintLF на iprint. Создаем исполняемый файл и запускаем его. (Рис. 11-12)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.009.png)
Рис. 9. Текст программы

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.010.png)
Рис. 10. Запуск файла

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.011.png)
Рис. 11. Текст программы

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.012.png)
Рис. 12. Запуск файла

Разница в том, что подпрограмма iprintLF переводит сообщение на следующую строку, а iprint данного действия не делает.

6) Создаем файл lab6-3.asm в каталоге ~/work/arch-pc/lab06 и вводим в него текст программы. (Рис. 13-14)
Создаем исполняемый файл и запускаем его. (Рис. 15)
Изменяем текст программы для вычисления выражения 𝑓(𝑥)=(4∗6+2)/5. (Рис. 16)
Создаем исполняемый файл и проверяем его работу. (Рис. 17)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.013.png)
Рис. 13. Создание файла

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.014.png)
Рис. 14. Текст программы

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.015.png)
Рис. 15. Запуск файла

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.016.png)
Рис. 16. Изменения

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.017.png)
Рис. 17. Запуск файла

7) Создаем файл variant.asm в каталоге ~/work/arch-pc/lab06 и вводим в него текст программы. (Рис. 18-19)
Создаем исполняемый файл и запускаем его. (Рис. 20)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.018.png)
Рис. 18. Создание файла

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.019.png)
Рис. 19. Текст программы

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.020.png)
Рис. 20. Запуск файла

1. Какие строки листинга 7.4 отвечают за вывод на экран сообщения ‘Ваш вариант:’?
mov eax,rem 
call sprint
2. Для чего используется следующие инструкции nasm? 
mov ecx,x – запись входной переменной в регистр ecx;
mov edx,80 – запись переменной в регистр edx;
call spread – вызов процедуры чтения данных.
3. Для чего используется инструкция “call atoi”?
Для вызова подпрограммы преобразования ASCII кода в число, `eax=x`.
4. Какие строки листинга 7.4 отвечают за вычисления варианта?
xor edx,edx
mov ebx,20
div ebx
inc edx.
5. В какой регистр записывается остаток от деления при выполнении инструкции “div ebx”?
В регистр ebx.
6. Для чего используется инструкция “inc edx”?
Для увелечения на 1.
7. Какие строки листинга 7.4 отвечают за вывод на экран результата вычислений?
mov eax,rem
call sprint
mov eax,edx
call iprintLF.

**Задание для самостоятельной работы.**

1)Напишем программу вычисления выражения 𝑦 = (11 + 𝑥) ⋅ 2 – 6 (Вариант 8). (Рис. 21)
Получаем исполняемый файл и проверяем его работу для значений x1 = 1 и x2 = 9 (Вариант 8). (Рис. 22)

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.021.png)
Рис. 21. Текст программы

![](image/Aspose.Words.0fb6742c-d4db-4dcb-b256-541845a2753d.022.png)
Рис. 22. Запуск файла

# Вывод

В ходе выполнения данной лабороторной работы я освоил арифметические инструкции языка ассемблера NASM.
