# First Research Track 2 Assignment 
## Description
The first RT2 assignment consists in replicating the functionalities of the third RT1 assignment (https://github.com/LaRambla20/Repo06_RT1-assignment3.git), by implementing the graphical user interface and some visualization features in a jupyter notebook.  
As far as the visualization task is concerned, the robot's position, the laser scanner's output and the number of reached and non-reached goal should be represented.
## Organization
In order to accomplish the above mentioned task, a ROS package and a notebook have been implemented.  
The first one contains the simulation launch file and two nodes that realize the three modalities for controlling the simulated robot. The notebook instead implements an upgraded GUI and allows the user to visualize some useful pieces of information about the robot's state.  
The ROS package is contained in the github repository named `Repo08_RT2-assignment1_ROSpkg`, whereas the notebook can be found here. In the first case a folder named `docs` is also present: it contains the nodes documentation generated by the tool `Sphinx` starting from the comments in the code (link to visualize this documentation: https://larambla20.github.io/Repo08_RT2-assignment1_ROSpkg/).
## How to run
Before running the notebook it is necessary to have both the simulation and the two external nodes up and running. To this end, follow the steps hereafter mentioned:
* open a terminal window and navigate to the `src` folder of your ROS workspace
* clone the repository https://github.com/LaRambla20/Repo08_RT2-assignment1_ROSpkg in the `src` folder of your ROS workspace
* build your ROS workspace with the command:
```bash
catkin_make
```
* from your ROS workspace folder, execute the following line to open the simulation environment:
```bash
roslaunch rt2_first_assignment final_assignment_sim.launch
```
* open another terminal window and navigate to your ROS workspace folder
* from your ROS workspace folder, execute the following line to run the two external nodes:
```bash
roslaunch rt2_first_assignment modalities_architecture.launch
```
As far as the notebook contained in this repository is concerned, the steps are instead the following:
* open a terminal window and navigate to a folder of your choosing
* clone this repository (https://github.com/LaRambla20/Repo07_RT2-assignment1) in the folder at issue
* from the folder, execute the following line to open Jupyter:
```bash
jupyter notebook --allow-root
```
* once Jupyter has been run in a browser window, click on the notebook named `rt2_assignment1` to open it
* run each block of the notebook
