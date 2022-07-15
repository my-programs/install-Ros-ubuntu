# Setup-Ros-ubuntu
here i will explain how to install ros on ubuntu

- first we will need to install vmware workstation https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html

- then we install ubuntu iso https://ubuntu.com/download/desktop/thank-you?version=22.04&architecture=amd64

- then we open Vmware , and go to `File > New Virtual Machine Wizard ` 
![image](https://user-images.githubusercontent.com/87250282/179124607-6cc06f2b-7e6e-4441-8433-65c4c46983d6.png)

- select Typical 
![image](https://user-images.githubusercontent.com/87250282/179124708-0162c196-24dc-421c-a74b-1e1f04b86596.png)

- select `installer disc image file (iso)` and upload the ubunto iso file 
![image](https://user-images.githubusercontent.com/87250282/179124737-7c08880d-d61d-48a6-8e45-2d0410bfabe6.png)


- then write Name and passowrd 
![image](https://user-images.githubusercontent.com/87250282/179124877-1c700f7a-5fe6-4022-8ad8-910e3ca315a9.png)


- and select the Location 


- then you can change the disk size by defult it will be 20.0 .


- after setup Ubuntu we open terminal , and for we setup ros we need to write this command on terminal

- `sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'`

- `sudo apt install curl # if you haven't already installed curl
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -`

- `sudo apt-get update`

- `sudo apt-get install ros-kinetic-desktop-full`

- `echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
source ~/.bashrc`

- then we write `roscore`, to make sure that the installation process was successful
