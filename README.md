# **Install Python** ![Python](img/python_65.png)

A Quick Guide for Installing Python on Common Operating Systems

1. [Install on Windows](#windows-)
2. [Install on MacOS](#macos-)
3. [Install on Linux](#linux-)


## **Windows** ![Windows](img/windows_65.png)
1. If you have not yet installed Python on your Windows OS, then download and install the latest Python3 installer from [Python Downloads Page](https://www.python.org/downloads/)
   - Make sure to check the box during installation which adds Python to PATH. Labeled something like **Add Python 3.X to PATH**

2. Once Python is installed, you should be able to open a command window, type `python`, hit ENTER, and see a Python prompt opened. Type `quit()` to exit it. You should also be able to run the command `pip` and see its options. If both of these work, then you are ready to go.
  - If you cannot run `python` or `pip` from a command prompt, you may need to add the Python installation directory path to the Windows PATH variable
    - The easiest way to do this is to find the new shortcut for Python in your start menu, right-click on the shortcut, and find the folder path for the `python.exe` file
      - For Python2, this will likely be something like `C:\Python27`
      - For Python3, this will likely be something like `C:\Users\<USERNAME>\AppData\Local\Programs\Python\Python37`
    - Open your Advanced System Settings window, navigate to the "Advanced" tab, and click the "Environment Variables" button
    - Create a new system variable:
      - Variable name: `PYTHON_HOME`
      - Variable value: <your_python_installation_directory>
    - Now modify the PATH system variable by appending the text `;%PYTHON_HOME%\;%PYTHON_HOME%;%PYTHON_HOME%\Scripts\` to the end of it.
    - Close out your windows, open a command window and make sure you can run the commands `python` and `pip`

## **MacOS** ![MacOS](img/apple_65.png)
MacOS often comes with a native version of Python, but we likely want to upgrade that and install PIP. The best way to do this is with a MacOS Linux-like package manager called [Homebrew](https://brew.sh/). You can visit the below pages to walk you through installing Homebrew and an updated Python interpreter along with it

1. Open Terminal and run: `xcode-select --install`. This will open a window. Click **'Get Xcode'** and install it from the app store.
2. Install Homebrew. Run: `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
3. Install latest Python3: `brew install python`
6. Once Python is installed, you should be able to open Terminal, type `python`, hit ENTER, and see a Python 3.X.X prompt opened. Type `quit()` to exit it. You should also be able to run the command `pip3` and see its options. If both of these work, then you are ready to go.
  - Additional resources on [Installing Python 3 on Mac OS X](https://docs.python-guide.org/starting/install3/osx/)

## **Linux** ![Linux](img/linux_65.png)
- ### **Raspberry Pi OS** may need Python and PIP
  - ### Install them: `sudo apt install -y python-pip`
- ### **Debian (Ubuntu)** distributions may need Python and PIP
  - ### Install Python and PIP: `sudo apt install -y python-pip`
- ### **RHEL (CentOS)** distributions usually need PIP
  - ### Install the EPEL package: `sudo yum install -y epel-release`
  - ### Install PIP: `sudo yum install -y python-pip`
