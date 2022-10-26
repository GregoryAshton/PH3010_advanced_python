# Getting setup with a personal computer

## Introduction
Often when we are taught "programming", we are given a [walled garden or closed platform](https://en.wikipedia.org/wiki/Closed_platform) to work in (e.g. think of [co-calc](https://cocalc.com/) or the lab computers where everything is pre-installed). Walled gardens are great, they are filled with pretty flowers and you rarely find `ModuleNotFoundError`, `TabError: inconsistent use of tabs and spaces in indentation`, or the dreaded `malloc() failed: insufficient memory!`. In a walled garden, the environment you work in is carefully prepared to make it easy to focus on the problem in hand.

Following your degree, wherever your interests take you, you may want to apply the skills that you have learned. The problem is that you can't take a walled garden with you. I mean physically, the lab computers are attached to the desk! Sometimes an employer might give you a new walled garden, but really you need to prepare for the reality of working in open environments and managing the environment yourself.

Of course, many of you will have already been hitting this head on by using your own computer. I suspect you have spent several hours (days?) installing different python installations, WSSL, trying cloud solutions, scanning dead stackoverflow posts all just to fix <WEIRD BUG THAT ONLY YOU HAVE EVER EXPERIENCED> in order to <SUBMIT PYTHON COURSEWORK DUE TOMORROW>. In many cases, the result is a probably something like this [XKCD](https://xkcd.com/1987/):
<p align="center">
<a href=https://xkcd.com/1987/><img src="https://imgs.xkcd.com/comics/python_environment.png" alt="https://xkcd.com/1987" width="300"> </a>
</p>

This page is a help guide on **how to get a sane environment for software development**. It will apply to people with a Windows, Mac, or Linux device. The guide is not the only way to get a sane environment, and probably not the best. Hopefully, this is a useful nonetheless. 

> **Note**
> If you get stuck at any stage in these steps, please post to the Moodle page for the course requesting help or contact me (gregory.ashton@rhul.ac.uk).

## Step 1: Operating System (Windows only)

*The first step applies to Windows only: for Linux and Mac move to step 2.*

Windows is a great OS. But, for software development it has some quirks which we want to avoid. Therefore, we are going to use Windows Subsystem For Linux (WSL). This will provide you with a Linux environment inside your Windows device.

1. Follow the instructions here to install WSL: https://docs.microsoft.com/en-us/windows/wsl/install
2. Follow the instructions here to set up a WSL development environment: https://docs.microsoft.com/en-us/windows/wsl/setup/environment: **You only need to follow these up to and including "Set Up Windows Terminal"**. You can of course follow the other steps, but these are not neccersery.
3. You should now have Windows Terminal installed and be able to open a Terminal in "Ubuntu" (Open the Terminal app and hit the dropdown box then click "Ubuntu").

## Step 2: Installing conda

> **Note**
> Before continuing, you may wish to review the [guide to using the command line](using_the_command_line.md)

Python can be installed in a multitude of ways (and remember that if you use WSL the "python" on your windows machine will be different to the python in WSL. I strongly recommend the use of the `anaconda` python package manager (or `conda` for short). `conda` allows you to control and manage multiple *environments* which can contain different versions of python and python packages. This prevents many headaches. 

If you already use anaconda, or you are happy to use an existing installation. Please ignore these steps. Otherwise, here are the steps to get an anaconda installation and an environment to work in (more detailed instructions can be found [here](https://docs.anaconda.com/anaconda/user-guide/getting-started/)).

1. Follow the instructions for [installing conda on linux for Ubuntu or (i.e. if you are using WSL)](https://docs.anaconda.com/anaconda/install/linux/) or [installing conda on maxOS](https://docs.anaconda.com/anaconda/install/mac-os/). You should install follow the instructions for python 3+.
2. After installing conda, you should be able to run
   ```console
   $ which conda
   ```
   to find out where the program is installed. 
3. In addition, `conda` will change your command-line prompt adding `(base)`. This tells you what conda environment you are in (see more on this in the next section).

## Step 3: Using conda environments

Now that you have `conda` installed, it is time to set up an environment. For each different project, you should create a new project with a sensible name. By doing so, you avoid installed all the packages for all the projects at once and ending up with version clashes, missing dependencies and all the other headaches.

1. Create a new environment. Here it is named `"PH3010"`, but you can name it as you like and it uses `python3.9`:
   ```console
   (base) $ conda create --name PH3010 python=3.9
   ```
2. Activate the environment:
   ```console
   (PH3010) $ conda activate PH3010
   ```

## Step 4: Installing packages 
You can install released python packages using either `conda` or `pip`, typically the package should tell you how this is done (try Googling the package name and "installation"). [Here is an example of the documentation](https://numpy.org/install/) for installing the popular numpy package. **Making sure you have activated the environment you want to use**, the set of commands you would need are:
```console
(PH3010) $ conda install numpy
```
or
```console
(PH3010) $ pip install numpy
```

## Step 5: Running python programs from the command line
To run a program from the command line, you simply write a file names `my_program.py` with contents
```
print("Hello world")
```
Then run it as
```console
(PH3010) $ python my_program.py
```
An example of this is shown in the video above.

## Step 6: Running jupyter notebooks
You can start jupyter notebooks from the command line by running
```console
(PH3010) $ jupyter notebook
```
You should run run this **form the directory you want to store the notebooks in** and **from the conda environment you want to use**. You may also need to install `jupyter` using
```
(PH3010) $ pip install notebook
```

## Step 7: Install git
In this course, you will need to use the tool `git`. This can be installed on Ubuntu with
```console
$ sudo apt install git
```
(Note this will ask for your password, when you type it it is blank to protect it. Just type it out and hit enter). You can also install it using `conda`, e.g.:
```console
(PH3010) $ conda install git
```

## Final steps

* Okay, now that you no how to access the command line on the lab machines, [please follow the guide to getting started with PH3010](https://github.com/GregoryAshton/PH3010_advanced_python/blob/main/guides/PH3010_getting_started).
