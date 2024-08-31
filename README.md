## Setup Python

Prefer using [miniconda](https://docs.anaconda.com/miniconda/) to install, manage Python environments. You need to download `miniconda` [here](https://docs.anaconda.com/miniconda/miniconda-install/)

After correctly setting up `miniconda`, you are able to use it from ternimal

```
# Show version of installed conda
conda --version
```

Create a Python environment for this repository

```
# Create a Python version 3.10 at `.venv` directory from root of this project
conda create --prefix ./.venv python=3.10
```

_Notice that this environment is a virtual environment (venv), might be used, should be used only by this project. This process ensures that there is no packages, libraries messing or conflicting between projects._

To use this virtual environment (venv), you need to activate it

```
# Activate Python venv for current terminal session
conda activate ./.venv
```

_This activation is only available in a terminal session, if you reopen or reload terminal, you will need to reactivate the `venv`_

## Setup Coding

You need somehow to write the code and run it. There are 3 common ways to work with Python (or ML) code
- Interactive terminal
- Python script with VSCode (or any code editor)
- ML Notebook (Jupiter Notebook or Google Colab)

### Interactive terminal

Open a terminal, and ensure that there is a global Python environment or an activated venv. Run the command

```
python
```

Terminal will show an interactive Python, you can code and run Python line by line

```
Python 3.10.14 (main, May  6 2024, 14:42:37) [Clang 14.0.6 ] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> a = 1
>>> b = 2
>>> c = a + b
>>> print(c)
3
>>>
```

### Python script with VSCode

[VSCode](https://code.visualstudio.com/) is a code editer to write the code, you need to install it [here](https://code.visualstudio.com/download)

After installing VSCode, open it with a project directory (might be this project) or any directory

Create a python file `main.py`. You can do it either by VSCode interface or VSCode integrated terminal or external terminal.

By terminal

```
# Create a Python script file
touch main.py
```

Put some code to the script `main.py`

```
a = 1
b = 2
c = a + b
print("Hello world", c)
```

Run it by the terminal
```
python main.py
```

And it shows

```
Hello world 3
```

_You can run Python code by VSCode's built-in features or extensions, but the above running is exactly how the Python code is run behind any scene. The code is run by the Python environment which you activated, you need to be aware about it. Sometimes, you might want to check which Python you are using, by running `which python` in terminal_





