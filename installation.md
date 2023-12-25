# Installation Steps
```
git submodule update --init --recursive
DONT_RUN=1 make px4_sitl_default gazebo

source Tools/simulation/gazebo-classic/setup_gazebo.bash $(pwd) $(pwd)/build/px4_sitl_default
export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:$(pwd):$(pwd)/Tools/simulation/gazebo-classic/sitl_gazebo-classic

roslaunch ./launch/xxx.launch
```

