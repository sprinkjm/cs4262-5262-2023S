# Installation
Author: Jonathan Sprinkle

This file gives installation instructions for cs4262/5262 at Vanderbilt University, Spring 2023.

We're going to be using Jupyter with Python 3.8 for this course. To streamline this process, you should download and install anaconda3 and then proceed to getting the right kernel version.

## Download and install Anaconda3 

Visit https://www.anaconda.com/download/ to download. 

## Create a Python 3.8 virtual environment

From the terminal,

```
conda create -n python38 python=3.8
```

## Activate your environment

From the terminal
```
conda activate python38
```

If you can't remember what you called it

```
conda env list
```

If you want to ensure your get this env all the time, just add it to the end of your `.bashrc`

## Confirm your install
After activating, run

```
python --version
```
It should be 3.8.x

## Install various dependencies

There will be lots of packages you need, here is a great way to get started based on what is in this folder (this will work only if you cloned the repo or downloaded all the files):

Confirm you are in python38 env and have the requirements38.txt file in this folder, then:
```
python3 -m pip install -r requirements38.txt
```
On Windows, you may need to type `python` instead of `python3`
```
python -m pip install -r requirements38.txt
```

## Install the kernel for your jupyter notebook
In some circumstances, your kernel and installed packages may not match what you expect in jupyter lab. To solve this, we install a kernel from within the python38 env (make sure yuo have typed `conda activate python38` first...)
```
python -m ipykernel install --user --name=python38
```
If you have issues with install paths or other versioning, then make sure you select from within Jupyter `Kernel->python38`. Once that kernel starts, you will get the installed package versions as needed.

# Test your setup
Try out your setup on the included files---and confirm whether you are able to see the materials.

