# Using the RHUL Physics Lab machines

The lab computers come pre-installed with all the software needed for this group project. This tutorial will walk you through how to use it.

## Using the command line
While there are Graphical User Interfaces (GUIs) available, here we will learn how to use git from the command line, but first we need to access the command line.
Both Windows and UNIX systems (i.e. linux or Macs) have a command line, but they are different. Since these machines are Windows machines, we'll be using the Windows command line!

There are several ways to access it, but here we will the   Anaconda Prompt
1. Launch the Anaconda Prompt: `Start > Anaconda 3 (64 bit) > Anaconda prompt`
2. Check that git is installed, type `git --version` and check that you get a message like this:

  ![image](https://user-images.githubusercontent.com/1926734/198074651-74010cc8-392a-451a-a049-9291a279adbe.png)

3. You can now review [the guide to the command line](https://github.com/GregoryAshton/PH3010_advanced_python/blob/main/guides/using_the_command_line.md) for some general advice on its use. However, **note that `du` is not available in the Windows command line**. 

## Starting Jupyter notebook

1. Now we want to start the jupyter notebook server, you can launch it from [your "Y" drive](https://intranet.royalholloway.ac.uk/staff/it-services/it-essentials/network-drives.aspx) by running
```
$ jupyter notebook --notebook-dir=Y:
```
This will ensure your work is backed up. 

2. Jupyter will usually start in internet explorer, if you wish to open it in another browser, switch to the "Jupyter Notebook" window (see example below) and copy and paste one of the URLs as instructed.
   <img src="https://user-images.githubusercontent.com/1926734/198066167-e07caec8-5234-4198-9121-64d7729aa3f9.png" width="800" align="middle" />


## Final steps

* Okay, now that you no how to access the command line on the lab machines, [please follow Step 8 and Step 9](https://github.com/GregoryAshton/PH3010_advanced_python/blob/main/guides/getting_setup.md#step-8-getting-a-github-account) in the getting started guide. You may find it useful to browse the rest of the instructions which show how to get python and git installed on your own machine.

   
   
