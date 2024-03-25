# ROS 2 Cheat Sheet

## [rosdep](https://docs.ros.org/en/humble/Tutorials/Intermediate/Rosdep.html)
Command-line utility for identifying and installing dependencies to build or install a package.

### Steps
1. If it's the first time using `rosdep` on a computer, you must initialize and update the locally cached ROS distribution index.
```sh
sudo rosdep init
rosdep update
```

2. In the top level of your workspace directory, install dependencies.
```sh
rosdep install --from-paths src -y --ignore-src
```
