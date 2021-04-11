---
layout: post
title:      "Software Developer and the Holy Grail: Part 2 (What do I install?)"
date:       2021-04-11 04:12:04 +0000
permalink:  software_developer_and_the_holy_grail_part_2_what_do_i_install
---


In my last blog post, I talked about the exciting opportunities that Python offers. I am sure after looking up and researching Python, you are very eager to start writing some code and creating some awesome web applications in Django! Let us take a step back for a second though and talk about installing Python 3 and setting up your local environment. In this post, I will be covering how to start developing in Python for Windows 10. Hopefully, this list of steps will help you quickly and efficiently set up Python for local development. If you are more interested in Python web development or prefer working in a Linux environment, I recommend this document [Microsoft Python Web-Frameworks](https://docs.microsoft.com/en-us/windows/python/web-frameworks), and these documents on setting up WSL2 [Visual Studio WSL Tutorial](https://code.visualstudio.com/docs/remote/wsl-tutorial), [Microsoft Install WSL and WSL2](https://docs.microsoft.com/en-us/windows/wsl/install-win10). 

*(Sidebar) I do apologize if you are on a Mac. I have not installed Python on Mac yet, but I have heard that most Macs come pre-installed with Python. There are also many articles out there that do a better job than I would on Mac Python development. 

1) Check to see if you have Python.

While this might seem obvious, sometimes applications install Python 3 without you knowing about it. To determine if you already have Python 3 on your computer:

-Open command prompt or Windows Terminal (I highly recommend using/installing [Windows Terminal](https://www.microsoft.com/en-us/p/windows-terminal/9n0dx20hk701?activetab=pivot:overviewtab)

-Type in ```py - -version``` in console and hit enter key
 (you can also try ```python - -version``` or ```python3 - -version```)
 
-If it does not produce an output or the first number after Python is a 2, then you need to install Python 3.

2) Install Python 3

-Go to [Python.org Downloads](https://www.python.org/downloads/)

-Select the Download Python 3 button and follow install instructions

*(Python Sidebar) You can also download Python 3 from the Microsoft Store. It uses the basic Python3 interpreter but handles PATH settings so you can avoid the need for admin access. The downside is that this version could be unstable when used with other tools and copies of Python. If you just want to learn Python then you can download from  [Microsoft Store - Python](https://www.microsoft.com/en-us/p/python-37/9nj46sx7x90p?rtc=1&activetab=pivot:overviewtab), but for most developers it’s recommended to download latest version from python.org. 

-Check installation by repeating step one

3) Install Code Editor or Local IDE

-VS Code is nice and beginner friendly but any Code Editor compatible with Python will do!
[VS Code Download](https://code.visualstudio.com/Download)

4) Install Python extension

-For VS Code, select the Extensions icon in the Activity Bar on the left side of Visual Studio Code. Search for Python and select/install the Python extension published by Microsoft. 
5)Select a Python interpreter

-In VS Code, select an interpreter by opening the Command Palette (Ctrl+Shift+P) and type ```Python: Select Interpreter```. Then select the command and choose your desired interpreter. If you need troubleshooting or help choosing an interpreter, check out this document [Visual Studio Python Environments](https://code.visualstudio.com/docs/python/environments).

5) Rejoice and start Pythoning (That is definitely not a word!)

Next week I will go back to what I’ve learned in Python and how it differs from Ruby development, but I think it is important to understand the Python installation process. Properly setting up your local environment will not only save you future headaches, but it will also help create a zen workspace to maximize development efficiency. When you are in the code zone, you don’t want any technical hiccups to interrupt your flow. 

