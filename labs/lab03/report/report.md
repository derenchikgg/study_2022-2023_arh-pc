---
## Front matter
title: "ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ №2"
subtitle: "Система контроля версий Git"
author: "Панченко Денис Дмитриевич"

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

Изучить идеологию и применение средств контроля версий. Приобрести практические навыки по работе с системой git.

# Выполнение лабораторной работы

1. Настройка github 

Создаём учётную запись на сайте https://github.com/ и заполняем основные данные. (Рис. 1) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.001.jpeg)
Рис. 1. Учетная запись GitHub 

2. Базовая настройка git 

1) Сначала сделаем предварительную конфигурацию git. Откроем терминал и введем следующие команды, указав свое имя и email. (Рис. 2) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.002.png)
Рис. 2. Имя и email 

2) Настроим utf-8 в выводе сообщений git. (Рис. 3) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.003.png)
Рис. 3. Настройка utf-8 

3) Зададим имя начальной ветки (будем называть её master). (Рис. 4) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.004.png)
Рис. 4. Начальная ветка 

4) Параметр autocrlf. (Рис. 5) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.005.png)
Рис. 5. Параметр autocrlf 

5) Параметр safecrlf. (Рис. 6) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.006.png)
Рис. 6. Параметр safecrlf 

3. Создание SSH ключа 
1) Для последующей идентификации пользователя на сервере репозиториев сгенерируем пару ключей (приватный и открытый). (Рис. 7) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.007.jpeg)
Рис. 7. Генерация ключей 

2) Скопируем из локальной консоли ключ в буфер обмена. (Рис. 8) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.008.png)
Рис. 8. Скопированный ключ 

3) Загружаем сгенерённый открытый ключ на GitHub. (Рис. 9) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.009.png)
Рис. 9. Загруженный ключ 

4. Создание рабочего пространства и репозитория курса на основе шаблона. 

Создадим каталог для предмета «Архитектура компьютера». (Рис. 10) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.010.png)
Рис. 10. Создание каталога 

5. Создание репозитория курса на основе шаблона. 
1) Создаём репозиторий на GitHub. (Рис. 11-12) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.011.png)
Рис. 11. Репозиторий на GitHub 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.012.jpeg)
Рис. 12. Репозиторий на GitHub 

2) Откроем терминал и перейдем в каталог курса. (Рис. 13) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.013.png)
Рис. 13. Каталог курса 

3) Клонируем созданный репозиторий. (Рис. 14) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.014.jpeg)
Рис. 14. Клонирование репозитория 

6. Настройка каталога курса. 
1) Перейдем в каталог курса. (Рис. 15) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.015.png)
Рис. 15. Каталог курса 

2) Удаляем лишние файлы. (Рис. 16) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.016.png)
Рис. 16. Удаление лишних файлов 

3) Создаем необходимые каталоги. (Рис. 17) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.017.png)
Рис. 17. Создание каталогов 

4) Отправляем файли на сервер. (Рис. 18-19) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.018.png)
Рис. 18. Отправка файлов 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.019.png)
Рис. 19. Отправка файлов 

5) Проверяем правильность создания иерархии рабочего пространства в локальном репозитории и на странице GitHub. (Рис. 20) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.020.jpeg)
Рис. 20. Репозиторий 

2.5. Задание для самостоятельной работы. 

1) Создаём отчет по выполнению лабораторной работы в соответствующем каталоге рабочего пространства (labs>lab03>report). (Рис. 21) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.021.jpeg)
Рис. 21. Отчет по выполнению ЛР 

2) Скопируем отчеты по выполнению предыдущих лабораторных работ в соответствующие каталоги созданного рабочего пространства. (Рис. 22) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.022.jpeg)
Рис. 22. Отчет по выполнению ЛР 

3) Загружаем файлы на GitHub. (Рис. 23) 

![](image/Aspose.Words.88e81674-4da9-42a2-b8a3-193e1d7d0d89.023.jpeg)
Рис. 23. Файлы на GitHub 

# Вывод

В ходе выполнения данной лабороторной работы я изучил идеологию и применение средств контроля версий, а также приобрел практические навыки по работе с системой git. 
