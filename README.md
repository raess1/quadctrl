# quadctrl

```
source /opt/ros/melodic/setup.bash
mkdir -p ~/catkin_ws2/src
cd catkin_ws2/
catkin_make
cd src
git clone https://github.com/Derek-TH-Wang/quadruped_ctrl.git
cd ..
catkin_make
```


```
If build fails bevause of eigen (quick fix) add this to line 126

include_directories("/home/k3lso/catkin_ws/src/third-party/eigen3")
## Declare a C++ library
```

