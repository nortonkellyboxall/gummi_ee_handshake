<a href="#hardware">Click here to learn about the Hardware</a>
------

<a href="#package layout">Click here to learn about the file layout in the package</a>
------

<a href="#startup">Click here to learn about the how to start up the Gummi Arm</a>
------

# Introduction
Gummi_ee_luffy is the end effector package for the gummi arm, everything for this part of the robot is configured in this package however, everything is launched and run from either the gummi_base_luffy package or the gummi_interface package. Below are links to all the packages involved in running the Luffy version of the Gummi Arm.

The packages are as follows:
- [gummi_base_luffy](https://nortonkellyboxall.github.io/gummi_base_luffy/)
- [gummi_ee_luffy](https://nortonkellyboxall.github.io/gummi_ee_luffy/)
- [gummi_head_twodof](https://nortonkellyboxall.github.io/gummi_head_twodof/)
- [gummi_interface](https://nortonkellyboxall.github.io/gummi_interface/)
- [gummi_moveit](https://github.com/nortonkellyboxall/gummi_moveit)
- [gummi_hardware_luffy](https://nortonkellyboxall.github.io/gummi_hardware_Luffy/)

Each of these packages are connected and required to be cloned or forked.

<a id="hardware"> Hardware </a>
======
The end effector package encapsulates the forearm roll and wrist (as well as accompanying links). The wrist joint is a VSA joint, so it contains two dynamixels for actuation and one dyamixel as an encoder. The encoder dynamixel does not have a gearbox and so only measures position, however since it is a dynamixel it allows it to be connected on the same bus as the driving motors. The links are all printed in nylon with the model able to be found in the gummi_hardware_luffy repo. 

<img src="images/Gummi_Forearm.png" alt="Gummi Forearm"/>

<a id = "package layout"> Package layout </a>
======
The file system layout for this package is identical to the gummi_base_luffy package. Refer to that for further information. 

<a id = "startup"> Start Up </a>
======
This package is only referenced in startup. To see how to start up the arm refer to the gummi_base_luffy website.


