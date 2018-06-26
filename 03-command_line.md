# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > 
* show current working directory path: pwd
* creating a directory: mkdir
* deleting a directory: rm -r
* creating a file using `touch` command: touch 'file'
* deleting a file: rm 'file'
* renaming a file: mv
* listing hidden files: ls -a
* copying a file from one directory to another: cp 'file' 'destination'
* change the access permissions to file system objects: chmod
* kills running process: kill

---

### Q2.  List Files in Unix   

What do the following commands do:  
* `ls`  : lists directory contents
* `ls -a` : includes directory contents whose names start with a dot
* `ls -l`  : lists directory contents in long format
* `ls -lh`  : when used with '-l', uses unit suffixes (Byte, Kilobyte, etc); human-readable format
* `ls -lah`  : lists directory contents using long format, including contents whose names start with a dot, in human-readable format
* `ls -t`  : sort directory contents by time modified
* `ls -Glp`  : enable colorized output, long format, and write a slash after each filename if that file is a directory

> > See above for definitions of each command

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

- `m` : stream output format
- `u`: sorts by time of last access
- `U`: sorts by time of file creation
- `S`: sorts file by size
- `R`: recursively lists subdirectories encountered

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > `xargs` builds and executes command lines from standard input: echo 'one two three' | xargs mkdir (the 'standard input' of 'one two three' is piped to the xargs command which is used as an argument to mkdir, which then creates three directories named 'one', 'two' and 'three'


 

