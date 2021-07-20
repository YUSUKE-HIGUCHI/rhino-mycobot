# rhino-mycobot
unofficial myCobot Package

## Description
Now you can move a digital robot and an actual machine in real time! With 6 axes, you can use Rhino+Grasshopper to link any object with urdf and an actual machine.
![E4ej41dVIAA0QH1](https://user-images.githubusercontent.com/36808163/126074631-a4cc930a-aa1e-41f8-a7f3-36da0dc6f8e4.jpg)
## Demo
[youtube](https://www.youtube.com/watch?v=F2F7dBSZWgw)
## Requirement
| item |  |
| --- | --- |
| OS | Windows10 |
| Arm Robot | myCobot |
| CAD | Rhinoceros7 |
| python | Anaconda3.8 |
## Usage
Connect myCobot and PC with USB-C cable
## Preparation
1. Install pymycobot. See how to install it. https://github.com/elephantrobotics/pymycobot (AtomMain2.5 + pymycobot v2.2.0, or AtomMain2.4 + pymycobot v2.1.2)
1. Install [COMPAS packages](https://compas.dev/compas/latest/installation.html).(This package is made by ETHZ)
  
    The recommended way to install COMPAS is with conda. For example, create an environment named research and install COMPAS.
    ```
    conda config --add channels conda-forge
    conda create -n research python=3.8 COMPAS
    ```
    You could provide a Rhino version number (6.0, 7.0). The default is 6.0.
    ```
    python -m compas_rhino.install -v 7.0
    ```
 
3. Install [COMPAS FAB](https://gramaziokohler.github.io/compas_fab/latest/getting_started.html).(This package is made by ETHZ)

    The recommended way to install COMPAS FAB is with conda. For example, create an environment named research and install COMPAS FAB.
    ```
    conda install -n research python=3.8 compas_fab
    ```
    To make COMPAS FAB available inside Rhino, open the command prompt, activate the appropriate environment, and type the following:
    ```
    python -m compas_rhino.install -v 7.0
    ```
  
## Licence

[MIT](https://github.com/tcnksm/tool/blob/master/LICENCE)
## Author

[yusukehiguchi](https://github.com/YUSUKE-HIGUCHI)
