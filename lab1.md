# Lab Report 1: Setting Up The Begining of CSE 15L Journey 
 
 
## Step 1: Installing Visual Art Studio and Setting Up The Enviroment 

Download visual art studio, if you haven't done so. Use this [link](https://code.visualstudio.com/) to get started. Once you have download visual art studio,
use this [link](https://gitforwindows.org/) to download git. To set up git, click next on everything except the default editor and change it to using visual 
art studio as default editor. As shown below: 

![Image](Screenshot (105).png)

Once your done installing git, open visual art studio and open a new terminal and under the tab powershell or +, change it to git bash. Now your ready to go and 
you should see a $ in the terminal. 

![Image](Screenshot (108).png) 
![Image](Screenshot (110).png) 

## Step 2: Accessing Your CSE 15L Account 

In order to connect to the server, you must access your account. Use this [link](https://sdacs.ucsd.edu/~icc/index.php) to find your account. Enter your PID and
username. Under additional account, you have a course specific account and should start with cs15lwi23, follow by three letter which is different from each student. Click on it and then change your password. Note this will change your password globally and usually take 15 minuites to complete the change. 

![Image](Screenshot (112).png) 
![Image](Screenshot (114).png)

## Step 3: Remote Connecting To UCSD Server 

After completing the password change, head back to visual art studio terminal where we set up git bash terminal. Type in ssh follow by your CS15L account @ieng6.ucsd.edu for example $ssh cs15lwi23avi@ieng6.ucsd.edu which should prompt a message like this one below:

> $ ssh cs15lwi23avi@ieng6.ucsd.edu
> 
> The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
> 
> RSA key fingerprint is ...
> 
> Are you sure you want to continue connecting (yes/no/[fingerprint])? 

Type in yes and will prompt to tell you to enter the password. Note that the password can't be seen when typed. If you type in the right password, but still can't log in then wait and try again. When you logged in, the following message will appear and that means your connected:

![Image](Screenshot (5).png) 

## Step 4: Running Commands 

Now that your connected lets run some commands on the server. Here is a list of commands:
- cd <path> (switch the current working directory)
- cd <~>  (switch to home directory)
- ls <-a> (shows list of all files in the server)
- ls <-lat> (shows list of all files in complete detail) 
- cp </home/linux/ieng6/cs15lwi23/public/hello.txt ~/> (copy a file in a given path)
- cat </home/linux/ieng6/cs15lwi23/public/hello.txt> (prints the content of files of the given path)
- exit (log out the server)

Here is an example of the above commands running: 
![Image](Screenshot (6).png)

