# Calibration

Calibration of the Active Camera  sensors can be divided into intrinsic calibration and extrinsic calibration.

Intrinsic calibration refers to the internal parameters of the Active Camera, including camera intrinsics (such as focal length and distortion coefficients), as well as the relative poses between the camera and LiDAR, and between the camera and IMU.

Extrinsic calibration determines the pose of the Active Camera relative to other sensors or mechanical platforms. Typical scenarios include calibration of the Active Camera relative to a wheeled mobile platform, or calibration relative to the coordinate frame of a robotic arm.

## Extrinsic Calibration

For extrinsic calibration, we take AC1 as an example. Two typical scenarios are considered: mounting the Active Camera on a wheeled mobile platform and mounting it on the end effector of a robotic arm.
For each scenario, an example implementation of the calibration method is provided.

### AC1 to Wheeled Mobile Platform Extrinsic Calibration

This module provides extrinsic calibration between AC1 and a wheeled mobile platform (only angular calibration). 

The module requires recording two segments of data in advance:
- A segment where the platform moves in a straight line at constant speed
- A segment where the platform rotates at a constant angular velocity around a fixed axis

Following the tool instructions, developers start the calibration program and play back the two recorded datasets sequentially. After calibration is completed, the system outputs the angular extrinsic parameters between the sensor and the wheeled mobile platform.

Data: [AC1 to Wheeled Platform Calibration data](https://cdn.robosense.cn/AC_wiki/calibration_extrinsic.zip)  
Source Code: [AC1 to Wheeled Platform Calibration code](https://github.com/RoboSense-Robotics/robosense_calibration_extrinsic)

### AC1 to Robotic Arm Extrinsic Calibration

This module provides extrinsic calibration between AC1 and a robotic arm (AC1 mounted on the robotic arm end effector).

By combining the end-effector pose of the robotic arm with the point cloud registration results, the calibration is performed using a hand–eye calibration method to estimate the extrinsic parameters between AC1 and the robotic arm.

During calibration, the robotic arm needs to be moved along different directions. After the calibration process is completed, the program outputs the extrinsic parameters between AC1 and the robotic arm end effector.

<div style="margin-bottom: 24px; position:relative; width:100%; padding-top: 56.25%;" class="video-container">
    <iframe src="https://cdn.robosense.cn/AC_wiki/sensor_to_mechanical_arm_en.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

Data: [AC1 to  Robotic Arm Calibration code](https://cdn.robosense.cn/AC_wiki/sensor_to_arm_calib.zip)  
Source Code: [AC1 to  Robotic Arm Calibration code](https://github.com/RoboSense-Robotics/robosense_calibration_extrinsic)

## Intrinsic Calibration

### AC1 Intrinsic Calibration

The AC1 sensor is already calibrated for intrinsic parameters at the factory. The following methods are provided for developers when recalibration is required.

#### Camera Intrinsic Calibration

Pinhole cameras introduce image distortion, mainly including radial distortion and tangential distortion.
This module provides a camera intrinsic calibration tool based on Zhang’s calibration method.

Developers can follow the tool instructions and capture images of a calibration board from different viewpoints (the calibration board can be created using the sample pattern provided in this module) to perform camera calibration. The calibration results provide the camera intrinsic parameters and distortion coefficients required by other modules.

The following video demonstrates a real-time calibration process for camera intrinsics. The main hardware configuration used is:

<table class="docutils align-default" style="width: 100%;">
    <tbody>
        <tr class="row-even centered-table-text">
            <td>Computing Platform</td>
            <td>CPU: Intel® Core™ i5-1135G7 @ 2.40GHz × 8 <br> MEM: 16GB</td>
        </tr>
        <tr class="row-odd centered-table-text">
            <td>Sensor</td>
            <td>AC1</td>
        </tr>
    </tbody>
</table>   

<div style="margin-bottom: 24px; position:relative; width:100%; padding-top: 56.25%;" class="video-container">
    <iframe src="https://cdn.robosense.cn/AC_wiki/camera_intrinsics_calib_en.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

Data: [AC1 Camera Intrinsics Calibration data](https://cdn.robosense.cn/AC_wiki/camera_intrinsics_calib.zip)   
Source Code: [AC1 Camera Intrinsics Calibration code](https://github.com/RoboSense-Robotics/robosense_ac_calibration)

#### Camera to LiDAR Calibration
This module provides a camera–LiDAR calibration tool. It reuses the camera intrinsic calibration checkerboard and estimates the checkerboard pose separately in the camera image and LiDAR point cloud, thereby obtaining the extrinsic parameters between the camera and the LiDAR required by other modules.
During calibration, ensure that the checkerboard is within the FOV of both the image and the point cloud, and keep the AC1 sensor as stable as possible to avoid calibration errors caused by sensor motion.

Data: [AC1 Camera to LiDAR Calibration data](https://cdn.robosense.cn/AC_wiki/camera_lidar_calib.zip)  
Source Code: [AC1 Camera to LiDAR Calibration code](https://github.com/RoboSense-Robotics/robosense_calibration_extrinsic)

#### Camera to IMU Calibration
This module provides a camera–IMU calibration tool. It reuses the camera intrinsic calibration checkerboard to estimate the checkerboard pose from the camera at different orientations. Combined with IMU motion data, a hand–eye calibration method is used to estimate the extrinsic parameters between the camera and the IMU required by other modules.

<div style="margin-bottom: 24px; position:relative; width:100%; padding-top: 56.25%;" class="video-container">
    <iframe src="https://cdn.robosense.cn/AC_wiki/camera2imu_calib_en.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

Data: [AC1 Camera to IMU Calibration data](https://cdn.robosense.cn/AC_wiki/camera_imu_calib.zip)  
Source Code: [AC1 Camera to IMU Calibration code](https://github.com/RoboSense-Robotics/robosense_ac_calibration)

### AC2 Intrinsic Calibration

Calibration code examples for AC2 will be provided here in the future. Stay tuned.

The AC2 sensor is already calibrated for intrinsic parameters at the factory. If developers need to perform recalibration, it can be implemented based on the AC1 intrinsic calibration code.