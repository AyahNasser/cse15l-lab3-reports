# cse15l-lab3-reports
----------------
**Researching Commands**
 - Chosen Command is (grep).
 
 - grep command is in command line searches for words in a file . 
 
 - 1) -i
 The command line -i option is a kind of a command line option that ignores the case sensitivity when searching of a pattren. 
 This command line is helpful when you want to search something in a file, and you want all the words in lower and upper case. Because this command line
 will not distinguish between uppercase and lowecase. 
 - For example, in the screenshot below, i wanted to look for the word history in the HistoryJapan.txt file, and as we can see that i wrote the history 
 with all loswecases, but it did show the uppercase words of History. 
 
 - a) Using -i the command-line and its output Example 1:
 
  ````
 ayahsmacbook.@Ayahss-MBP berlitz1 % grep -i "history" HistoryJapan.txt 
        A Brief History
        Prehistory and Early Chronicles
        of Japan to study Chinese religion, history, music, literature, and
        At this early stage in its history Japan was already (for
 ````
 
 <img width="607" alt="Screenshot 2023-02-13 at 11 27 43 PM" src="https://user-images.githubusercontent.com/122571192/218668477-cb57e28d-56a4-49f2-8976-ecf9d2d7841f.png">
 
  - b) Using -i the command-line and its output Example 2: 
  ````
ayahsmacbook.@Ayahss-MBP berlitz1 % grep -i "according to the earliest" History
Japan.txt
        According to the earliest official accounts, the
  ````
  In this example, I wanted to look up the sentance in the txt file, howeever, I was not sure if the sentance is written in an uppercase letters or
  lowercases, so I just wrote the sentance I remember, and it gave me where the sentance did appear and how it is actuallu written. 
  
 - This is very useful because it saves time to go over the whole text to exatcly match how the sentance or word was written to search it. 
 
 
 
 - 2) -c 
 This command-line Shows how many a word appeared in a text file, and again it is not a case sensitive, which means I can write a word in lower or upper 
 case, and it will still give me how many times this specific word appeared. 
 
 - a) First example is a code block of how I wrote the terminal and the output. 
 
 ````
 ayahsmacbook.@Ayahss-MBP berlitz1 % grep -c "official" HistoryJapan.txt
 3
````
Here, I wanted to see how many times the word "official" appeared in the text file, and this is helpful again because it saves vso much time, instead
of counting each word in the terminal. 

- b) Second example is looking for the word "Hello" in a the WhatToGreek text file. 
````
ayahsmacbook.@Ayahss-MacBook-Pro berlitz1 % grep -c "Hello" WhatToGreek.txt 
0
````
Here I wanted to look for the word Hello in the text file (WhatToGreek), and the output was zero which means the word did not appear in the text file.
- This command-line is helpful because it saves you so much time counting how many times a word appeared, without having to go over all of the text file. 
Also, this becomes even more helpful when the text files get larger. 

- 3) -l
This command-line shows where a specific word appeared in differenet files, and it prints the names of the files thta have the word. Moreover, even if the word appeared more than once, the file name will be printed only once.  

- a) Here is an example of me trying to find where the word "Official" appeared in so many files. This is helpful because it is fast and it gives you a list of where the word appeared between so many files. 

````
ayahsmacbook.@Ayahss-MBP berlitz1 % grep -l "Official" *.txt
WhatToHongKong.txt
WhereToFrance.txt
WhereToMadrid.txt
`````
- The syntax to write the command was ```grep -l "Official" *.txt```, and the output was ```WhatToHongKong.txt WhereToFrance.txt WhereToMadrid.txt ``` which are the files where this word appeared. 

- b) The second example is trying to find all the files in a directory that contain a xertain pattren. 
````
ayahsmacbook.@Ayahss-MacBook-Pro berlitz1 % grep -l "^[0-9]*$" *
HandRHawaii.txt
HandRHongKong.txt
HandRIbiza.txt
HandRIsrael.txt
HandRIstanbul.txt
HandRJamaica.txt
HandRJerusalem.txt
HandRLakeDistrict.txt
HandRLasVegas.txt
HandRLisbon.txt
HandRLosAngeles.txt
HandRMadeira.txt
HandRMadrid.txt
HandRMallorca.txt
HistoryDublin.txt
HistoryEdinburgh.txt
HistoryEgypt.txt
HistoryFWI.txt
HistoryFrance.txt
HistoryGreek.txt
HistoryHawaii.txt
HistoryHongKong.txt
HistoryIbiza.txt
HistoryIndia.txt
HistoryIsrael.txt
HistoryIstanbul.txt
HistoryItaly.txt
HistoryJamaica.txt
HistoryJapan.txt
HistoryJerusalem.txt
HistoryLakeDistrict.txt
HistoryLasVegas.txt
HistoryMadeira.txt
HistoryMadrid.txt
HistoryMalaysia.txt
HistoryMallorca.txt
IntroDublin.txt
IntroEdinburgh.txt
IntroEgypt.txt
IntroFWI.txt
IntroFrance.txt
IntroGreek.txt
IntroHongKong.txt
IntroIbiza.txt
IntroIndia.txt
IntroIsrael.txt
IntroIstanbul.txt
IntroItaly.txt
IntroJamaica.txt
IntroJapan.txt
IntroJerusalem.txt
IntroLakeDistrict.txt
IntroLasVegas.txt
IntroLosAngeles.txt
IntroMadeira.txt
IntroMadrid.txt
IntroMalaysia.txt
IntroMallorca.txt
JungleMalaysia.txt
WhatToDublin.txt
WhatToEdinburgh.txt
WhatToEgypt.txt
WhatToFWI.txt
WhatToFrance.txt
WhatToGreek.txt
WhatToHawaii.txt
WhatToHongKong.txt
WhatToIbiza.txt
WhatToIndia.txt
WhatToIsrael.txt
WhatToIstanbul.txt
WhatToItaly.txt
WhatToJamaica.txt
WhatToJapan.txt
WhatToLakeDistrict.txt
WhatToLasVegas.txt
WhatToLosAngeles.txt
WhatToMadeira.txt
WhatToMalaysia.txt
WhatToMallorca.txt
WhereToDublin.txt
WhereToEdinburgh.txt
WhereToEgypt.txt
WhereToFWI.txt
WhereToFrance.txt
WhereToGreek.txt
WhereToHawaii.txt
WhereToHongKong.txt
WhereToIbiza.txt
WhereToIndia.txt
WhereToIsrael.txt
WhereToIstanbul.txt
WhereToItaly.txt
WhereToJapan.txt
WhereToJerusalem.txt
WhereToLakeDistrict.txt
WhereToLosAngeles.txt
WhereToMadeira.txt
WhereToMadrid.txt
WhereToMalaysia.txt
WhereToMallorca.txt
`````
- Here the command will search for lines that consist of only one or more digits in all files in the directory, then the command will print the names of all the files that contain the specified pattren. 
- This command-line is helpful because it helps you to quickly find a certain pattren through all the files in the directory without having to go through all the files one by one which again saves time and effort. 



- 4) choose one more with two examples 
  


 
 
 


