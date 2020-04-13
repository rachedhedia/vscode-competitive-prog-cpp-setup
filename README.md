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
* Create a new .vscode folder in your current directory
* Copy launch.json & task.json inside (either windows or macos ones)
* Launch palette with ctrl+maj+p (cmd+maj+p on mac), and find open keyboard shortcuts
* Paste keybings.json content inside (to have intellij shortcuts)
* Launch palette with ctrl+maj+p (cmd+maj+p on mac)and find Configure user snippets
* Paste cpp.json content in the opened file
* Save all files
* Launch palette (ctrl+maj+p) (cmd+maj+p on mac) and find Reload window **Do not forget or doesn't work**

## Usage
* Create a new file and save it with cpp extension
* Type **algo** in the editor and hit tab to autocomplete
* You'll be provided with a template that you can start filling
* To **build** the code : **ctrl + f9**
* To **run** the code: **shift + f10**
* To **debug** the code: **shift + f9**
* To build and run a **sanitized** version (detect memory corruptions): **shift + f11**


