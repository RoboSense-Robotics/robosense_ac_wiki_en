# Dense Depth Estimation
By inputting a single frame of image and point cloud, the PromptDA algorithm is utilized to generate a dense depth map based on the image resolution. Below demonstrates the effects exhibited by models of different sizes.

## PromptDA-vitlarge
The computational platforms currently supported by this network are listed in the table below:

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
            <td>○</td>
            <td>○</td>
            <td>○</td>
            <td>○</td>
        </tr>
        <tr class="row-even centered-table-text">
            <td>Model Size</td>
            <td colspan="5">1360M</td>
        </tr>
        <tr class="row-odd centered-table-text">
            <td>Sensor</td>
            <td colspan="5">AC1</td>
        </tr>
    </tbody>
</table>

The following video demonstrates the offline dense depth estimation effect of this network on a supported computing platform for an indoor scene.

<div style="margin-bottom: 24px; position:relative; width:100%; padding-top: 44.12%;" class="video-container">
    <iframe src="https://cdn.robosense.cn/AC_wiki/dense_depth_net_wiki.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

Video Data: [Library](https://cdn.robosense.cn/AC_wiki/dense_depth_net_demo.zip)  
Source Code: [AC1 Dense Depth vitlarge](https://github.com/RoboSense-Robotics/robosense_ac_perception)

## PromptDA-vitsmall
The computational platforms currently supported by this network are listed in the table below:

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
            <td>Model Size</td>
            <td colspan="5">100M</td>
        </tr>
        <tr class="row-odd centered-table-text">
            <td>Sensor</td>
            <td colspan="5">AC1</td>
        </tr>
    </tbody>
</table>

The following video demonstrates the offline dense depth estimation effect of this network on a supported computing platform for an indoor scene.

<div style="margin-bottom: 24px; position:relative; width:100%; padding-top: 44.12%;" class="video-container">
    <iframe src="https://cdn.robosense.cn/AC_wiki/dense_depth_net_radxa.mp4" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height:100%;"></iframe>
</div>

Video Data: [Library](https://cdn.robosense.cn/AC_wiki/dense_depth_net_demo.zip)    
Source Code: [AC1 Dense Depth vitsmall](https://github.com/RoboSense-Robotics/robosense_ac_perception)
