# Lab 1 Report 
## Misha Tavera
---
  To demonstrate a bit about the `ls`, `cd`, and `cat` commands' functions and how they work we will look at some examples as we explaing more about them. A very simple overview of what each of these cammands do is as follows. The  `ls` command will print a list of your files and folders. The `cd` command will change the directory in which you are working in. Finally the `cat` command will print the contents of a file. To better understand these commands it is also important to know what about paths, which can be described as what goes after a command that specify files or directories. 

## `ls` Command

![Image](ls.png)

First, we start here in the terminal with the command `ls` followed by no arguement. The `ls` command is short for the word "list" . This command alone when written in the terminal shows the folders and files are in the current directory you are working in. The working directory that I began with in this was the home directory. As we can see in this image after inputing `ls` the following line prints out `lecture1` which is bolded and blue, this highlighting signifies folders/directories. Looking into the the tab of your folders and files we can confirm that this output does indeed print a list of the folders/files withing your corresponding directory. Not shown in this example, but other plaintext that could appear here would be indication of files. 


![Image](lapathdirectory.png)

In this example, from the home directory I input the `ls` command followed by a path to directory `lecture1`. This result is still successful despite currently working in the home directory. This is because the `ls` command followed by a path to a directory is able to print out a list of the files/folders in the specified path to directory despite not being in it. In fact it will only print out the folders/files in the directory specified. As we can see the `lecture1` folder is not printed here like in the last example because it is located in the home directory not the `lecture1` directory that we have specified. 


![Image](lspathfileee.png)
In this image, as indicated by the prompt I am in the `lecture1` directory. I once again use the `ls` command but this time followed by a path to a file in my directory. The result here is an output of `README`, the arguement we just used. This is successfully executed and listing the files, in this case `README`.

## `cd` Command

![Image](cdpathdirectory.png)

 For this command I was working in the home directory. The `cd` command is short for "change directory". In this image I use the command `cd` followed by a path to a directory. Specifically, I am starting in the home directory and I used a path to directory `lecture1` as the argument following the `cd` command. This changes my working directory to the inteded directory that we input as the arguement, in this case `lecture1`. After entering this command, we find that the prompt in the following line has changed and now includes our `lecture1` directory. This change in directory can be noted to be done successfully as the prompt now displays your intended directory.

 ![Image](cdd.png)

   As indicated by the prompt, here I am beginning in the `~/lecture1/messages` directory. If I only input the command `cd` followed by no argument I am returned to the home directory. This command alone followed by no argument will return us to the home directory no matter the directory we are currently working in. We can once again confirm that we are in the home directory as we look at the changed prompt where the `~` indicates as such. 


![Image](cdpathfilee.png)

Here, I once again begin in the `lecture1` directory only now I give a path to a file in this directory, `README`. As mentioned previously the `cd` command is short for "change directory" and is meant to do as such. Therefore, when given a path to a file this command will not work resulting in the error message shown in the image. In short, the `cd`  command does not work with paths to files as it is only inteded to work between changing directories. 

## `cat` Command

![Image](catpathfilee.png)

  From the `lecture1` directory I use the command `cat`, short for "concatenate", followed by a path to file `Hello.java`. Then, the contents of the file are successfully printed out. when this command is put into the terminal with a path to a file it will simply return the contents of that file. It is important to note that the path must correspond to only files in your current working directory or it would result in an error for any files outside the current directory.  This would also work for multiple files as it will concatenate, print the contents of each file one after another, of each path to a file that you have written in the the arguement following the `cat` command. 

![Image](catt.png)

  Once again from the `lecture1` directory I use the `cat` command only with no aurgument this time. This then resulted in a completely blank line (no prompt) and repeated back my input until using ctrl + c. This happens because with no arguement after the command there is no file for it to return. So, nothing is returned initially as there is not file to print and whatever is typed after is simply repeated back because our commands were being typed into the `cat` command.


![Image](catpathdirectoryy.png)

  Here, I start in the `lecrure1` directory and use the `cat` command follwed by a path to the directoy `messages` which is a folder within our current working directory. As we have seen the `cat` command works by printing the content of a given file. However, this command cannot do this with paths to directories. Which can be confirmed by the error message we recieve when we attempt to use a path to the directory `messages`. In short, the command `cat` only works with paths to files and will not work with paths to directories therefore, it prints a corresponding error message. 



