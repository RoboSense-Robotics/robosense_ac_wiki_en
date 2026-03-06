# SLAM

This example demonstrates an implementation of a tightly coupled multi-sensor odometry system that integrates LiDAR, vision, and IMU sensors. It is developed based on the VOXEL_SLAM project open-sourced by the HKU-MARS Lab.
The system has been specifically adapted and optimized for the Active Camera, with visual constraints incorporated into the framework. As a result, the odometry system can estimate the pose of the Active Camera in real time and generate a 3D point cloud with color information. 

The video below demonstrates the SLAM performance of an early AC2 engineering prototype in an indoor environment.

<div style="margin-bottom: 24px; position:relative; width:100%; padding-top: 42.46%;" class="video-container">
    <iframe src="https://cdn.robosense.cn/AC_wiki/AC2_SLAM.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

We provide the AC2 adaptation code and default configuration files, enabling developers with an algorithm background to perform joint debugging and development on their own AC2 devices.

🚀 Source Code: [robosense_voxel_odom](https://github.com/RoboSense-Robotics/robosense_voxel_odom)
