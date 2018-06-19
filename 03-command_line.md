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
* show current working directory path          : pwd
* creating a directory                         : mkdir
* deleting a directory                         : rm -r "directory name"
* creating a file using `touch` command        : touch "file name"
* deleting a file                              : rm "file name"
* renaming a file                              : mv file.txt newfilename.txt
* listing hidden files                         : ls -a
* copying a file from one directory to another : cp biopic/cleopatra.txt historical/
* navigating to a directory                    : cd "directory name"
* select all files in a satire directory       : cp * satire/

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls` 
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> >
 * ls : lists files in current working directory
* ls -a : lists all contents of a directory, including hidden files and directories
* ls -l : lists all contents in long format
* ls -lh: lists all contents in long format and displays file sizes using more human-friendly units
* ls -lah: lists all contents in long format, displays file sizes uing more human-friendly units, and lists hidden files
* ls -t : sorts entries by time. By default, this option sorts the output by the modification times of files.
* ls -Glp : lists all content in long format, highlights different file types with different colors, and adds '/' after     directory names
---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > 
* ls -u
* ls -t
* ls -d
* ls -l
* ls -a

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > xargs is a command line utility for building an execution pipeline from standard input. A common usage of xargs is with the find command. "find /tmp -mtime +14 | xargs rm" the left sid of this command finds files older than 2 weeks which is piped to the xargs command whichc then removes each file.

 

