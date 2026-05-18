# Linux Command Line TLDR
A list of commands and other things people (especially new users) may want to know.

All command inputs in this guide will be prefixed by `$` with a name of what to put there. All commands will have examples displayed below the explanation, with the second line of explanation showing command output (if applicable). 

Note that for a lot of commands, the argument --help or -h will show a helptext and list of arguments with explanation.
# Simple Commands
## whoami
`whoami` -- Prints the current user.
```
jane@ubuntuServer:~$ whoami
jane
```
## pwd
`pwd` -- Prints the current working directory.
```
jane@ubuntuserver:~/docs/server/$ pwd
/home/jane/docs/server
```
## cd
`cd $TARGET_DIR` -- Changes your working directory.
```
EXAMPLEUSER@computer:~/games/starsector$ cd /home/EXAMPLEUSER
EXAMPLEUSER@computer:/home/EXAMPLEUSER$
```
Tip: You can also use `cd ..` to go back one directory in the working directory.

## ls
`ls $TARGET_DIR` -- Lists everything in a directory.
```
maria@laptop:~$ ls
Documents  Downloads  Videos  Pictures  starsector  Python
```
```
maria@laptop:~$ ls /home/maria/Documents
doc1.odt  notes.txt
```
Tip: you can add the modifier `-a`, as in `ls -a`. to also show "hidden" files and folders. That is, those with a `.` at the start of their name, such as `.local` or `.steam` or `.bashrc`.

## touch

## mkdir

## rm

## rmdir

## man

## lsblk

## mount

## umount

## lsusb

## lspci

# Advanced Commands

# Application-specific Commands (package managers, etc)

# Bash syntax
(todo: stuff like & and && and |)

# Useful Programs (not preinstalled on most systems)
