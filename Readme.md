## Setup

To install Anaconda follow the instructions in the following webpage:  
https://www.digitalocean.com/community/tutorials/how-to-install-anaconda-on-ubuntu-18-04-quickstart

Create a conda environment for the PyBullet tutorial:  
```
$ conda create --name pyb_env  
```
Switch to the newly create environment (you will notice the name of the environment on the command line in the extreme left):  
```
$ conda activate pyb_env  
```

Once in the desired environment install the following packages:  
```
$ conda install nb_conda_kernels  
```

Install PyBullet (while in the environment):  
```
$ pip install pybullet  
```


To check the installation launch:  
```
$ python  
```

Inside the python environment import the pybullet library:  
```
>> import pybullet
```
If this command executes without any error then the pybullet installation is successful.  


Check the Jupyter notebook by running the following command in the bash shell:  
```
$ jupyter notebook  
```
This command will provide a URL. Run the URL in a browser (Firefox). If a web page opens up, then the Jupyter software is successfully installed.  



## Agenda 

* Kinematics of a serial-2R manipulator  
    * Forward kinematics  
    * Inverse kinematics  
    * Verification of the FK and IK modules against each other  


* Introduction to PyBullet  
    * How to start a PyBullet session  
    * Settings the simulation parameters in PyBullet  
    *Loading URDF files in PyBullet  


* Torque control of robot state in PyBullet  
    * Obtaining joint information  
    * Setting the control mode (and enabling the motors)  
    * Control of joint torque  


* PID control of robot  
    * Reading the joint state  
    * Determining the control action  
    * Setting the required control torque  


* Point-to-point tracking of end-effector  
    * Obtaining the required joint angles to reach the desired end-effector position  
    * Simulating a PID position control loop to reach the desired end-effector position  


* Simulating an industrial robot (KUKA KR120)  
    * Obtaining the URDF models for the robots  
    * Loading the URDF model  
    * Obtaining the joint information  
    * Controlling the robot joints  



## References
* [PyBullet Quick start guide.](https://usermanual.wiki/Document/pybullet20quickstart20guide.479068914/html)

* [Introduction to PyBullet.](https://alexanderfabisch.github.io/pybullet.html)

* [Kinematics of serial-2R manipulators.](https://ed.iitm.ac.in/~sandipan/files/serialkinematicsv2.pdf)

