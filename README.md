# ROS Dependencies

This repository contains the necessary files to set up `rosdep` to install dependencies from Saga Robotics' package repositories.

To set up rosdep for installing the packages, please add a file to your rosdep sources:

``` shell
export RELEASE="public"
echo "yaml https://raw.githubusercontent.com/SAGARobotics/rosdistro/main/rosdep/saga-${RELEASE}.yaml" >> /etc/ros/rosdep/sources.list.d/60-saga.list
```

`rosdep` will now pull the specified YAML so you can install the packages it documents.
