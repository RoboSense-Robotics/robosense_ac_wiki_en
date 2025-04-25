# Object Detection and Recognition
Through the Yolov8 detection model, it recognizes main obstacles (such as people, cars, etc.) in the image, obtaining the category and location of the target.

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
            <td>Model Size</td>
            <td colspan="6">100M</td>
        </tr>
        <tr class="row-odd centered-table-text">
            <td>Sensor</td>
            <td colspan="6">AC1</td>
        </tr>
    </tbody>
</table>

The following video demonstrates the offline pedestrian detection effect on a supported computing platform for an indoor scene.

<div style="margin-bottom: 24px; position:relative; width:100%; padding-top: 72.98%;" class="video-container">
    <iframe src="https://cdn.robosense.cn/AC_wiki/target_detection_radxa_wiki.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

Video Data: [Foreground](https://cdn.robosense.cn/AC_wiki/target_detection_radxa.tar.gz)  
Source Code: [AC1 Pedestrian Detection](https://github.com/RoboSense-Robotics/robosense_ac_perception)
