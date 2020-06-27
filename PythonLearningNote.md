# PythonLearningNote
## Python Learning Step by Step
   * Tutorial
      + [Beginner's Guide to Python](https://wiki.python.org/moin/BeginnersGuide)<br>
      + [The Python Tutorial](https://docs.python.org/3/tutorial/)<br>
      + YouTube
        - [Introduction to Computer Science and Programming Using Python | Python Basics | Introduction](https://www.youtube.com/watch?v=Q_itdXI3YeE&list=PLRJdqdXieSHN0U9AdnmwD-9QcR9hmw04d)<br>
        - [6.0001 Introduction to Computer Science and Programming in Python. Fall 2016](https://www.youtube.com/playlist?list=PLUl4u3cNGP63WbdFxL8giv4yhgdMGaZNA)<br>
      + [Python Numpy Tutorial (with Jupyter and Colab)](https://cs231n.github.io/python-numpy-tutorial/)<br>
## Python Development --> [PythonDevelopingNote.md](https://github.com/squirrel-nest/PythonLearningNote/blob/master/PythonDevelopingNote.md)<br>      
## Python 安装
   * Windows
      + Download Page
         - [Python Releases for Windows](https://www.python.org/downloads/windows/)<br>
   * Mac OS
      + Download Page
         - [Python Releases for Mac OS X](https://www.python.org/downloads/mac-osx/)<br>
   * Raspberry 安装请移步 - [RaspberryPiePractice/RaspberryPieDevelopment](https://github.com/huarui0/RaspberryPiePractice/blob/master/RaspberryPieDevelopment)<br>
## Python 环境搭建
   * 参考
      + Youtube
         - [Setting Up VSCode For Python Programming](https://www.youtube.com/watch?v=W--_EOzdTHk&list=PLRVt-3hg7Jl6k8NuKvfX-jeLfe9MxaNnk&index=2&t=18s)<br>
         - [Install Python 3 and PIP on Windows 10](https://www.youtube.com/watch?v=gFNApsyhpKk)<br>
   * 环境变量的设置
      + 参考
         - [Installing packages using pip and virtual environments](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/) - 优先看吧。。。<br>
         - []()<br>
      + 设置
         - Windows
            1. PYTHON_HOME 的设置
               * PYTHON_HOME=E:\Softwares\Python\Python38
            2. PYTHON_SCRIPT 的设置
               * PYTHON_SCRIPT=%PYTHON_HOME%\Scripts
            3. Path 的设置
               * %PYTHON_HOME%;%PYTHON_SCRIPT%;Path
         - MAC OS X
     + 验证
        - pip --version
        - pip --version
        - py -m pip --version
        - 
   * pip - 包管理工具的使用
      + 安装 - Installing pip
         - Windows
            * 随Python一起安装。
         - Linux and macOS
            * 随Python一起安装。
      + 安装与更新
         - py -m pip install --upgrade pip
         
   * Installing virtualenv - 不用这个，已过时
      + >Note: If you are using Python 3.3 or newer, the venv module is the preferred way to create and manage virtual environments. venv is included in the Python standard library and requires no additional installation. If you are using venv, you may skip this section.
      + 安装
   * 12. Virtual Environments and Packages - 用这个
      + 参考
         - [12. Virtual Environments and Packages](https://docs.python.org/3/tutorial/venv.html)<br>
      + 步骤
         1. 12.2. Creating Virtual Environments
            - To create a virtual environment with Command：
               * ```bash
                    python -m venv tutorial-env
                 ```
            - Once you’ve created a virtual environment, you may activate it.
               * Windows
               ```bash
                   tutorial-env\Scripts\activate.bat
            
               ```
               * On Unix or MacOS, run:
               ```bash
                   source tutorial-env/bin/activate
               ```
   * 12.3. Managing Packages with pip
      + 参考
         - [12.3. Managing Packages with pip](https://docs.python.org/3/tutorial/venv.html#managing-packages-with-pip)<br>
## Installing Python Modules
   * 参考
      + [Installing Python Modules](https://docs.python.org/3/installing/index.html#installing-index) - 诸如：pip、venv、以及各种package统称为 Modules<br>
        
## Installing Packages - 与 Installing Python Modules 什么区别？ - Packages是包含在 Modules 中的一个部分
   * 参考
      + [Installing Packages](https://packaging.python.org/tutorials/installing-packages/#requirements-for-installing-packages)<br>
         - >This section covers the basics of how to install Python packages.
           >
           >It’s important to note that the term “package” in this context is being used as a synonym for a distribution (i.e. a bundle of software to be installed), not to refer to the kind of package that you import in your Python source code (i.e. a container of modules). It is common in the Python community to refer to a distribution using the term “package”. Using the term “distribution” is often not preferred, because it can easily be confused with a Linux distribution, or another larger software distribution like Python itself.
## Installing scientific packages
   * 参考
      + [Installing scientific packages](https://packaging.python.org/guides/installing-scientific-packages/)<br>
## Installing packages using pip and virtual environments
   * 参考
      + [Installing packages using pip and virtual environments](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/)<br>

# Samples
## AI
   * [yoyoyohamapi/mit-ml](https://github.com/yoyoyohamapi/mit-ml)<br>
