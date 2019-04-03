# Installation and configuration

## How to setup this library on your computer.  

This library is developed for using with docker system, thus firstly few configuration of the system is required for Windows 10 users.  
Users with other operating systems e.g. may skip the step 0 below and may start from step 1.  


## 0. Initial configration for docker. (only for Windows)
Windows need to be configured as following the official [reference](https://docs.docker.com/docker-for-windows/install/). Here is a summary.  
- at first *visualization technology (VTx)* need to be enabled from BIOS setup menue.  
- Then after Hyper-V needs to be enabled also.  
Please refer [this blog](https://www.nextofwindows.com/how-to-enable-configure-and-use-hyper-v-on-windows-10) to know how to do them.
 
## 1. Install Docker
Download and install Docker (or Docker-ce for Windows) in your computer. Download link and instructions can be found [here](https://www.docker.com/get-started) depending on your OS type.  
It is necessary to create an user account of Docker site.  
During the installation, please *DO NOT* check the option to use windows container.  

## 2. Install Gmsh  
From `http://gmsh.info/bin/Windows/gmsh-4.1.4-Windows32.zip` download the gmsh executable.

---
For the installation of this library, there are two ways for it and users may select from them depending on their environment.  

- for the users who may connect to internet and download/install any softwares without limitation, use of git may be the best way to get the latest updates of the library as this library is under actively developed situation. For installing in this way, please follow the guidance with numbering `A-*`.

- for the user whose environment has limitations on downloading/installation of numerical libraries, user may install this library with `docker import` function. Please follow `B-*` instractions to do so.
  
---
## A-1. Install Git
This is an utility for controlling the version of library codes.
As this library is under development state, user may be required to update the code using git, thus please install it from [Git official site](https://git-scm.com/downloads).


## A-2. Download the code of library and initial run.

1. On your terminal (or Powershell for Windows), run the command below to download the codes of this library by:
    ```bash
    git clone https://github.com/mnagaso/SPECFEM2D_on_docker_with_boat
    ```
2. then enter into the directory which was downloaded now:
    ```bash
    cd SPECFEM2D_on_docker_with_boat
    ```
    `cd` (change directory) command is used for changing the current directory in the Powershell window.  

3. start docker daemon if the daemon is not running. (please see the tutorial page for details.)
4. run the command below to initialize the docker container
   ```bash
   docker-compose up
   ```  
   this may take about few minutes for the initial setup. Windows users will be asked to share c disk with docker. please allow it.

   In the case where the installation process stops with an error, please retry the same command above.

   Sometimes, standard output on Powershell window stops by unknow reason. In this case, you just need to tap `enter` key and the standard output restarts.

---
## B-1. Import an entire docker image.
this part will be written after testing


This script does not support docker toolbox (docker system working with virtual box).