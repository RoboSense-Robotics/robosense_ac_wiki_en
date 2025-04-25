# Point Cloud and Vision Fusion
Utilizes the built-in IMU of the sensor for motion compensation, maps images and point clouds to each other, and visualizes them.

The computational platforms currently supported by this algorithm are listed in the table below:

<table class="docutils align-default" style="width: 100%;">
    <tbody>
        <tr class="row-even centered-table-text">
            <td rowspan="2">Computing Platform</td>
            <td>General X86 Architecture Computers</td>
            <td>Radxa ROCK5B+</td>
            <td>OrangePi 5 Ultra</td>
            <td>NVIDIA Jetson Orin Nano Super</td>
            <td>NVIDIA Jetson AGX Orin</td>
            <td>D-Robotics RDK X5</td>
        </tr>
        <tr class="row-odd centered-table-text">
            <td>●</td>
            <td>●</td>
            <td>●</td>
            <td>●</td>
            <td>●</td>
            <td>●</td>
        </tr>
        <tr class="row-even centered-table-text">
            <td>Sensor</td>
            <td colspan="6">AC1</td>
        </tr>
    </tbody>
</table>

The following video demonstrates the real-time point cloud coloring effect on the supported computing platforms.

<div style="margin-bottom: 24px; position:relative; width:100%; padding-top: 42.46%;" class="video-container">
    <iframe src="https://cdn.robosense.cn/AC_wiki/postprocess_nezha_wiki.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

Video Data: [Nezha](https://cdn.robosense.cn/AC_wiki/nezha.tar.gz)  
Source Code: [AC1 Color Lidar](https://github.com/RoboSense-Robotics/robosense_ac_postprocess)
