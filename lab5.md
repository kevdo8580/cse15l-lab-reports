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
> $ !1
> 
> ls
> 
> berlitz2-wordcount.txt  DocSearchServer.java  grep-results.txt  README.md    start.sh  TestDocSearch.java
count-txts.sh           find-results.txt      lib/              Server.java  test.sh   written_2/

The command ```$ ![number]``` was used in the docsearch file in lab 3 and the purpose was to recall a past command and execute it based on number given. The number arguement was defined by the result of ```history``` in ```$ history``` section. This is useful for recall and reuse previously executed commands without having to type them out again. This can save you time and increase your productivity. 

- ```$ !!``` ([source](https://www.cherryservers.com/blog/a-complete-guide-to-linux-bash-history))
> $ !!
> 
> ls
> 
> berlitz2-wordcount.txt  DocSearchServer.java  grep-results.txt  README.md    start.sh  TestDocSearch.java
count-txts.sh           find-results.txt      lib/              Server.java  test.sh   written_2/

The command ```$ !!``` was used in docserach file of lab 3 after executing ```$ ![number]``` section. The purpose of ```$ !!``` is to execute the previous or last command used. The usefulness of this command is it can save you time as for example if you have a long line of command that needs to excecuted again or for automation in bash script.

- ```$ cp -r [dir1] [dir2]``` ([source](https://www.geeksforgeeks.org/cp-command-linux-examples/))
> $ mkdir kevin
> 
> $ cp -r travel_guides kevin
> 
> $ ls kevin
> 
> travel_guides/

The command ```$ cp -r [dir1] [dir2]``` was used in docsearch file of Lab 3 and purpose was to make a copy of dir1 to dir 2. Dir2 was created by using ```$ mkdir```. The ```$ cp -r``` command is useful for recursively copy directories and their contents, including subdirectories, files, and other directories to create a backup of a directory tree, or when you need to duplicate a directory structure for testing or development purposes.

- ```$ rm -r [dir]``` ([source](https://www.geeksforgeeks.org/rm-command-linux-examples/))
> $ rm -r kevin 
> 
> $ ls
> 
> non-fiction/  travel_guides/

The command ```$ rm -r [dir]``` was used in docserach of Lab 3 and after ```$ cp -r [dir1] [dir2]``` section where a new directory was created to copy contents of a directory to the new directory. The purpose of ```$ rm -r``` is to recursively deletes the contents of the given directory and is useful for cleaning up directory instead of a single file but also to delete directory after making a copy of a directory. 

- ```$ touch [File/Directory]``` ([source](https://www.educative.io/answers/what-is-the-touch-command-in-linux))

Example of ```$ touch [File]```
> $ touch a.txt
> 
> $ ls 
> 
> a.txt non-fiction/  travel_guides/

Example of ```$ touch [Directory]```
> $ touch ./non-fiction/b.txt
> 
> $ ls non-fiction 
> 
> b.txt  OUP/

The command ```$ touch [File/Directory]``` was used in docsearch lab 3 and the purpose is to create a new file. This is useful when you want to create a new file in the current directory or a specify directory in the terminal instead of manually adding and creating a file in text editor. You can also create multiple files at once so it's more efficent and less time consuming. 

- ```$ uniq [File]``` ([source](https://www.geeksforgeeks.org/uniq-command-in-linux-with-examples/))
> $ cat a.txt
> 
> KEVIN
> 
> KEVIN
> 
> KEVIN
> 
> LOL
> 
> $ uniq a.txt
> 
> KEVIN
> 
> LOL

The commmand ```$ uniq [File]``` uses the given file and removes duplicate lines from the give file. The return result is the file without duplicate lines which we can store the results by piping to a file by attaching ```> [File]``` to the end of ```$ uniq [File]```. The usefulness of this command is it allows you to easily identify and remove duplicate lines from a file or input stream. Duplicate lines can be a common problem when working with large datasets or logs, and can make it difficult to analyze the data accurately. By using this command you efficiently remove the duplicates. 

- ```$ uniq -c [File]``` ([source](https://www.geeksforgeeks.org/uniq-command-in-linux-with-examples/))
> $ cat b.txt
> 
> KEVIN 
> 
> KEVIN 
> 
> LOL
> 
> APPLE
> 
> $uniq -c b.txt
> 
> 2 KEVIN
> 
> 1 LOL
> 
> 1 APPLE

The command ```$ uniq -c [File]``` counts the number of occurance or count of each line in the terminal. This is useful when sorting out data because it allows you to count the number of occurrences of each unique line in a file or input stream. This can be useful for understanding patterns and trends in the data, and for identifying which lines are the most common or the least common. 







