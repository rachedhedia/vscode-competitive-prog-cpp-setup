## Introduction

This repository contains Visual studio code configuration files to get started with competitive programming using C++. It covers both Windows and MacOs

## Setup
### Windows specific
* Install visual studio code
* Install Remote - WSL extension (vscode extension)
* Install C/C++ extension
* Install ubuntu for windows (WSL)
* Open an Ubuntu terminal and install the followings:
```
sudo apt-get update
sudo apt-get install build-essential gdb
```
* start visual studio code, ctrl+maj+p to open palette and launch WSL - new window
* Open extensions pane, on C/C++ extension, click install on wsl

### Common for Windows and MacOs
* install conan:
```
pip install conan
```
* edit ~/.conan/profiles/default and configure it accordingly (cf: https://gist.github.com/rhedia/e5113da754d1ae0639b3a4bf58ac020e for MacOs configuration)
* launch init-conan.sh script
* Create a new .vscode folder in your current directory
* Copy launch.json & task.json inside (either windows or macos ones)
* Launch palette with ctrl+maj+p (cmd+maj+p on mac), and find open keyboard shortcuts
* Paste keybings.json content inside (to have intellij shortcuts)
* Launch palette with ctrl+maj+p (cmd+maj+p on mac)and find Configure user snippets
* Paste cpp.json content in the opened file
* Save all files
* Launch palette (ctrl+maj+p) (cmd+maj+p on mac) and find Reload window **Do not forget or doesn't work**

**Note**
When using gtest includes, you can have error displayed.  
A pop up will allow you to update the include directories used by intellisense.  
Add the include directory specified in **conan-build/conanbuildinfo.txt**, include section to the **c_cpp_properties** file created by vscode.

## Usage
* Create a new file and save it with cpp extension
* Type **algo** for file with main or **algot** for file with test in the editor and hit tab to autocomplete
* You'll be provided with a template that you can start filling
* To **build** the code : **ctrl/cmd + f9**
* To **run** the code: **shift + f10**
* To **debug** the code: **shift + f9**
* To build and run a **sanitized** version (detect memory corruptions): **shift + f11**


