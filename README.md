# HW_1.-Ksendzov.
GitBash Linux.

1. Посмотреть где я:  
**pwd**
1. Создать папку:  
**mkdir QA**
1. Зайти в папку:  
**cd /home/user/QA**
1. Создать 3 папки:  
**mkdir learn_qa1 learn_qa2 learn_qa3**
1. Зайти в любую папку:  
**cd learn_qa1/**
1. Создать 5 файлов (3 txt, 2 json):  
**cat file1.txt file2.txt file3.txt file1.json file2.json**
1. Создать 3 папки:  
**mkdir repo1 repo2 repo3**
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
**mv file_1.txt file_2.txt learn_qa2**
1. Скопировать любые 2 файла, которые вы создали, в любую другую папку:  
**cp file1.json file2.json learn_qa3**
1. Найти файл по имени:  
**find –name file_1.txt**
1. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает:  
**tail –f learn_qa2/file_1.txt**
1. Вывести несколько первых строк из текстового файла:  
**head –n3 learn_qa2/file_1.txt**
1. Вывести несколько последних строк из текстового файла:  
**tail –n3 learn_qa2/file_1.txt**
1. Просмотреть содержимое длинного файла (команда less) изучите как она работает:  
**less learn_qa2/file_1.txt**
1. Вывести дату и время:  
**date**


1. Отправить http запрос на сервер. http://162.55.220.72:5005/terminal-hw-request:  
**curl http://162.55.220.72:5005/terminal-hw-request**
1. Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13:  
  
cat > script.sh  
#!/bin/bash  
cd /home/user/QA/  
mkdir learn_qa1 learn_qa2 learn_qa3  
cd learn_qa1  
cat file1.txt file2.txt file3.txt file1.json file2.json  
mkdir repo1 repo2 repo3  
ls –la  
mv file_1.txt file_2.txt learn_qa2  
// Enter, Ctrl+C  
chmod +x script.sh  
bash script.sh  
