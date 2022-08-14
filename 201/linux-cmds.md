[Home](README.md)

# Linux

## About Linux

- Everything in Linux is a file, including folders, devices, documents, pictures, etc
- Commands have a command word, followed by options (dentoed with a "-"), followed by arguments
- Linux is extensionless, meaning specified file extensions in the filename are ignored, and the OS determines the type of file by its contents
- Linux command line has no "undo" feature

## Linux/Terminal Commands

- `pwd` - print working directory; prints out the path of the current directory
- `cd [options] [path]` - change directory; move to a different directory
- `ls [options] [path]` - list; print out the contents of the current or specified directory
    - `-l` - returns contents in long form
    - `-a` - returns all contents, including hidden files (hidden files denoted by period in front of the filename)
- `file` - gives info about what type of file 
- `man [options] [command]` - manual; returns function, usage, options of a given command
    - `-k` - keyword search, for if you don't know the name of the command
    - `n` - after using `man -k`, go to the next matching item
- `mkdir` - creates a new directory
- `rmdir` - removes a directory
- `touch` - creates a new file
- `cp [options] <source> <destination>` - copies a file from one place to another
    - `-r` - recursive; applies to a directory and all contained files
- `mv [options] <source> <destination>` - moves a file from one place to another
- `rm` - removes a file
    - `-r` - recursive; applies to a directory and all contained files
- `CTRL + c` - universal sign for cancel in Linux
- `cat <file>` - concatenate; joins files, but in its most basic usage, can be used to view files
- `less <file>` - used to view longer files
    - arrow keys scroll up/down in the file
    - spacebar jumps to the next page
-

## Vi Text Editor


- vi is a command line text editor
- commands starting off with a colon `:` require you to press enter to execute - all others execute upon pressing a key/combination
- `vi <file>` - opens a file in vi
- files can be opened in insert or edit mode (opened files start off in edit mode)
- `i` enters insert mode
- `ESC` returns to edit mode
- `ZZ` - save and exit
- `:q!` - discard all changes and exit
- `:w` - save file, but don't exit
- `:wq` - save file and exit
- `:set nu` - in edit mode, enables line numbers
- Navigating files in vi:
    - Arrow keys - move the cursor around
    - `j`, `k`, `h`, `l` - move the cursor down, up, left and right (similar to the arrow keys)
    - `^` (caret) - move cursor to beginning of current line
    - `$` - move cursor to end of the current line
    - `nG` - move to the nth line (eg 5G moves to 5th line)
    - `G` - move to the last line
    - `w` - move to the beginning of the next word
    - `nw` - move forward n word (eg 2w moves two words forwards)
    - `b` - move to the beginning of the previous word
    - `nb` - move back n word
    - `{` - move backward one paragraph
    - `}` - move forward one paragraph
- Deleting content:
    - `x` - delete a single character
    - `nx` - delete n characters (eg 5x deletes five characters)
    - `dd` - delete the current line
    - `dn` - d followed by a movement command. Delete to where the movement command would have taken you. (eg d5w means delete 5 words)
- Undoing:
    - `u` - Undo the last action (you may keep pressing u to keep undoing)
    - `U` (Note: capital) - Undo all changes to the current line
- **Note: commands in this section were taken directly from ryanstutorials.net**

## Wildcards