# Introduction

## SPECFEM2D on Docker with analytics and visualization tools. 

This library is an utility tool for SPECFEM2D ([official repository](https://github.com/geodynamics/specfem2d)).
The original code of SPECFEM2D requires to compile and use it on only linux based operating system.
This library allow users to use SPECFEM2D on any kind of operating systems including Windows, by using [Docker](https://www.docker.com/).

Thanks to a docker script, users may compile and install SPECFEM2D with only one single command, instead of checking/installing several dependency.

This library includes an user interface which allow to configure the calculation settings, instead of modifying several plane text files.
Some simple post-processing functions, e.g. visualization of signals, making movies etc., is provided as well.
As using Jupyterlab as the base of the user interface, the user may additionally implement the pre/post processing functions for their purposes.