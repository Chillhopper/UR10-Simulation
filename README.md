
# Simulation Setup Instructions

Ensure a smooth simulation experience by adhering to the setup instructions and command sequences detailed below.

## Preliminary Steps

Before initiating the simulation, make sure to:

1. Place the `test.world` file in your home directory.
2. Store the building editor models in your home directory. If a models directory already exists, copy the new models into the existing directory.

## Running the Simulation

Follow these steps to launch and run the simulation:

### PROJ4 Command Sequence

Begin by opening a new terminal window and executing the following command:

```
ros2 launch ur_simulation_gazebo ur_sim_control.launch.py
```
```
export TURTLEBOT3_MODEL=waffle_pi && ros2 launch turtlebot3_gazebo assmaze.launch.py
```
```
ros2 run trajectory_executor trajectory_executor
```
```
ros2 topic pub /signal std_msgs/msg/Int32 "data: 42"    //This command is the trigger to activate the simulation, originally designed to be sent by the turtlebot after reaching its goal
```
```
export TURTLEBOT3_MODEL=waffle_pi && ros2 run turtlebot3_teleop teleop_keyboard
```

![image](https://github.com/Chillhopper/UR10-Simulation/assets/68851163/2a2c9feb-55e8-4648-ab47-8f6138ff1f15)
