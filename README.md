# Python Intro
## Linux based & Terminal Focused

A hands-on introduction to Python, from installing it to writing your first programs. Work through the sections in order, and use the notebooks to practice each new concept.

## Who this tutorial is for

This tutorial is for beginners. You don’t need any previous programming experience. It is for those who prefer a written, interactive experience, as well as a focus on cli practice. You can find many videos, online apps, courses etc. but this is the dead-simple toutorial I would have wanted starting out, because I just hate buttons. 

### My personal case for cli focused methods

Buttons seem like the easy way, GUI seems like the easy way, videos and AI seem like the easy way. But the comfort and predictibility that come from basic cli operation become so much easier once you practice. 

For example, to create a file:
cli: `touch "file1"` 
gui: right click>select add file>type in file1

I know, hot keys and usinf copy paste functions can help, and theres no reason to avoid gui entirely. However, the cli is a basic skill tht allows you to understand the logic in a tool agnostic way, it is easier to learn programs when you actually understand the underlying code, but also the structure. 

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
sudo apt update && sudo apt upgrade
```
The pyhton-is-python3 will make sure python points to python3. Updating and upgrading ensures the rest of your system doesn't miss dependencies based on the new install.

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
```
Now you have a root directory (python-intro) and a directory for your notebooks.

## Create a Virtual Environment
To keep alll of the dependancies in order, we will create a virtual environment. 
```
python -m venv .venv
```
I am on Ubuntu, if you are as well, you may get this message:
```
The virtual environment was not created successfully because ensurepip is not
available.  On Debian/Ubuntu systems, you need to install the python3-venv
package using the following command.

    apt install python3.14-venv
```
Generally, you are not the root users, so you need to add sudo. Usually, after adding a package it is a good idea to run an apt upgrade.
```
sudo apt install python3.14-venv
sudo apt update && sudo apt upgrade
```
Type y to accept updates
Once you have created the venv, you might wonder, where is it?
When you ran the cmd, it created several new folders and filesn now you directory should look more like this:
```
python-intro
    --./venv
            +--/bin
            +--/include
            +--/lib
            +--/lib64
            pyenv.cfg
    +--/notebooks
```
### Activate your venv
So, we have the installation done, and we have created our venv. To activate use `source .venv/bin/activate`, you can see this file in the directory. Once you have activated your venv, your cmd line path will show (.venv) in front of it. something like `(.venv) user@computer:~/python-intro$`. To deactivate, simpley type `deactivate` nothing fancy needed.

## Notebook No.1
*Button alert, pick your poison. Jupyter in the browser requires some mods to have dark mode (I am a vitamin-d deficient nerd and this is critical for me), and in my opinion, has more button click-throughs than an editor like Zed or VScode*

### Bash to Editor
Confirm with `pwd` you are still in python-intro, or python-intro/notebooks if you only want to see the notebooks in the editor.
- Zed uses `zed --classic` to launch, but I typed in zed . and it prompted me to add that as an alternate as well
- VScode uses `code . ` to launch


### Bash & browser
If you stayed in the terminal, congratulations, you are super cool! You will need to create the notebook and populate it as a json to open it in the browser. Type `jupyter notebook` to open the jupyter interfac in your browser.




# References
- https://python.land/installing-python
- https://computingforgeeks.com/basic-linux-terminal-shortcuts-cheat-sheet/

## AI Use

```
Copilot Code and Claude chat were used for brainstorming and formatting/proofing materials in this repo. None of the content originated from these programs, and everything was reviewed by me- a human

Conetent generated from AI will be marked (I frequently use it for translation purposes)
```
### MIT License

    Copyright (c) <year> <copyright holder>

    Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
