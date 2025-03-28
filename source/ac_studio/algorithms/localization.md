# Localization
Localization is used to provide real-time relative localization information or global localization information, this project includes the following two modules: 
- **msf_localization** is a fusion localization module based on the **ESKF** framework, which can provide relative localization information based only on **imu+wheel** speed and global localization information fused with point cloud localization results. This module can also access other sensor observations for subsequent expansion;
- **lidar_localization** is a point cloud localization module based on point cloud maps, using ceres for optimization, using pcl for point cloud processing.

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
            <td>●</td>
        </tr>
        <tr class="row-even centered-table-text">
            <td>Sensor</td>
            <td colspan="5">AC1</td>
        </tr>
        <tr class="row-odd centered-table-text">
            <td>Mobile Robot</td>
            <td colspan="5">Wheeled Mobile Platform</td>
        </tr>
    </tbody>
</table>

This video demonstrates the real-time localization effect of a mobile wheeled vehicle on supported computing platforms.

<div style="margin-bottom: 24px; position:relative; width:100%; padding-top: 50.28%;" class="video-container">
    <iframe src="https://cdn.robosense.cn/AC_wiki/localization_demo_wiki.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

Video Data: [Mobile wheeled vehicle](https://cdn.robosense.cn/AC_wiki/localization_demo.zip)  
Source Code: [AC1 Locatization](https://github.com/RoboSense-Robotics/robosense_localization)
