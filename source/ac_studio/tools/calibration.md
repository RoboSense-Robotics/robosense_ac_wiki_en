# Calibration
## Camera Intrinsic Calibration
The Active Camera has undergone intrinsic calibration prior to leaving the factory. The following method is provided for developers to recalibrate when necessary.  
Pinhole cameras can cause significant distortion in images, with the main types of distortion being radial and tangential.  
This module offers a camera intrinsic calibration tool based on the principles of Zhang's calibration method.  
Developers can follow the tool's instructions to photograph a calibration target (sample patterns provided in this module can be used for creation) at various angles to calibrate the camera, thereby providing the necessary camera intrinsics and distortion coefficients for other modules.  
The following video provides a real-time demonstration of the calibration field's camera intrinsic calibration, primarily using the hardware configuration of

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
    <iframe src="https://cdn.robosense.cn/AC_wiki/camera_intrinsics_calib.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

Video Data: [AC1 Camera Intrinsics Calibration data](https://cdn.robosense.cn/AC_wiki/camera_intrinsics_calib.zip)   
Source Code: [AC1 Camera Intrinsics Calibration code](https://github.com/RoboSense-Robotics/robosense_ac_calibration)

## Camera to LiDAR Calibration
The Active Camera has been calibrated from camera to LiDAR before leaving the factory. The following method is provided for developers to recalibrate when necessary.  
This module provides a camera-LiDAR calibration tool, reusing the calibration target from the camera intrinsic calibration to estimate the pose of the target for both the camera and the LiDAR separately, in order to provide the extrinsic parameters required by other modules.  
During calibration, please ensure that the target is within the FOV of both the image and the point cloud, and try to keep the AC1 stable to avoid calibration errors due to sensor jitter.

Video Data: [AC1 Camera to LiDAR Calibration data](https://cdn.robosense.cn/AC_wiki/camera_lidar_calib.zip)  
Source Code: [AC1 Camera to LiDAR Calibration code](https://github.com/RoboSense-Robotics/robosense_calibration_extrinsic)

## AC1 Sensor to Mobile Wheeled Platform Extrinsic Calibration
This module provides extrinsic calibration (angle calibration) for the AC1 to a mobile wheeled platform.  
This module requires the prior recording of two sets of data: one set of data for driving at a constant speed along a straight line, and one set of data for rotating at a constant speed around a fixed axis.  
Developers should follow the tool's operational instructions, start the project, and then play these two sets of data in sequence.  
After completing the calibration, the angle extrinsic parameters from the sensor to the mobile wheeled platform are output.  
The translation part needs to be measured by the developer and then filled into the calibration file.

Video Data: [AC1 to Wheel Platform Calibration data](https://cdn.robosense.cn/AC_wiki/calibration_extrinsic.zip)  
Source Code: [AC1 to Wheel Platform Calibration code](https://github.com/RoboSense-Robotics/robosense_calibration_extrinsic)
