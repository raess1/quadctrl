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

```
comment out #import pyquaternion in walking_simulation.py
```


## Add Custom URDF
Add path to custom urdf on line 297 in walking_simulation.py
   ``` 
    boxId = p.loadURDF("/home/k3lso/catkin_ws/src/third-party/k3lso_v3/k3lso.urdf", robot_start_pos,
                       useFixedBase=False)
                       ```
                       
                       
                       
                       ConvexMPCLocomotion.cpp
                       robot_height = 0.42 
                       
                       
                       ConvexMPCLocomotion.h
                         float _body_height = 0.40;
                         float _body_height_running = 0.40
                         float _body_height = 0.40;

   LegController.h
  float stand_target
