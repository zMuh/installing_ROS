# installing_ROS


Steps for installing ROS noetic

## 1 - Setup your sources.list
```
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```
## 2 - Setup keys
```
sudo apt install curl # if you haven't already installed curl && curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
```
## 3 - Update Packeges
```
sudo apt update
```
## 4 - Install ROS noetic
```
sudo apt install ros-noetic-desktop-full
```
## 5 - Adding ROS env to bashsource
```
echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc && source ~/.bashrc
```
## 6 - Installing dependencies
```
sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential && sudo apt install python3-rosdep
```
### 6.a - initialize rosedep
```
sudo rosdep init && rosdep update
```
# 7 - Run ROSCORE (master node)
![image](https://img001.prntscr.com/file/img001/v4qMo9MURTGRGikE8RkePg.png)
