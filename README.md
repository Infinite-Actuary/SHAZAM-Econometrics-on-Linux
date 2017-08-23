# Installing [SHAZAM 11.1.4](http://www.econometrics.com/download/) on Linux Mint 18.1 (64 bit)

> [SHAZAM](http://www.econometrics.com/) is powerfully simple software for econometricians, statisticians, biometricians, sociometricians, psychometricians, politicometricians and all others who analyze data.

## Install the latest stable version of [Wine](https://wiki.winehq.org/Ubuntu) for Ubuntu (currently 2.0.1)

> enable 32 bit architecture

`sudo dpkg --add-architecture i386`

> add the repository

`wget -nc https://dl.winehq.org/wine-builds/Release.key`

`sudo apt-key add Release.key`

`sudo apt-add-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ xenial main'`

> update packages

`sudo apt-get update`

> install stable branch

`sudo apt-get install --install-recommends winehq-stable`

> check version after installation completes

`wine --version`

##  Download the [SHAZAM 11.1.4](http://www.econometrics.com/download/) Desktop Edition (64 bit) Windows Installer File

* `SHAZAM_11_1_4_64_STD_TRIAL.msi` (Standard or Professional Edition)

* During the installation, you might be prompted to also install Mono & Gecko packages

## Run SHAZAM

* In `~/.wine/drive_c/SHAZAM/`, right click `SHAZAMW.exe` and open the windows application with Wine Windows program loader (*Shazamd* & *Shazamq.exe* are command line tools)

* Make sure to choose **Trial SHAZAM** or the program will close

## Getting Started

* SHAZAM Workspaces (*.shw*) are saved to `~WINE_PREFIX/drive_c/users/{user}/Temp/{workspace}`
For example `~/home/carlc/.wine/drive_c/users/carlc/Temp/SHAZDemo` is where you will find all of the SHAZAM data (*.sda* or *.dat*) and SHAZAM scripts (*.sha*) for the `SHAZDemo` workspace.

[Whistler's Guide](http://www.econometrics.com/intro/)
