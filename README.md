# HW_1.-Ksendzov.
GitBash Linux.

1. Посмотреть где я:  
**pwd**
1. Создать папку:  
**mkdir QA**
1. Зайти в папку:  
**cd /home/User/QA-Ksendzov/Lessson_1/**  
1. Создать 3 папки:  
**mkdir 1 2 3**
1. Зайти в любую папку:  
**cd 1**
1. Создать 5 файлов (3 txt, 2 json):  
**touch 1.txt 2.txt 3.txt 1.json 2.json**
1. Создать 3 папки:  
**mkdir 1 2 3**
1. Вывести список содержимого папки:  
**ls –la**
1. Открыть любой txt файл:  
**vim file1.txt**
1. Написать туда что-нибудь, любой текст:  
**Нажать “I” + написать:**

   Hello World!!!  
   213  
   213  
   123123  
   I’m learn QA  
   bye!
1. Сохранить и выйти:  
**Esc + :wq**
1. Выйти из папки на уровень выше:  
**cd ..**
1. Переместить любые 2 файла, которые вы создали, в любую другую папку:  
**mv 1/1.txt 1/2.txt ./3/**
1. Скопировать любые 2 файла, которые вы создали, в любую другую папку:  
**cp 1/1.json 1/2.json ./3/**
1. Найти файл по имени:  
**find –name 1.txt**
1. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает:  
**tail –f 2/1.txt**
1. Вывести несколько первых строк из текстового файла:  
**head –n3 2/1.txt**
1. Вывести несколько последних строк из текстового файла:  
**tail –n3 2/1.txt**
1. Просмотреть содержимое длинного файла (команда less) изучите как она работает:  
**less 2/1.txt**
1. Вывести дату и время:  
**date**


1. Отправить http запрос на сервер. http://162.55.220.72:5005/terminal-hw-request:  
**curl http://162.55.220.72:5005/terminal-hw-request**  
{"Intro":"Hello!! This is your the first response from server","Tasks":{"Task_1":"Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)","result":["Your_String","Your_number"]}}  
**curl "http://162.55.220.72:5005/get_method?name=Vladimir&age=25"**  
["Vladimir","25"]

1. Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13:  
  
#!/bin/bash  
cd /home/User/QA-Ksendzov/Lessson_1  
mkdir 1 2 3
cd 1  
touch 1.txt 2.txt 3.txt 1.json 2.json  
mkdir 1 2 3  
ls –la  
mv ./1.txt ./2.txt ./3

chmod +x script.sh  
bash script.sh  
