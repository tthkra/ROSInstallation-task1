# ROSInstallation-task1


to install ROS, you need first to have a linux based OS. If you are using Windows or macOS, you can install VirtualBox software to run Linux on your device. After that, you need to choose a compatible vesrion of Ubuntu to install. If you are using ROS Melodic, you can use Ubuntu 18.04.6 LTS (Bionic Beaver). Once you have installed Ubuntu, open the terminal and run the following commands:

### 1. set up sources.list 
` sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list' `

### 2. set up keys
` sudo apt install curl `
` curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add - `

### 3. update package lists
` sudo apt update `

### 4. install desktop-full
` sudo apt install ros-melodic-desktop-full `

### 5. set up environment
` echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc `
` source ~/.bashrc `

### 6. dependencies for building packages
` sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential `
` sudo apt install python-rosdep `
` sudo rosdep init `
` rosdep update `


