# Using the command line

In this course, you will need to learn how to use the command line. The command line is a user interface which uses text instead of a mouse.

## Opening the terminal
To access the command line, search for the "terminal" app on Windows, press `ctrl+alt+t` on Ubuntu, or follow [these instructions](https://support.apple.com/en-gb/guide/terminal/apd5265185d-f365-44cb-8b09-71a064a42125/mac) for a Mac. If successful, this should yield a window with a blinking cursor.

Below, we include a gif for the process in Windows:

<p align="center">
<img src="videos/opening_terminal.gif" alt="sdf" width="500">
</p>

> **Warning**
> To copy and paste into the terminal, you may need to use `CTRL+Shift+C` and `CTRL+Shift+V` depending on which terminal app you use.

## Terminal commands

To run programs in the terminal, we type the name of the command (also known as an executable or program), this looks like this
```console
$ <COMMAND>
```
For example, you can run the command `whoami` and it will output your username (in my case, `greg`)
```console
$ whoami
greg
```

> **Note**
> Throughout these notes, a "$" indicates a command run in the terminal. Where it is relevant, we will add the conda environment e.g. `(base) $ pwd`.

You can also provide an argument to the command. For example, this command **creates a new directory** (also known as a "drive", or "folder"):

```console
$ mkdir my_project
```
this command **prints out the contents** of the directory "Downloads":
```console
$ ls Downloads
some_file.txt notes.pdf 
```
and this command tells you the disk usage (or size) of a file:
```
$ du Downloads/some_file.txt
8 some_file.txt
```

Sometimes, arguments are provided as "flags", these are prepended with a `--`. For example, adding the `--human-readable` flag to `du` prints out the disk usage along with the units (in this case kilobytes)
```
$ du Downloads/some_file.txt --human-readable
8.0K some_file.txt
```
There are also short names, the `--human-readable` flag can also be given as `-h` for short.

To get help with a command, you provide the `--help` flag (or sometimes just `-h`).

## Navigating the file system

Perhaps the first tool to learn is how to move around. There are three commands to learn: `cd` to "change directory" (or "change drive"), "ls" to list the contents of the directory, and `pwd` to figure out the path to working directory (i.e. where are you). `cd` takes an argument of where to move to this can either be a path relative to where you are (e.g. `cd Downloads/`), or a absolute path from the top of the file system (e.g. `cd /home/greg/Downloads`). If you want to go up one level, you can give `..` instead of the path.

Once you know how to move, you'll then want to create directories. This can be done using `mkdir <DIRECTORY-NAME>`

Here is a quick video showing creating a directory, `cd` into it, checking where you are, and then deleting the directory:

<p align="center">
<img src="videos/getting_around.gif" alt="sdf" width="500">
</p>

## Editing a file

To edit a file, you need to use a **text editor**. In Windows, you can access the easy-to-use `notepad.exe` program from WSL, see the example below:

<p align="center">
<img src="videos/edit_a_file.gif" alt="sdf" width="500">
</p>

On `Ubuntu` you can use `gedit` while on MacOS you can use `TextEdit`. Note that any of these programs take as an argument the filename to edit. This file can already exist (i.e. edit a file) or can not exist, in which case you will create the file.

The commands above use a graphical text editor. There are also command-line text editors. The easiest to use is called `nano`, here is an example of using it:

<p align="center">
<img src="videos/nano.gif" alt="sdf" width="500">
</p>

## Running python

You may be used to running python in an interactive environment like a `jupyter` notebook, but under the hood, python is a command-line program that you can use to run a **script**. A script is simply a text file with python instructions in it and a filename that ends in `.py` (this isn't actually required, but useful).

Here is a video showing how to run a python script which creates a plot of $\sin(x)$.

<p align="center">
<img src="videos/plotting.gif" alt="sdf" width="500">
</p>

> **Note**
> We use the `explore.exe` program to open the file explorer (on Ubuntu this is `nautilus`). You can also open the file directly using an image-viewing program.

Unlike some computer languages, the python language is interpreted, not compiled. This means each line of a script is read, evaluated, then we move on to the next line (this makes it easy to reason about how a program will work!). You can also launch a python interpreter interactively like this:

<p align="center">
<img src="videos/python.gif" alt="sdf" width="500">
</p>

> **Note**
> When we are in the `python` interpreter the prompt is prepended with `>>>`. From hereon out, when we mean for you to run a command in `python`, we will use this to signifyer, for example:
> ```python
> >>> import numpy as np
> ```
> should be run in the python interpreter, not the command line!


## Useful tips

* If you want to re-run a command, press the "up" arrow on your keyboard and it will scroll through the history of commands. You can edit them before hitting enter to rerun.
* If you press `<TAB>`, the command line will try to auto-complete whatever you are typing. Hitting it twice will give a list of possible options.
* There are many cheat sheets online on the full set of commands available, see [this one for example](https://www.git-tower.com/blog/command-line-cheat-sheet/)



