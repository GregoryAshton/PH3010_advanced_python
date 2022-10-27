# Getting started with PH3010

Hopefully, you have followed the guide to getting set up with either a [personal computer](https://github.com/GregoryAshton/PH3010_advanced_python/blob/main/guides/getting_setup_personal_computer.md) or the [RHUL lab computers](https://github.com/GregoryAshton/PH3010_advanced_python/blob/main/guides/getting_setup_lab_computers.md) already; if not, please return to those guides.

This guide includes the final steps needed to get started with PH3010.

## Step 1: Getting a github account
[Github](https://github.com/) is a website which enables collaborate use of `git` repositories. You'll learn what these means later on, but for now we can say simply that "git is to github what writing in a diary is to twitter". 

In this course, you will need a github account and SSH keys for authentication:

1. Sign up for github for free [here](https://github.com/join).
2. As a student, you can also take advantage of the [github student developer pack](https://education.github.com/pack) which provides access to free training and software.
3. Finally, you need to add SSH keys [as described here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

## Step 2: Getting the notebooks for this course
Once you have completed all the steps above, you are ready to download the course materials and get started using the following commands.
These should be entered into a command line with git and jupyter installed.
If you are using a personal computer, open a terminal. If you are using the lab computers, the terminal is the "Anaconda Prompt".

0. Open a terminal and decide where you want to download the course materials. For those working on lab machines, you may wish to run `cd Y:` to use the University Y drive. Furthermore, you may wish to organise yourself and create a directory to store the course materials together.
1. Clone the course materials: 
    ```
    $ git clone https://github.com/GregoryAshton/PH3010_advanced_python.git
    ```
2. Enter the directory:
    ```
    $ cd PH3010_advanced_python
    ```
3. Install the requirements:
    ```
    $ pip install -r requirements.txt
    ```
Note that `requirements.txt` is a text file containing all the modules used in the notes. You can also install these individually using `pip install numpy` for example. But, the `-r` flag and the file tell `pip` to install everything all at once.

4. Start a jupyter notebook.
    ```
    $ jupyter notebook
    ```

5. Step 3 will open the notebook in a browser. If it does not, copy/paste the links given in the terminal into a browser or read the error message.

Here is a quick video showing the essential steps needed. If these steps don't work for you, revisit the guides to check that everything is installed.

<p align="center">
<img src="videos/getting_started.gif" alt="sdf" width="600">
</p>
