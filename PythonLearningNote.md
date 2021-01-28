# PythonLearningNote
## Python Learning Step by Step
   * Tutorial
      + [Beginner's Guide to Python](https://wiki.python.org/moin/BeginnersGuide)<br>
      + [The Python Tutorial](https://docs.python.org/3/tutorial/)<br>
      + [Python 3 Tutorial](https://www.python-course.eu/python3_functions.php)<br>
      + YouTube
        - [Introduction to Computer Science and Programming Using Python | Python Basics | Introduction](https://www.youtube.com/watch?v=Q_itdXI3YeE&list=PLRJdqdXieSHN0U9AdnmwD-9QcR9hmw04d)<br>
        - [6.0001 Introduction to Computer Science and Programming in Python. Fall 2016](https://www.youtube.com/playlist?list=PLUl4u3cNGP63WbdFxL8giv4yhgdMGaZNA)<br>
      + [Python Numpy Tutorial (with Jupyter and Colab)](https://cs231n.github.io/python-numpy-tutorial/)<br>
## Python Development --> [PythonDevelopingNote.md](https://github.com/squirrel-nest/PythonLearningNote/blob/master/PythonDevelopingNote.md)<br>      
## Python 安装 -- 参见 [RaspberryPieDevelopment - Python的安装](https://github.com/huarui0/RaspberryPiePractice/blob/master/RaspberryPieDevelopment.md#installofpython)<br>
   * Windows
      + Download Page
         - [Python Releases for Windows](https://www.python.org/downloads/windows/)<br>
   * Mac OS
      + Download Page
         - [Python Releases for Mac OS X](https://www.python.org/downloads/mac-osx/)<br>
   * Raspberry 安装请移步 - [RaspberryPiePractice/RaspberryPieDevelopment](https://github.com/huarui0/RaspberryPiePractice/blob/master/RaspberryPieDevelopment)<br>
## Python 环境搭建
### Python 默认安装模式环境搭建 - 由随Python一起安装的pip管理工具进行包管理
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
         - MAC OS X - 应该设置成版本可切换。。。
         
     + 验证
        - pip --version
        - pip --version
        - py -m pip --version
        - 
   * pip - 包管理工具的使用
      + 安装 - Installing pip --> 
         - 参见：
            * [RaspberryPieDevelopment - pip的安装](https://github.com/huarui0/RaspberryPiePractice/blob/master/RaspberryPieDevelopment.md#installofpip)<br>
            * <a href="https://github.com/huarui0/RaspberryPiePractice/blob/master/RaspberryPieDevelopment.md#installofpip">查看 RaspberryPieDevelopment - pip的安装</a>
         - Windows
            * 随Python一起安装。
         - Linux and macOS
            * 随Python一起安装。
      + 安装与更新
         - py -m pip install --upgrade pip
   * 12.3. Managing Packages with pip
      + 参考
         - [12.3. Managing Packages with pip](https://docs.python.org/3/tutorial/venv.html#managing-packages-with-pip)<br>
### Anaconda模式环境的搭建
   * 参考
      + [Anaconda介绍、安装及使用教程](https://zhuanlan.zhihu.com/p/32925500) - **按照这篇介绍操作即可**<br>
   * 步骤
      1. 安装
      
      2. 管理conda
         + 打开命令行模式的方法
            - Windows
               * 开始菜单 --> 打开“Anaconda Prompt”
            - Linux/MacOS
               * 打开“Terminal”（“终端”）进行操作。
         + 验证安装结果及版本
            - conda --version
         + 更新conda至最新版本
            - conda update conda
         + 查看conda帮助信息
            - conda --help | conda -h
         + 卸载conda
            - Windows
               * 控制面板 → 添加或删除程序 → 选择“Python X.X (Anaconda)” → 点击“删除程序”
            - Linux/MacOS
               * rm -rf ~/anaconda3
      3. 管理环境
         + 创建新环境
            - conda create --name `<env_name>` `<package_names>`
         + 切换环境
            - Windows
               * activate `<env_name>`
            
            - Linux/MacOS
               * source activate `<env_name>`
         + 退出环境至root
            - Windows
               * deactivate
            - Linux/MacOS
               * source deactivate
         + 显示已创建环境
            - conda info --envs | conda info -e | conda env list
         + 复制环境
            - conda create --name `<new_env_name>` --clone `<copied_env_name>`
         + 删除环境
            - conda remove --name <env_name> --all
         + 导入导出环境 --> 参考：
            - 导出环境
               * conda env export > environment.yaml
            - 导入环境
               * conda env create -f environment.yaml
      4. 管理包
         1. 查找可供安装的包版本
            - ① 精确查找
               + conda search --full-name `<package_full_name>`
            - ② 模糊查找
               + conda search `<text>`
         2. 获取当前环境中已安装的包信息
            - conda list
         3. 安装包
            1. ① 在指定环境中安装包
               - conda install --name `<env_name>` `<package_name>`
            2. ② 在当前环境中安装包
               - conda install <package_name>
            3. ③ 使用pip安装包
            4. ④ 从http://Anaconda.org安装包
         4. 卸载包
            1. ① 卸载指定环境中的包
               - conda remove --name <env_name> <package_name>
            2. ② 卸载当前环境中的包
               - conda remove <package_name>
         5. 更新包
            1. ① 更新所有包
               - conda update --all | conda upgrade --all
            2. ② 更新指定包 - 更新多个指定包，则包名以空格隔开，向后排列。
               - conda update <package_name> | conda upgrade <package_name>
      
         
            
### 12. Virtual Environments and Packages - 用这个
   * 参考
      + [12. Virtual Environments and Packages](https://docs.python.org/3/tutorial/venv.html)<br>
   * 步骤
      1. 12.2. Creating Virtual Environments
         - To create a virtual environment with Command：
            * Linux
            ```bash
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

### Installing virtualenv - 不用这个，已过时
   * >Note: If you are using Python 3.3 or newer, the venv module is the preferred way to create and manage virtual environments. venv is included in the Python standard library and requires no additional installation. If you are using venv, you may skip this section.
   * 安装

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
## Packaging Python Projects
   * 参考
      + [Packaging Python Projects](https://packaging.python.org/tutorials/packaging-projects/)<br>
## 开机启动 Python 应用的方法 - Linux & Raspberry Pi
   * 参考
      + [SkinnyPi - Weight Loss Party - Python Script](https://github.com/jazmy/raspberrypi-skinnypi/README.md)<br>

## Python 的编译
   * 官网参考
      + [PyInstaller Quickstart](http://www.pyinstaller.org/)<br>
   * 参考
      + [https://pyinstaller.readthedocs.io/en/stable/](https://pyinstaller.readthedocs.io/en/stable/)<br>
      + [How to Install PyInstaller](https://pyinstaller.readthedocs.io/en/stable/installation.html#installed-commands)<br>
      
      + 
## Pi 与 步进电机 精准控制
   * 参考
      + [Adafruit 16-Channel PWM / Servo HAT for Raspberry Pi - Mini Kit](https://www.adafruit.com/product/2327)<br>
# Samples
## AI
   * [yoyoyohamapi/mit-ml](https://github.com/yoyoyohamapi/mit-ml)<br>
## Smart Home
   * [pubnub
/
pi-house](https://github.com/pubnub/pi-house)<br>
