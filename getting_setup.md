# Getting a sane environment for software development

## Introduction
Often when we are taught "programming", we are given a [walled garden or clased platform](https://en.wikipedia.org/wiki/Closed_platform) to work in (e.g. think of [co-calc](https://cocalc.com/) or the lab computers where everything is pre-installed). Walled gardens are great, they are filled with pretty flowers and you rarely find `ModuleNotFoundError`, `TabError: inconsistent use of tabs and spaces in indentation`, or the dreaded `malloc() failed: insufficient memory!`. In a walled garden, the environment you work in is carefully prepared to make it easy to focus on the problem in hand.

Following your degree, wherever your interests take you, you may want to apply the skills that you have learned. The problem is that you can't take a walled garden with you. I mean physically, the lab computers are attached to the desk! Sometimes an employer might give you a new walled garden, but really you need to prepare for the reality of working in open environments and managing the environment yourself.

Of course, many of you will have already been hitting this head on by using your own computer. I suspect you have spent several hours (days?) installing different python installations, WSSL, trying cloud solutions, scanning dead stackoverflow posts all just to fix <WEIRD BUG THAT ONLY YOU HAVE EVER EXPERIENCED> in order to <SUBMIT PYTHON COURSEWORK DUE TOMORROW>. In many cases, the result is a probably something like this [XKCD](https://xkcd.com/1987/):
<p align="center">
<a href=https://xkcd.com/1987/><img src="https://imgs.xkcd.com/comics/python_environment.png" alt="https://xkcd.com/1987" width="300"> </a>
</p>

This page is a help guide on **how to get a sane environment for software development**. It will apply to people with a Windows, Mac, or Linux device and give an introduction to the [command-line](https://en.wikipedia.org/wiki/Command-line_interface). The guide is not the only way to get a sane environment, and probably not the best. Hopefully, this is a useful nonetheless. 


## Step 1: Operating System (Windows only)

*The first step applies to Windows only: for Linux and Mac move to step 2.*

Windows is a great OS. But, for software development it has some quirks which we want to avoid. Therefore, we are going to use Windows Subsystem For Linux (WSL). This will provide you with a Linux environment inside your Windows device.

1. Follow the instructions here to install WSL: https://docs.microsoft.com/en-us/windows/wsl/install
2. Follow the instructions here to set up a WSL development environment: https://docs.microsoft.com/en-us/windows/wsl/setup/environment: **You only need to follow these up to and including "Set Up Windows Terminal"**. You can of course follow the other steps, but these are not neccersery.
3. You should now have Windows Terminal installed and be able to open a Terminal in "Ubuntu" (Open the Terminal app and hit the dropdown box then click "Ubuntu").

## Step 2: The command line or "terminal"

