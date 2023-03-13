# Lab Report 5: Continuation of Reseraching from Lab 3

- ```$ history``` ([source](https://www.cherryservers.com/blog/a-complete-guide-to-linux-bash-history))
> $ history 
>  
> 1 ls
> 
> 2 cd written_2
> 
> 3 bash.sh
> 
> 4 history 

The command ```history``` was used in the docsearch file of lab 3 and purpose was to get all the past commands written within the terminal similar to seeing your search history but instead it's the past commands as shown above. This is useful to troubleshoot to see which command caused an error, learn and improve commands, and security to see a potential breach in the system. ```history``` also have numeric number to shoow in what order the command was executed. These numeric number are useful in executing a specific command which is shown in ```$ ![number]``` section.

- ```$ ![number]``` ([source](https://www.cherryservers.com/blog/a-complete-guide-to-linux-bash-history))
> $!1
> 
> berlitz2-wordcount.txt  DocSearchServer.java  grep-results.txt  README.md    start.sh  TestDocSearch.java
count-txts.sh           find-results.txt      lib/              Server.java  test.sh   written_2/

The command ```$ ![number]``` was used in the docsearch file in lab 3 and the purpose was to recall a past command and execute it based on number given. The number arguement was defined by the result of ```history``` in ```$ history``` section. This is useful for recall and reuse previously executed commands without having to type them out again. This can save you time and increase your productivity. 

- ```$ cp -r [dir1] [dir2]``` ([source](https://www.geeksforgeeks.org/cp-command-linux-examples/))
> $ mkdir kevin
> $ cp -r travel_guides kevin
