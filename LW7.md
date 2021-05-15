---
# Front matter
lang: ru-RU
title: " Поиск файлов. Перенаправление ввода-вывода. Просмотр запущенных процессов"
subtitle: "ЛР по ОС №7"
author: "Аникин Константин Сергеевич"
group: НПИбд-01-20

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

- Ознакомление с инструментами поиска файлов и фильтрации текстовых данных. 

- Приобретение практических навыков: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.


# Задание

- Ознакомиться с теоретическим материалом

- Выполнить задание лабораторной


# Выполнение лабораторной работы

1. Я не понял, что подразумевается этим пунктом. Просто войти в систему под своим именем? Я это и так каждый раз делаю.

2. Запись названий файлов папки etc и домашнего каталога (рис. 2.1)

![](images/021.png)

*Рис. 2.1: Запись названий файлов папки etc и домашнего каталога*

... и вывод результатов работы (рис. 2.2)

![](images/022.png)

*Рис. 2.2: Вывод результатов работы*

3. Запись названий всех .conf файлов в conf.txt

Во время работы я ошибся. Надо было указать "\*.conf" вместо ".conf", в файл попали лишние названия (рис. 3)

![](images/031.png)

*Рис. 3: Запись названий всех .conf файлов в conf.txt*

4. Команда для вывода всех файлов домашнего каталога, начинающихся на c. 

Второй вариант - записать все названия в файл, после чего вывести их cat-ом или подобным. (рис. 4)

![](images/041.png)

*Рис. 4: Вывод всех файлов домашнего каталога, начинающихся на c*

5. Программа для вывода всех файлов из etc, начинающихся на h, на экран. (рис. 5.1)

![](images/051.png)

*Рис. 5.1: Программа для вывода всех файлов из etc, начинающихся на h*

И результаты работы программы  (рис. 5.2)

Как вывести это постранично, я так и не разобрался.

![](images/052.png)

*Рис. 5.2: Результат работы программы*

6. Программа для запуска в фоновом режиме записи log файлов в logfile (рис. 6)

![](images/061.png)

*Рис. 6: Программа для запуска в фоновом режиме записи log файлов в logfile*

7. Удаление logfile (рис. 7)

![](images/071.png)

*Рис. 7: Удаление logfile*

8-9. Запуск gedita фоном, узнавание идентификатора процесса ps-ом

Узнать идентификатор можно проще, либо командой jobs, 

либо посмотрев на номер работы при создании процесса (рис. 8)

![](images/08191.png)

*Рис. 8: Пункты 8 и 9*

10. Убийство gedita (рис. 10)

![](images/101.png)

*Рис. 10: Убийство gedita*

11. Выведенный man по df (рис. 11.1)

![](images/111.png)

*Рис. 11.1: man df*

Результат работы команды df (рис. 11.2)

![](images/112.png)

*Рис. 11.2: Команда df*

Выведенный man по du (рис. 11.3)

![](images/113.png)

*Рис. 11.3: man du*

Результат работы команды du (рис. 11.4)

![](images/114.png)

*Рис. 11.2: Команда du*

12. Команда для вывода всех подпапок домшнего каталога (рис. 12.1)

![](images/121.png)

*Рис. 12.1: Вывод всех подпапок каталога ~*

Также я нашёл способ вывести только подпапки текущего каталога, но без команды find (рис. 12.2)

![](images/122.png)

*Рис. 12.2: Вывод подпапок каталога ~*

# Выводы

По ходу работы возникли недопонимания, и сказать, что всё выполнено правильно, я не могу, однако большая часть должна быть сделана верно.