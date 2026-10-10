# Python Intro
## Linux based & Terminal Focused

A hands-on introduction to Python, from installing it to writing your first programs. Work through the sections in order, and use the notebooks to practice each new concept.

## Who this tutorial is for

This tutorial is for beginners. You don’t need any previous programming experience.

## What you’ll need

- A PC running Linux
- A terminal or command prompt
- Python 3
- A code editor or notebook environment

## Learning path

1. Install and check Python
2. Set up a project and virtual environment
3. Work through the notebooks in order
4. Complete the practice checklist
5. Try the mini-projects

## 1. Install Python

### Open a terminal

- Open your terminal application.
    -Tip: check your settings> keyboard> shortcuts> launcher settings, for me, I can use `super+x` to launch terminal
    - GUI users look for this icon:

        ![Terminal showing the project files](public/screenshots/terminalicon.png)


### Check whether Python is installed

Try:

```bash
python3 --version
```
For me, this returns:
```bash
Python 3.14.4
```

### Install Python

If you do not have a current install, use:
```bash
sudo apt install python3 python-is-python3
```
The pyhtin-is-python3 will make sure python points to python3.

## Create a directory 
You've installed python! Now what? Well, most people start with jupyter notebooks. They are files with an .ipynb extension, and like all files, you need a place to put them. 

Back to the terminal - you can also use the terminal in VSCode or Zed, if you want a GUI experience. At this point, I normally do. In both, this is how to open the terminal.
```bash
ctrl+shift+`
```
Usually your terminal opens on your home directory under your user. To get beck here at any time you can use `cd ~` cd is how we navigate in the terminal (change directory). If you want your directory (folder) here, then stay here to create it, otherwise navigate to where you want it. 
```bash
cd chosen-folder
cd "folder with spaces"
cd .. --go up a level

mkdir -p python-intro notebooks
cd notebooks
```
Now you have a directory and you are in the notebook directory.
