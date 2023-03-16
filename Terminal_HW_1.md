|Terminal HW_1                                                                           |Command|
|----------------------------------------------------------------------------------------|-----|
| 1) Посмотреть где я                                                                    | pwd |
| 2) Создать папку                                                                       | mkdir qa_homework    |
| 3) Зайти в папку                                                                       | cd qa_homework    |
| 4) Создать 3 папки                                                                     | mkdir hw1 hw2 hw3    |
| 5) Зайти в любоую папку                                                                | cd hw1    |
| 6) Создать 5 файлов (3 txt, 2 json)                                                    | touch 1.txt 2.txt 3.txt 1.json 2.json    |
| 7) Создать 3 папки                                                                     | mkdir a b c    |
| 8. Вывести список содержимого папки                                                    | ls -a    |
| 9) + Открыть любой txt файл                                                            | nano 1.txt    |
| 10) + написать туда что-нибудь, любой текст.                                           | 123 123 \n 123  |
| 11) + сохранить и выйти.                                                               | Ctrl+S Ctrl+X   |
| 12) Выйти из папки на уровень выше                                                     | cd ..    |
| 13) переместить любые 2 файла, которые вы создали, в любую другую папку.               | mv /i/'QA course Vadim'/HW/qa_homework/hw1{1.json,2.json} /i/'QA course Vadim'/HW/qa_homework/hw/a    |
| 14) скопировать любые 2 файла, которые вы создали, в любую другую папку.               | cp /i/'QA course_Vadim'/HW/qa_homework/hw1/a/{1.json,2.json} /i/'QA course_Vadim'/HW/qa_homework/hw1/b    |
| 15) Найти файл по имени                                                                | find . -name "1.txt"    |
|||
| 16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает. | cd hw1    |
||grep 123 "1.txt"|
||less +F 1.txt|
||ctrl+C|
||q|
| 17) вывести несколько первых строк из текстового файла                                 | head -3 1.txt     |
| 18) вывести несколько последних строк из текстового файла                              | tail -5 1.txt    |
| 19) просмотреть содержимое длинного файла (команда less) изучите как она работает.     | less -N 1.txt    |
| 20) вывести дату и время                                                               | date    |






|Terminal HW_1_Additional tasks                                                          |Command|
|----------------------------------------------------------------------------------------|-----|
|1) Отправить http запрос на сервер. http://162.55.220.72:5005/terminal-hw-request| curl http://162.55.220.72:5005/terminal-hw-request|
|2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13 | nano hw1_script.sh |
||#!/bin/bash
||cd qa_homework
||mkdir hw1 hw2 hw3
||cd hw1
||touch 1.txt 2.txt 3.txt 1.json 2.json
||mkdir a b c
||ls a
||mv *.json a
||echo "Скрипт выполнен. Пункты 3, 4, 5, 6, 7, 8, 13 завершены"
|| exit 0|
