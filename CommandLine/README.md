#SHELL COMMANDS
##

###General purpose:

* ls *(list)*
* pwd *(print working directory)*
* cd *(change directory)*
* mkdir *(make dir)*
* touch *(creates a new file)*
* cp file1 file2 *(copies files or directories)*
* mv name1 name2 *(moves files)*
* rm filename *(remove)*
* echo "Hello" *(echoes the string back to the terminal as standard output)*
* ```>``` *(redirects the standard output to a file, ex: ```$ echo "hello" > hello.txt```)*
* cat filename *(eng. concatenate, outputs the contents of a file to the terminal)*
* ```>>``` *(takes stdin and appends it ot the file on the right)*
* wc *(eng. word count, number of lines, words and characters)*
* sort *(takes the standart input and orders it alphabetically)*
* uniq *(stands for "unique" and filters out adjacent, duplicate lines in a file)*
* grep *(search Globally for lines matching the Regular Expression, and Print them)*
* sed *(stream editor, similar to find and replace)*
* history *(history of commands that were entered in current session)*
* env *(returns a list of the environment variables for the current user)*

###With options:

* ls -a *(list all contents, including hidden files and directories)*
* ls -l *(list all contents of a directory in long format)*
* ls -t *(order files and directories by the time the were last modified)*
* rm -r *(remove recursively)*

### Stardart Values:

* stdin *(standard input)*
* stdout *(standard output)*
* stderr *(standard error)*

### Environment settings:
```~``` represents the user's home directory

```.``` indicates a hidden file.

The name **~/.bash_profile** is important, since thi is how the command line recognizes the bash profile.
$ nano ~/.bash_profile

$ source ~/.bash_profile - activates the changes in **~/.bash_profile** for the current session.

alias pd = "pwd"  (inside .bash_profile) - allows you to create aliases

export USER = "Jane Doe"

$ echo $USER

```PS1``` - is a variable that defines the makeup and style of the command prompt

export PS1 = ">>" - change prompt

### Environment Variable:
* $HOME
* $PATH

### Nano:

```Ctrl + O```  to save file

```Ctrl + X``` to exit nano
