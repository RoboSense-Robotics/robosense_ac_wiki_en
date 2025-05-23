# Hardware Ecosystem
## Computing Platforms

The table below lists some computing platforms compatible with Active Camera, along with the supported SDK applications and system images. 

These system images include the dependencies required for compiling and running the supported SDKs.

<table class="docutils align-default">
    <tr class="centered-table-text">
        <td style="font-weight: bold;" colspan="2">Computing Platform</td>
        <td style="font-weight: bold;">General x86<br> Architecture Computers</td>
        <td style="font-weight: bold;">Radxa ROCK5B+</td>
        <td style="font-weight: bold;">OrangePi 5 Ultra</td>
        <td style="font-weight: bold;">NVIDIA Jetson<br> Orin Nano Super</td>
        <td style="font-weight: bold;">NVIDIA Jetson AGX Orin</td>
        <td style="font-weight: bold;">D-Robotics RDK X5</td>
    </tr>
    <tr class="centered-table-text">
        <td colspan="2">SOC</td>
        <td>-</td>
        <td>Rockchip RK3588</td>
        <td>Rockchip RK3588</td>
        <td>Jetson Orin Nano<br>8GB module</td>
        <td>Jetson Orin</td>
        <td>Sunrise 5</td>
    </tr>
    <tr class="centered-table-text">
        <td colspan="2">CPU</td>
        <td>Intel® Xeon(R)<br> Gold 6230R CPU @<br> 2.10GHz x 104</td>
        <td>8-Core 64-bit Processor<br> 4 x Cortex-A76@2.4GHz<br> 4 x Cortex-A55@1.8GHz</td>
        <td>8-Core 64-bit Processor<br> 4 x Cortex-A76@2.4GHz<br> 4 x Cortex-A55@1.8GHz</td>
        <td>6 x Cortex-A78@2.4GHz</td>
        <td>12 x Cortex-A78AE@2.2GHz</td>
        <td>8 x Cortex-A55@1.5GHz</td>
    </tr>
    <tr class="centered-table-text">
        <td colspan="2">MEM</td>
        <td>64 GB</td>
        <td>16 GB LPDDR5</td>
        <td>16 GB LPDDR5</td>
        <td>8 GB LPDDR5</td>
        <td>64 GB LPDDR5</td>
        <td>8 GB LPDDR4</td>
    </tr>
    <tr class="centered-table-text">
        <td colspan="2">AI Computing Power</td>
        <td>NVIDIA A40<br> (299.3 TOPS@INT8 GPU)</td>
        <td>6 TOPS@INT8 NPU</td>
        <td>6 TOPS@INT8 NPU</td>
        <td>67 TOPS@INT8 GPU</td>
        <td>275 TOPS@INT8 GPU</td>
        <td>10 TOPS@INT8 BPU</td>
    </tr>
    <tr class="centered-table-text">
        <td rowspan="12">Supported <br> SDKs <sup>1</sup> </td>
    </tr>
    <tr class="centered-table-text">
        <td>Driver</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
    </tr>
    <tr class="centered-table-text">
        <td>Data Acquisition</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
    </tr>
    <tr class="centered-table-text">
        <td>Monitoring</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
    </tr>
    <tr class="centered-table-text">
        <td>Calibration</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
    </tr>
    <tr class="centered-table-text">
        <td>Point Cloud & Vision Fusion</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
    </tr>
    <tr class="centered-table-text">
        <td>Localization</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
    </tr>
    <tr class="centered-table-text">
        <td>SLAM</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
    </tr>
    <tr class="centered-table-text">
        <td>3D Gaussian Splatting</td>
        <td>●</td>
        <td>○</td>
        <td>○</td>
        <td>○</td>
        <td>●</td>
        <td>○</td>
    </tr>
    <tr class="centered-table-text">
        <td>Dense Depth Estimation</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>○</td>
    </tr>
    <tr class="centered-table-text">
        <td>Object Detection & Recognition</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
    </tr>
    <tr class="centered-table-text">
        <td>Semantic Segmentation</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
        <td>●</td>
    </tr>
    <tr class="centered-table-text">
        <td colspan="2">System image/<br>SDK Environment Container <sup>2</sup> </td>
        <td>
            <a href="https://github.com/RoboSense-Robotics/ros2_ac_sdk_infra/tree/main/tools/cross_compilation">
                SDK Environment<br>Container
            </a>
        </td>
        <td>
            <a href="https://github.com/RoboSense-Robotics/robosense_ac_ros2_sdk_infra/blob/main/tools/system_image/Radxa_Image_Readme.md">
                System image<br>installation description
            </a>
        </td>
        <td>-</td>
        <td>
            <a href="https://github.com/RoboSense-Robotics/robosense_ac_ros2_sdk_infra/blob/main/tools/system_image/Orin_Nano_Image_Readme.md">
                System image<br>installation description
            </a>
        </td>
        <td>-</td>
        <td>
            <a href="https://github.com/RoboSense-Robotics/robosense_ac_ros2_sdk_infra/blob/main/tools/system_image/RDK_X5_Image_Readme.md">
                System image<br>installation description
            </a>
        </td>
    </tr>
</table>

<sup>1</sup> ● (Solid Circle): Indicates support for a specific feature or functionality. <br> &nbsp; ○ (Hollow Circle): Indicates no support for a specific feature or functionality.

<sup>2</sup> The Active Camera SDK provides containers and system images on different platforms. The SDK container provides Docker containers for cross-platform compilation and local compilation environments, including container management, image management and automatic environment Settings. And the system image comes preinstalled with third-party dependencies for ros2 Humble and SDK.
