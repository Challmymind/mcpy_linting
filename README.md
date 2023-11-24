# mcpy_linting
This repo was created to provide simple linting and autocompletion for people that don't want to relay on big IDEs.

## So how it works?
These files provide interfaces for LSPs like pyright so you can use them on your favourite IDE or LSP.
It works by adding to or replacing orginal python libraries so LSP can use them for linting and autocompletion instead of system's one.

## How to use?
Okey so to keep things clean and separate, it is important to create virtual env using python venv module.
1. Create venv in your desired place:
``` python -m venv __your_path__```
2. After its done clone this repo somewhere (you can delete it later)
```git clone https://github.com/Challmymind/mcpy_linting```
3. Copy contents of this repo into your venv site-packages
```mv mcpy_linting/* __your_path__/lib/python3.11/site-packages```
__IMPORTANT: your path can differ!__

You are done! Now you can delete mcpy_linting repo!
Now everytime you want open micropython project and have cool linting and autocompletion you must do:
```source __your_path__/bin/activate``` (it just activates your venv)
After you are done with your work just type ```deactivate```.

Quick note that those files are copied from [here](https://github.com/JetBrains/intellij-micropython) and segregated.
As far as i can tell, few files are incomplete and i will try to complete them (for ex. rp2 module)

### Before using:
If you are not familiar with python virtual envoirments i higly recommend to check it's docs before using this method.
[Here is link for your convenience.](https://docs.python.org/3/library/venv.html)
