# Lab 1 Report 
## Misha Tavera
---
To demonstrate a bit about the `ls`, `cd`, and `cat` commands' functions and how they work we will look at some examples as we explaing more about them.

##**`ls` Command**
![Image](ls.png)
First, we start here in the terminal with the command `ls` followed by no arguement. The `ls` command is short for the word "list" . This command alone when written in the terminal shows the folders and files are in the current directory you are working in. The working directory that I began with in this was the home directory. As we can see in this image after inputing `ls` the following line prints out `lecture1` which is bolded and blue, this highlighting signifies folders/directories. Looking into the the tab of your folders and files we can confirm that this output does indeed print a list of the folders/files withing your corresponding directory. Not shown in this example, but other plaintext that could appear here would be indication of files. 
![Image](lapathdirectory.png)
From the home directory I input the `ls` command followed by a path to directory `lecture1`
![Image](lspathfile.png)

##**`cd` command**
![Image](cd.png)
For this command I was working in the home directory. `cd` short for "change directory". 
![Image](cdpathdirectory.png)
In this image I use the command `cd` followed by a path to a directory. Specifically, I am starting in the home directory and I used a path to directory `lecture1` as the argument following the `cd` command. This changes my working directory to the inteded directory that we input as the arguement, in this case `lecture1`. After entering this command, we find that the prompt in the following line has changed and now includes our `lecture1` directory. This change in directory can be noted to be done successfully as the prompt now displays your intended directory.
![Image](cdpathfile.png)
##** `cat` Command**
![Image](cat.png)
Once again to execute this command with no arguments I began from the home directory. `cat` standing for the word "concatenate".
![Image](catpathdirectory.png)
I input the command cat followed by the path to directory `lecture1`. The command `cat` does not work with directories therefore it prints a corresponding error message. 
![Image](catpathfile.png)
Shows the context of a file. This would also work for multiple files as it will concatenate, print the contents of each file one after another, of each path to a file that you have written in the the arguement following the `cat` command. Note that the path must correspond to only files in your current working directory and result in error for files outside the current directory. 
