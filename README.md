# rhino-mycobot
unofficial myCobot Package

## Description
Now you can move a digital robot and an actual machine in real time! With 6 axes, you can use Rhino+Grasshopper to link any object with urdf and an actual machine.
![E4ej41dVIAA0QH1](https://user-images.githubusercontent.com/36808163/126074631-a4cc930a-aa1e-41f8-a7f3-36da0dc6f8e4.jpg)
## Demo


https://user-images.githubusercontent.com/36808163/126579699-ad6c878a-de22-4357-964a-f25803434101.mp4


## Requirement
| item |  |
| --- | --- |
| OS | Windows10 |
| Arm Robot | myCobot |
| CAD | Rhinoceros7 |
| python | Anaconda3.8 |
## Preparation
Open the command prompt

1. Install pymycobot. See how to install it. https://github.com/elephantrobotics/pymycobot (AtomMain2.5 + pymycobot v2.2.0, or AtomMain2.4 + pymycobot v2.1.2)
  
    Check [karaage's zenn book](https://zenn.dev/karaage0703/books/3be6bad93b0c8e) for a more detailed explanation.(in Japanese)
1. Install [COMPAS packages](https://compas.dev/compas/latest/installation.html).(This package is made by ETHZ)
  
    The recommended way to install COMPAS is with conda. For example, create an environment named research and install COMPAS.
    ```
    conda config --add channels conda-forge
    conda create -n research python=3.8 COMPAS
    ```
    You could provide a Rhino version number (6.0, 7.0). The default is 6.0.
    To make COMPAS FAB available inside Rhino and type the following:
    ```
    python -m compas_rhino.install -v 7.0
    ```
 
1. Install [COMPAS FAB](https://gramaziokohler.github.io/compas_fab/latest/getting_started.html).(This package is made by ETHZ)

    The recommended way to install COMPAS FAB is with conda. For example, install COMPAS FAB in environment named research.
    ```
    conda install -n research python=3.8 compas_fab
    ```
    To make COMPAS FAB available inside Rhino and type the following:
    ```
    python -m compas_rhino.install -v 7.0
    ```
## Usage
If you have a mycobot, connect myCobot and PC with USB-C cable. If you don't, please ignore this.

1. Download mycobot_artist_grasshopper.ghx and mycobot to any folder.
2. Start rhinoceros, grasshopper, and open mycobot_artist_grasshopper.ghx
3. Click 'Load' button, so you can see the model of mycobot.
![image](https://user-images.githubusercontent.com/36808163/126385545-cae1eed2-320d-4ccf-b818-9d5a90a877e0.png)

If you have a mycobot, make mycobot component enable. So, the mycobot will move!
## Licence

[MIT](https://github.com/tcnksm/tool/blob/master/LICENCE)
## Author

[yusukehiguchi](https://github.com/YUSUKE-HIGUCHI)
## Thanks

[Gramazio Kohler Research](https://github.com/gramaziokohler/workshop_tokyo_2020) for grasshopper model

[Tiryoh](https://github.com/Tiryoh/mycobot_ros) for urdf file
