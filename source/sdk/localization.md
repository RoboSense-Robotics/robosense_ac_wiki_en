# Localization  
localization is used to provide real-time relative localization information or global localization information, this project includes the following two modules:  
- msf_localization is a fusion localization module based on the **ESKF** framework, which can provide relative localization information based only on **imu+wheel** speed and global localization information fused with point cloud localization results. This module can also access other sensor observations for subsequent expansion.
- lidar_localization is a point cloud localization module based on point cloud maps, using ceres for optimization, using pcl for point cloud processing.  
[Click to learn more](http://10.10.0.20/super_sensor_sdk/ros2_sdk/localization/-/blob/main/README_zh.md) 