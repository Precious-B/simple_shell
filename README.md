#An implementation of a simple shell in C programming language

##Overview

**SIMPLE SHELL PROJECT**

##Description
A recreation of a shell that takes user input (commands with arguments) and outputs accordingly.

##Basic loop of a shell:

-Read command from standard input.
-Parse commandline string into an executable program and its arguments.
-Run parsed command.

##Environment
Our custom shell was developed and tested on Ubuntu 14.04 LTS via Vagrant in VirtualBox.

##Features
-displays a prompt and waits for user to type a command
-can handle commands with options and arguments
-prompt displays again each time command is executed
-uses PATH variable to find executable command
-if executable is not found, prints an error message and displays prompt again
-includes an exit function that exits the shell
-includes an env built-in that prints the current environment

##Usage

-Enter custom shell by typing "./hsh". You should be prompted with a ($).
-Type a command of your liking and press "Enter".
-Appropriate output will appear.
-Prompt reappears and awaits your next command.
-Exit shell by typing "exit"

##Installation
Clone the repository. Compile the ".c" files. Run executable.

$ git clone https://github.com/Precious-B/simple_shell.git

##Compilation
Enter the following command to compile: $ gcc -Wall -Werror -Wextra -pedantic *.c -o hsh

###Example

Interactive Mode

$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$

Non-interactive Mode

$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$

##Authors
[Bahakae Precious Solomon](https://github.com/Precious-B)
[Teddy Omondi](https://github.com/Teddy0328
