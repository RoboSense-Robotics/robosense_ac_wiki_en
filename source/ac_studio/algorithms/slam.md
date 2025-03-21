# SLAM  
A multi-sensor tightly coupled odometry system that fuses LiDAR, vision, and IMU.  
Developed based on the FAST-LIVO project open-sourced by the HKU-MARS laboratory, specifically adapted and optimized for Active Camera, it can output the pose of Active Camera in real-time and generate three-dimensional point clouds with color information.

The computational platforms currently supported by this algorithm are listed in the table below:

<table class="docutils align-default" style="width: 100%;">
    <tbody>
        <tr class="row-even centered-table-text">
            <td rowspan="2">Computing Platform</td>
            <td>General X86 Architecture Computers</td>
            <td>Radxa ROCK5B+</td>
            <td>OrangePi 5 Ultra</td>
            <td>NVIDIA Jetson Orin Nano Super</td>
            <td>D-Robotics RDK X5</td>
        </tr>
        <tr class="row-odd centered-table-text">
            <td>●</td>
            <td>●</td>
            <td>●</td>
            <td>○</td>
            <td>○</td>
        </tr>
        <tr class="row-even centered-table-text">
            <td>Sensor</td>
            <td colspan="5">AC1</td>
        </tr>
    </tbody>
</table>

The following videos demonstrates the offline SLAM effects on two scenic areas using supported computing platforms.

<div style="margin-bottom: 24px; position:relative; width:100%; padding-top: 37.87%;" class="video-container">
    <iframe src="https://cdn.robosense.cn/AC_wiki/AC1_2.0_zuopaotai_wiki.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

Video Data: [Climbing Spot](https://cdn.robosense.cn/AC_wiki/zuopaotai.zip)

<div style="margin-bottom: 24px; position:relative; width:100%; padding-top: 41.00%;" class="video-container">
    <iframe src="https://cdn.robosense.cn/AC_wiki/shuichi_slam_demo.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

Video Data: [European architecture](https://cdn.robosense.cn/AC_wiki/shuichi.zip)  
Source Code: [AC1 SLAM](https://github.com/RoboSense-Robotics/robosense_ac_slam)
