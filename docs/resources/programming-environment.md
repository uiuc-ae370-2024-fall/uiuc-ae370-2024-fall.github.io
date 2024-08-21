---
layout: page
title: Programming Environment
permalink: /resources/programming-environment/
nav_order: 4
parent: Resources
---
# Setting up your programming environment

You will need the following in your programming environment for this course:

- Programming language: Python 3
- Code editor: Up to you

## Install Python 3

We strongly recommend that you install Python using Anaconda (see steps below). If you already have Python and/or Anaconda installed, you may want to consider uninstalling your existing Python and/or Anaconda installations and following these steps (or at least skip to the steps that test your Anaconda and Python installations).  **Make sure you have Python 3 if you are using an existing installation.**

1. Go to <https://www.anaconda.com/products/individual> and download the appropriate installer.

1. Open the installer and go through the installation process.

    - Windows: we recommend that you check the box that adds Anaconda to your PATH variable (even though the installer will say this option is not recommended).

    - macOS: we recommend the default installation options.

1. After finishing installation, test that Anaconda was properly installed.

    1. Open the command prompt (Windows) or terminal (macOS).

        - Windows: you can open the command prompt by searching for "cmd" in the start menu.

        - macOS: you can open the terminal by pressing Command-Space bar and searching for "terminal" in Spotlight Search.

    1. Type the following in the command prompt (Windows) or terminal (macOS) and hit `Enter`.

            $ conda

    1. You should see something like this:

            usage: conda-script.py [-h] [-V] command ...

            conda is a tool for managing and deploying applications, environments and packages.

            Options:

            positional arguments:
            command
                clean        Remove unused packages and caches.
            ...

1. Also test that Python was properly installed.

    1. Open the command prompt (Windows) or terminal (macOS).

    1. Type the following in the command prompt (Windows) or terminal (macOS) and hit `Enter`.

            $ python --version

    1. You should see `Python 3.X.X`. For example, my installation shows:

            Python 3.9.7

## Install a Code Editor

You should use whatever code editor you are comfortable with. Some popular options are:
  - [Jupyter Notebook App](https://jupyter.org/). The Jupyter Notebook App is an easy way to work with Python and should already be installed through Anaconda.

  - [PyCharm](https://www.jetbrains.com/pycharm/). PyCharm is a popular IDE that is pretty easy to use out of the box. The free version is fine, though student licenses are available for the pro version [here](https://www.jetbrains.com/community/education/#students).

  - [VS Code](https://code.visualstudio.com/). VS Code is another popular IDE that requires a little more set up than PyCharm but it is free and supports multiple code languages (Huy uses this).

  - [Atom](https://atom.io/). Atom is a text editor that is a lightweight alternative to full IDEs with plug-ins available to give more features than simple Jupyter notebooks.

## Opening IPython (Jupyter) Notebooks

You can open IPython (Jupyter) notebooks (e.g., `.ipynb` files) using your code editor of choice.

For example, you can use the Jupyter Notebook App (more details [here]( https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/execute.html)) by clicking the Jupyter Notebook icon (Windows) or typing the following in the command prompt (Windows) or terminal (macOS):

```
$ juptyer notebook
```