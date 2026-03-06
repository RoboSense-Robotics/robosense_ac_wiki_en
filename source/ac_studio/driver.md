# Driver
## rs_driver
rs_driver is the driver for RoboSense robotic sensing products. It is developed in C/C++ and provides low-level driver functions for users. The driver is responsible for fundamental device operations such as configuration, initialization, and calibration, as well as hardware detection and device status management, ensuring efficient sensor operation.
It also provides developer APIs that support sensor configuration, data acquisition, and device control, enabling developers to quickly integrate and use the device.

Source Code: [rs driver](https://github.com/RoboSense-LiDAR/rs_driver/tree/dev_opt_AC2)

## ROS Driver  
For developers using ROS, we provide robosense_ac_driver, a ROS wrapper built on top of rs_driver. It publishes sensor data obtained from rs_driver as ROS messages.
At the same time, it also serves as a reference example for integrating rs_driver into other C++ projects.
This project supports both AC1 and AC2 devices, and is compatible with ROS1 and ROS2.

Source Code: [AC Driver](https://github.com/RoboSense-Robotics/robosense_ac_driver/tree/main)
