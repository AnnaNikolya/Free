					**Group 29_QA_FREE**
 
Telegram @anyutanik 

HW_1. The first part

_**Linux terminal (GitBash) commands**_

1.  Посмотреть где я **`pwd`**
1. Создать папку **`mkdir`** *`name`*
1. Зайти в папку **`cd`** *`mane`*
1. Создать 3 папки **`mkdir`** *`qa1 qa2 qa`3* 
1. Зайти в любую папку **`cd`** *`qa1`* 
2. Открыть в проводнике **`open .`**
1. Создать 5 файлов (3 txt, 2 json) **`touch`** *`qq.txt qq1.txt qq2.txt qq.json qq1.json`*
1. Вывести список содержимого папки **`ls -la`**
1. Открыть любой txt файл **`vim`** *`name.txt`*
1. написать туда что-нибудь, любой текст **`I `**- *вводим текст*
1. Сохранить и выйти **`ESC  :wq Enter `**
1. Выйти из папки на уровень выше **`cd ../`**
1. Переместить любой файл, который вы создали, в любую другую папку. **`mv`** *`qq2.txt qa2`*
1. скопировать файл, который вы создали, в любую другую папку. **`cp -R`** *`qq.txt qa3`*
1. Найти файл по имени **`find -name`** *`'*.txt' `*
1. росмотреть содержимое в реальном времени
1. **`tail -F `** *test.txt*
1. Вывести несколько первых строк из текстового файла **head** *`-2 qq1.txt`* (цифра обозначает количество строк для вывода)
1. Вывести несколько последних строк из текстового файла **`tail`** *`-2 file.txt`* 
1. Просмотреть содержимое длинного файла (команда less) изучите как она работает **`less`** *`file.txt`*
1. Вывести дату и время **`date +%c`**

	## Задание *
1) Отправить http запрос на сервер.
[http://162.55.220.72:5005/terminal-hw-request]()

*curl -X GET http://162.55.220.72:5005/terminal-hw-request
*
{"Intro":"Hello!! This is your the first response from server","Tasks":{"Task_1":"Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)","result":["Your_String","Your_number"]}}

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

* - Для этого создаем файл с расширением sh
touch myscript1.sh и заполняем его командами
* .*#!/bin/bash
echo "It's my first scri"
cd group && mkdir q1 > cd q1 & mkdir q2 q3 q4; 
cd q1 && touch q1.txt q2.txt q3.txt q4.json q5.json; touch a b c; ls -la > mv q1.txt a 
echo "Кто молодец? Я молоцец!"*

* Чтобы bash-скрипт работал, для начала нужно изменить права доступа с помощью команды **`chmod +x`**
chmod +x myscript1.sh 
* Запустить скрипт можно 2 способами:
> 1. ./myscript1.sh  
> 1. bash myscript1.sh 
