# Using the command line

In this course, you will need to learn how to use the command line. The command line is a user interface which uses text instead of a mouse.

## Opening the terminal
To access the command line, search for the "terminal" app on Windows, press `ctrl+alt+t` on Ubuntu, or follow [these instructions](https://support.apple.com/en-gb/guide/terminal/apd5265185d-f365-44cb-8b09-71a064a42125/mac) for a Mac. If successfull, this should yield a window with a blinking cursor.

Below, we include a gif for the process in Windows:

<p align="center">
<img src="videos/opening_terminal.gif" alt="sdf" width="500">
</p>

## Terminal commands

To run programs in the terminal, we type the name of the program (also known as an executable), this looks like this
```console
$ <PROGRAM>
```
For example, you can run the program `whoami`
```console
$ whoami
```

> **Note**
> Throughout these notes, a "$" indicates a command run in the terminal

## Navigating the file system

Perhaps the most important tool is getting around. There are two commands that you should remember `cd` to "change directory" (or "change drive") and "ls" to list the contents of the directory:
<p align="center">
<img src="videos/getting_around.gif" alt="sdf" width="500">
</p>


2. There are many cheat sheets online on the full set of commands available, see [this one for example](https://www.git-tower.com/blog/command-line-cheat-sheet/)
3. To get you started, take a look at the following video which contains the commands you'll need for this project:

> **Warning**
> To copy and paste into the terminal, you may need to use `CTRL+Shift+C` and `CTRL+Shift+V` depending on which terminal app you use.


In the following (and elsewhere in these documents), commands that should be run in the command line (or terminal) are pre-pended by "$", for example
```console
$ pwd
```
while commands run in a python terminal will use ">>>":
```python
>>> print("Hello world")
```
Where it is relevant, we will add the conda environment (see below), e.g. `(base) $ pwd`.
